# Comparing `tmp/fastapi-0.96.1.tar.gz` & `tmp/fastapi-0.97.0.tar.gz`

## Comparing `fastapi-0.96.1.tar` & `fastapi-0.97.0.tar`

### file list

```diff
@@ -1,1875 +1,1879 @@
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 fastapi-0.96.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fastapi-0.96.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 fastapi-0.96.1/SECURITY.md
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 fastapi-0.96.1/.github/FUNDING.yml
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fastapi-0.96.1/.github/dependabot.yml
--rw-r--r--   0        0        0     5629 2020-02-02 00:00:00.000000 fastapi-0.96.1/.github/DISCUSSION_TEMPLATE/questions.yml
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 fastapi-0.96.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 fastapi-0.96.1/.github/ISSUE_TEMPLATE/privileged.yml
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 fastapi-0.96.1/.github/actions/comment-docs-preview-in-pr/Dockerfile
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 fastapi-0.96.1/.github/actions/comment-docs-preview-in-pr/action.yml
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 fastapi-0.96.1/.github/actions/comment-docs-preview-in-pr/app/main.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 fastapi-0.96.1/.github/actions/notify-translations/Dockerfile
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 fastapi-0.96.1/.github/actions/notify-translations/action.yml
--rw-r--r--   0        0        0    12661 2020-02-02 00:00:00.000000 fastapi-0.96.1/.github/actions/notify-translations/app/main.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 fastapi-0.96.1/.github/actions/people/Dockerfile
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 fastapi-0.96.1/.github/actions/people/action.yml
--rw-r--r--   0        0        0    19794 2020-02-02 00:00:00.000000 fastapi-0.96.1/.github/actions/people/app/main.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 fastapi-0.96.1/.github/actions/watch-previews/Dockerfile
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 fastapi-0.96.1/.github/actions/watch-previews/action.yml
--rw-r--r--   0        0        0     3407 2020-02-02 00:00:00.000000 fastapi-0.96.1/.github/actions/watch-previews/app/main.py
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 fastapi-0.96.1/.github/workflows/build-docs.yml
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 fastapi-0.96.1/.github/workflows/issue-manager.yml
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fastapi-0.96.1/.github/workflows/label-approved.yml
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 fastapi-0.96.1/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 fastapi-0.96.1/.github/workflows/notify-translations.yml
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 fastapi-0.96.1/.github/workflows/people.yml
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 fastapi-0.96.1/.github/workflows/preview-docs.yml
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 fastapi-0.96.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 fastapi-0.96.1/.github/workflows/smokeshow.yml
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 fastapi-0.96.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/missing-translation.md
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/az/mkdocs.yml
--rw-r--r--   0        0        0    18627 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/az/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/az/overrides/.gitignore
--rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/cs/mkdocs.yml
--rw-r--r--   0        0        0    19467 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/cs/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/cs/overrides/.gitignore
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/de/mkdocs.yml
--rw-r--r--   0        0        0    11231 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/de/docs/features.md
--rw-r--r--   0        0        0    18492 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/de/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/de/overrides/.gitignore
--rw-r--r--   0        0        0     6759 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/mkdocs.yml
--rw-r--r--   0        0        0    19136 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/alternatives.md
--rw-r--r--   0        0        0    19114 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/async.md
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/benchmarks.md
--rw-r--r--   0        0        0    11703 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/contributing.md
--rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/external-links.md
--rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/fastapi-people.md
--rw-r--r--   0        0        0     8409 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/features.md
--rw-r--r--   0        0        0    12235 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/help-fastapi.md
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/history-design-future.md
--rw-r--r--   0        0        0    17670 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/index.md
--rw-r--r--   0        0        0     4978 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/project-generation.md
--rw-r--r--   0        0        0    13966 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/python-types.md
--rw-r--r--   0        0        0     8055 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/advanced/additional-responses.md
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/advanced/additional-status-codes.md
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/advanced/advanced-dependencies.md
--rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/advanced/async-sql-databases.md
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/advanced/async-tests.md
--rw-r--r--   0        0        0    10306 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/advanced/behind-a-proxy.md
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/advanced/conditional-openapi.md
--rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/advanced/custom-request-and-route.md
--rw-r--r--   0        0        0     9988 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/advanced/custom-response.md
--rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/advanced/dataclasses.md
--rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/advanced/events.md
--rw-r--r--   0        0        0     9748 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/advanced/extending-openapi.md
--rw-r--r--   0        0        0     8663 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/advanced/generate-clients.md
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/advanced/graphql.md
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/advanced/index.md
--rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/advanced/middleware.md
--rw-r--r--   0        0        0     4917 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/advanced/nosql-databases.md
--rw-r--r--   0        0        0     6784 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/advanced/openapi-callbacks.md
--rw-r--r--   0        0        0     5886 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/advanced/path-operation-advanced-configuration.md
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/advanced/response-change-status-code.md
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/advanced/response-cookies.md
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/advanced/response-directly.md
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/advanced/response-headers.md
--rw-r--r--   0        0        0    11642 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/advanced/settings.md
--rw-r--r--   0        0        0    19705 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/advanced/sql-databases-peewee.md
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/advanced/sub-applications.md
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/advanced/templates.md
--rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/advanced/testing-database.md
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/advanced/testing-dependencies.md
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/advanced/testing-events.md
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/advanced/testing-websockets.md
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/advanced/using-request-directly.md
--rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/advanced/websockets.md
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/advanced/wsgi.md
--rw-r--r--   0        0        0     4160 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/advanced/security/http-basic-auth.md
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/advanced/security/index.md
--rw-r--r--   0        0        0    11325 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/advanced/security/oauth2-scopes.md
--rw-r--r--   0        0        0    14832 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/deployment/concepts.md
--rw-r--r--   0        0        0     6087 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/deployment/deta.md
--rw-r--r--   0        0        0    28740 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/deployment/docker.md
--rw-r--r--   0        0        0     9658 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/deployment/https.md
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/deployment/index.md
--rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/deployment/manually.md
--rw-r--r--   0        0        0     8396 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/deployment/server-workers.md
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/deployment/versions.md
--rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/background-tasks.md
--rw-r--r--   0        0        0    15678 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/bigger-applications.md
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/body-fields.md
--rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/body-multiple-params.md
--rw-r--r--   0        0        0     9408 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/body-nested-models.md
--rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/body-updates.md
--rw-r--r--   0        0        0     6683 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/body.md
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/cookie-params.md
--rw-r--r--   0        0        0     4170 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/cors.md
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/debugging.md
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/encoder.md
--rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/extra-data-types.md
--rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/extra-models.md
--rw-r--r--   0        0        0     8281 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/first-steps.md
--rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/handling-errors.md
--rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/header-params.md
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/index.md
--rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/metadata.md
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/middleware.md
--rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/path-operation-configuration.md
--rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/path-params-numeric-validations.md
--rw-r--r--   0        0        0     7878 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/path-params.md
--rw-r--r--   0        0        0    12188 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/query-params-str-validations.md
--rw-r--r--   0        0        0     4576 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/query-params.md
--rw-r--r--   0        0        0     6803 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/request-files.md
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/request-forms-and-files.md
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/request-forms.md
--rw-r--r--   0        0        0    16358 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/response-model.md
--rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/response-status-code.md
--rw-r--r--   0        0        0     5674 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/schema-extra-example.md
--rw-r--r--   0        0        0    25882 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/sql-databases.md
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/static-files.md
--rw-r--r--   0        0        0     5296 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/testing.md
--rw-r--r--   0        0        0     6134 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/dependencies/classes-as-dependencies.md
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/dependencies/dependencies-in-path-operation-decorators.md
--rw-r--r--   0        0        0     8941 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/dependencies/dependencies-with-yield.md
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/dependencies/global-dependencies.md
--rw-r--r--   0        0        0     6888 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/dependencies/index.md
--rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/dependencies/sub-dependencies.md
--rw-r--r--   0        0        0     6946 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/security/first-steps.md
--rw-r--r--   0        0        0     4474 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/security/get-current-user.md
--rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/security/index.md
--rw-r--r--   0        0        0     9718 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/security/oauth2-jwt.md
--rw-r--r--   0        0        0     9107 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/docs/tutorial/security/simple-oauth2.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/em/overrides/.gitignore
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/mkdocs.yml
--rw-r--r--   0        0        0    18874 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/data/external_links.yml
--rw-r--r--   0        0        0    25966 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/data/github_sponsors.yml
--rw-r--r--   0        0        0    22157 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/data/people.yml
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/data/sponsors.yml
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/data/sponsors_badge.yml
--rw-r--r--   0        0        0    23768 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/alternatives.md
--rw-r--r--   0        0        0    23576 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/async.md
--rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/benchmarks.md
--rw-r--r--   0        0        0    13719 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/contributing.md
--rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/external-links.md
--rw-r--r--   0        0        0     6515 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/fastapi-people.md
--rw-r--r--   0        0        0     9479 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/features.md
--rw-r--r--   0        0        0    14258 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/help-fastapi.md
--rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/history-design-future.md
--rw-r--r--   0        0        0    19423 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/index.md
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/newsletter.md
--rw-r--r--   0        0        0     5826 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/project-generation.md
--rw-r--r--   0        0        0    17461 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/python-types.md
--rw-r--r--   0        0        0   266822 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/release-notes.md
--rw-r--r--   0        0        0     8996 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/advanced/additional-responses.md
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/advanced/additional-status-codes.md
--rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/advanced/advanced-dependencies.md
--rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/advanced/async-sql-databases.md
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/advanced/async-tests.md
--rw-r--r--   0        0        0    11778 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/advanced/behind-a-proxy.md
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/advanced/conditional-openapi.md
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/advanced/custom-request-and-route.md
--rw-r--r--   0        0        0    11981 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/advanced/custom-response.md
--rw-r--r--   0        0        0     4248 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/advanced/dataclasses.md
--rw-r--r--   0        0        0     7828 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/advanced/events.md
--rw-r--r--   0        0        0    11429 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/advanced/extending-openapi.md
--rw-r--r--   0        0        0     9756 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/advanced/generate-clients.md
--rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/advanced/graphql.md
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/advanced/index.md
--rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/advanced/middleware.md
--rw-r--r--   0        0        0     5750 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/advanced/nosql-databases.md
--rw-r--r--   0        0        0     7934 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/advanced/openapi-callbacks.md
--rw-r--r--   0        0        0     7136 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/advanced/path-operation-advanced-configuration.md
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/advanced/response-change-status-code.md
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/advanced/response-cookies.md
--rw-r--r--   0        0        0     3060 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/advanced/response-directly.md
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/advanced/response-headers.md
--rw-r--r--   0        0        0    14584 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/advanced/settings.md
--rw-r--r--   0        0        0    23622 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/advanced/sql-databases-peewee.md
--rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/advanced/sub-applications.md
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/advanced/templates.md
--rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/advanced/testing-database.md
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/advanced/testing-dependencies.md
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/advanced/testing-events.md
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/advanced/testing-websockets.md
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/advanced/using-request-directly.md
--rw-r--r--   0        0        0     6370 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/advanced/websockets.md
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/advanced/wsgi.md
--rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/advanced/security/http-basic-auth.md
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/advanced/security/index.md
--rw-r--r--   0        0        0    20945 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/advanced/security/oauth2-scopes.md
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/css/custom.css
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/css/termynal.css
--rw-r--r--   0        0        0    18405 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/deployment/concepts.md
--rw-r--r--   0        0        0    13815 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/deployment/deta.md
--rw-r--r--   0        0        0    35157 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/deployment/docker.md
--rw-r--r--   0        0        0    12240 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/deployment/https.md
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/deployment/index.md
--rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/deployment/manually.md
--rw-r--r--   0        0        0     9364 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/deployment/server-workers.md
--rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/deployment/versions.md
--rwxr-xr-x   0        0        0      412 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/favicon.png
--rw-r--r--   0        0        0    58136 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/github-social-preview.png
--rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/github-social-preview.svg
--rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/icon-transparent-bg.png
--rw-r--r--   0        0        0     5210 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/icon-white-bg.png
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/icon-white.svg
--rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/logo-teal-vector.svg
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/logo-teal.svg
--rw-r--r--   0        0        0    51205 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/pycharm-completion.png
--rw-r--r--   0        0        0    62417 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/vscode-completion.png
--rw-r--r--   0        0        0   203390 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-01.png
--rw-r--r--   0        0        0   166992 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-02.png
--rw-r--r--   0        0        0   172943 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-03.png
--rw-r--r--   0        0        0   163423 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-04.png
--rw-r--r--   0        0        0   159869 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-05.png
--rw-r--r--   0        0        0   164838 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-06.png
--rw-r--r--   0        0        0   169968 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-07.png
--rw-r--r--   0        0        0   225993 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/async/parallel-burgers/parallel-burgers-01.png
--rw-r--r--   0        0        0   203644 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/async/parallel-burgers/parallel-burgers-02.png
--rw-r--r--   0        0        0   168628 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/async/parallel-burgers/parallel-burgers-03.png
--rw-r--r--   0        0        0   219429 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/async/parallel-burgers/parallel-burgers-04.png
--rw-r--r--   0        0        0   185116 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/async/parallel-burgers/parallel-burgers-05.png
--rw-r--r--   0        0        0   157113 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/async/parallel-burgers/parallel-burgers-06.png
--rw-r--r--   0        0        0   124827 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/deployment/concepts/image01.png
--rw-r--r--   0        0        0    10203 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/deployment/concepts/process-ram.drawio
--rw-r--r--   0        0        0    16640 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/deployment/concepts/process-ram.svg
--rw-r--r--   0        0        0    39996 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/deployment/deta/image01.png
--rw-r--r--   0        0        0    48297 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/deployment/deta/image02.png
--rw-r--r--   0        0        0    52704 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/deployment/deta/image03.png
--rw-r--r--   0        0        0    49760 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/deployment/deta/image04.png
--rw-r--r--   0        0        0    33130 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/deployment/deta/image05.png
--rw-r--r--   0        0        0   105270 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/deployment/deta/image06.png
--rw-r--r--   0        0        0    26363 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/deployment/https/https.drawio
--rw-r--r--   0        0        0    40488 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/deployment/https/https.svg
--rw-r--r--   0        0        0     6384 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/deployment/https/https01.drawio
--rw-r--r--   0        0        0    10583 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/deployment/https/https01.svg
--rw-r--r--   0        0        0     9636 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/deployment/https/https02.drawio
--rw-r--r--   0        0        0    15794 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/deployment/https/https02.svg
--rw-r--r--   0        0        0    12582 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/deployment/https/https03.drawio
--rw-r--r--   0        0        0    21549 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/deployment/https/https03.svg
--rw-r--r--   0        0        0    14291 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/deployment/https/https04.drawio
--rw-r--r--   0        0        0    23265 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/deployment/https/https04.svg
--rw-r--r--   0        0        0    15945 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/deployment/https/https05.drawio
--rw-r--r--   0        0        0    26167 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/deployment/https/https05.svg
--rw-r--r--   0        0        0    17470 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/deployment/https/https06.drawio
--rw-r--r--   0        0        0    27919 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/deployment/https/https06.svg
--rw-r--r--   0        0        0    19117 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/deployment/https/https07.drawio
--rw-r--r--   0        0        0    29659 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/deployment/https/https07.svg
--rw-r--r--   0        0        0    21427 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/deployment/https/https08.drawio
--rw-r--r--   0        0        0    33876 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/deployment/https/https08.svg
--rw-r--r--   0        0        0    74158 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/index/index-01-swagger-ui-simple.png
--rw-r--r--   0        0        0    68468 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/index/index-02-redoc-simple.png
--rw-r--r--   0        0        0    75099 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/index/index-03-swagger-02.png
--rw-r--r--   0        0        0    67572 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/index/index-04-swagger-03.png
--rw-r--r--   0        0        0    71441 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/index/index-05-swagger-04.png
--rw-r--r--   0        0        0    78842 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/index/index-06-redoc-02.png
--rw-r--r--   0        0        0     8036 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/logo-margin/logo-teal-vector.svg
--rw-r--r--   0        0        0    17680 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/logo-margin/logo-teal.png
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/logo-margin/logo-teal.svg
--rw-r--r--   0        0        0    21502 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/logo-margin/logo-white-bg.png
--rw-r--r--   0        0        0    17722 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/python-types/image01.png
--rw-r--r--   0        0        0    47799 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/python-types/image02.png
--rw-r--r--   0        0        0    42872 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/python-types/image03.png
--rw-r--r--   0        0        0    18604 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/python-types/image04.png
--rw-r--r--   0        0        0    42637 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/python-types/image05.png
--rw-r--r--   0        0        0    29581 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/python-types/image06.png
--rw-r--r--   0        0        0    37057 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/budget-insight.svg
--rw-r--r--   0        0        0    16949 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/calmcode.jpg
--rw-r--r--   0        0        0     5321 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/classiq-banner.png
--rw-r--r--   0        0        0     6286 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/classiq.png
--rw-r--r--   0        0        0   133690 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/cryptapi-banner.svg
--rw-r--r--   0        0        0   111142 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/cryptapi.svg
--rw-r--r--   0        0        0   122267 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/databento.svg
--rw-r--r--   0        0        0    38162 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/deta-banner.svg
--rw-r--r--   0        0        0    56518 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/deta.svg
--rw-r--r--   0        0        0   110000 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/docarray-top-banner.svg
--rw-r--r--   0        0        0   129629 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/docarray.svg
--rw-r--r--   0        0        0    53417 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/doist-banner.svg
--rw-r--r--   0        0        0    93166 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/doist.svg
--rw-r--r--   0        0        0    21211 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/dropbase-banner.svg
--rw-r--r--   0        0        0     7520 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/dropbase.svg
--rw-r--r--   0        0        0    10556 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/exoflare.png
--rw-r--r--   0        0        0    16235 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/fastapi-course-bundle-banner.png
--rw-r--r--   0        0        0    34985 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/fastapi-course-bundle-banner.svg
--rw-r--r--   0        0        0    31985 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/haystack-fastapi.svg
--rw-r--r--   0        0        0   107893 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/imgwhale-banner.svg
--rw-r--r--   0        0        0   108995 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/imgwhale.svg
--rw-r--r--   0        0        0    11727 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/ines-course.jpg
--rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/investsuite.svg
--rw-r--r--   0        0        0    14153 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/jina-ai-banner.png
--rw-r--r--   0        0        0    26112 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/jina-ai.png
--rw-r--r--   0        0        0    42239 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/jina-banner.svg
--rw-r--r--   0        0        0   162873 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/jina-top-banner.svg
--rw-r--r--   0        0        0   220435 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/jina.svg
--rw-r--r--   0        0        0   108837 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/jina2.svg
--rw-r--r--   0        0        0     6313 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/platform-sh-banner.png
--rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/platform-sh.png
--rw-r--r--   0        0        0    15311 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/powens.png
--rw-r--r--   0        0        0     9681 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/striveworks-banner.png
--rw-r--r--   0        0        0    22639 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/striveworks.png
--rw-r--r--   0        0        0    34780 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/striveworks2.png
--rw-r--r--   0        0        0    22430 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/svix.svg
--rw-r--r--   0        0        0    14807 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/talkpython.png
--rw-r--r--   0        0        0    26425 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/testdriven.svg
--rw-r--r--   0        0        0    15198 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/vimso.png
--rw-r--r--   0        0        0     6944 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/sponsors/wetransfer.svg
--rw-r--r--   0        0        0    72424 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/additional-responses/image01.png
--rw-r--r--   0        0        0    70687 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/async-sql-databases/image01.png
--rw-r--r--   0        0        0    29123 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/behind-a-proxy/image01.png
--rw-r--r--   0        0        0    62026 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/behind-a-proxy/image02.png
--rw-r--r--   0        0        0    74280 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/behind-a-proxy/image03.png
--rw-r--r--   0        0        0    74516 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/bigger-applications/image01.png
--rw-r--r--   0        0        0     6230 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/bigger-applications/package.drawio
--rw-r--r--   0        0        0    14368 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/bigger-applications/package.svg
--rw-r--r--   0        0        0    55506 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/body/image01.png
--rw-r--r--   0        0        0    81208 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/body/image02.png
--rw-r--r--   0        0        0    66011 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/body/image03.png
--rw-r--r--   0        0        0    40151 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/body/image04.png
--rw-r--r--   0        0        0    52951 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/body/image05.png
--rw-r--r--   0        0        0    78746 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/body-fields/image01.png
--rw-r--r--   0        0        0    93828 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/body-fields/image02.png
--rw-r--r--   0        0        0    40992 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/body-nested-models/image01.png
--rw-r--r--   0        0        0    54866 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/custom-response/image01.png
--rw-r--r--   0        0        0    72574 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/dataclasses/image01.png
--rw-r--r--   0        0        0   173614 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/debugging/image01.png
--rw-r--r--   0        0        0    99443 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/debugging/image02.png
--rw-r--r--   0        0        0    79658 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/dependencies/image01.png
--rw-r--r--   0        0        0    66817 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/dependencies/image02.png
--rw-r--r--   0        0        0    64786 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/extending-openapi/image01.png
--rw-r--r--   0        0        0    11292 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/extending-openapi/image02.png
--rw-r--r--   0        0        0    11176 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/extending-openapi/image03.png
--rw-r--r--   0        0        0    11180 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/extending-openapi/image04.png
--rw-r--r--   0        0        0    78022 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/generate-clients/image01.png
--rw-r--r--   0        0        0    59828 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/generate-clients/image02.png
--rw-r--r--   0        0        0    61043 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/generate-clients/image03.png
--rw-r--r--   0        0        0    53853 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/generate-clients/image04.png
--rw-r--r--   0        0        0    31091 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/generate-clients/image05.png
--rw-r--r--   0        0        0    43434 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/generate-clients/image06.png
--rw-r--r--   0        0        0    49947 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/generate-clients/image07.png
--rw-r--r--   0        0        0    30019 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/generate-clients/image08.png
--rw-r--r--   0        0        0    95541 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/graphql/image01.png
--rw-r--r--   0        0        0    90062 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/metadata/image01.png
--rw-r--r--   0        0        0    47719 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/metadata/image02.png
--rw-r--r--   0        0        0    99295 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/openapi-callbacks/image01.png
--rw-r--r--   0        0        0    68080 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/path-operation-advanced-configuration/image01.png
--rw-r--r--   0        0        0    41919 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/path-operation-configuration/image01.png
--rw-r--r--   0        0        0    86975 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/path-operation-configuration/image02.png
--rw-r--r--   0        0        0    71050 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/path-operation-configuration/image03.png
--rw-r--r--   0        0        0    38687 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/path-operation-configuration/image04.png
--rw-r--r--   0        0        0    74423 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/path-operation-configuration/image05.png
--rw-r--r--   0        0        0    79109 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/path-params/image01.png
--rw-r--r--   0        0        0    67289 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/path-params/image02.png
--rw-r--r--   0        0        0   118540 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/path-params/image03.png
--rw-r--r--   0        0        0    86345 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/query-params-str-validations/image01.png
--rw-r--r--   0        0        0    72770 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/query-params-str-validations/image02.png
--rw-r--r--   0        0        0    76191 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/response-model/image01.png
--rw-r--r--   0        0        0    89115 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/response-model/image02.png
--rw-r--r--   0        0        0    74275 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/response-status-code/image01.png
--rw-r--r--   0        0        0    30455 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/response-status-code/image02.png
--rw-r--r--   0        0        0    53959 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/security/image01.png
--rw-r--r--   0        0        0    90212 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/security/image02.png
--rw-r--r--   0        0        0    92466 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/security/image03.png
--rw-r--r--   0        0        0    84481 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/security/image04.png
--rw-r--r--   0        0        0    81962 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/security/image05.png
--rw-r--r--   0        0        0    91545 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/security/image06.png
--rw-r--r--   0        0        0    61135 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/security/image07.png
--rw-r--r--   0        0        0    88705 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/security/image08.png
--rw-r--r--   0        0        0   110760 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/security/image09.png
--rw-r--r--   0        0        0   159081 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/security/image10.png
--rw-r--r--   0        0        0    77654 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/security/image11.png
--rw-r--r--   0        0        0    69280 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/security/image12.png
--rw-r--r--   0        0        0    78949 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/sql-databases/image01.png
--rw-r--r--   0        0        0    83482 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/sql-databases/image02.png
--rw-r--r--   0        0        0    50472 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/sub-applications/image01.png
--rw-r--r--   0        0        0    53366 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/sub-applications/image02.png
--rw-r--r--   0        0        0    17229 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/websockets/image01.png
--rw-r--r--   0        0        0    18326 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/websockets/image02.png
--rw-r--r--   0        0        0    21283 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/websockets/image03.png
--rw-r--r--   0        0        0    30900 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/websockets/image04.png
--rw-r--r--   0        0        0    53330 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/img/tutorial/websockets/image05.png
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/js/chat.js
--rw-r--r--   0        0        0     6734 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/js/custom.js
--rw-r--r--   0        0        0     9540 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/js/termynal.js
--rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/background-tasks.md
--rw-r--r--   0        0        0    18654 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/bigger-applications.md
--rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/body-fields.md
--rw-r--r--   0        0        0     7858 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/body-multiple-params.md
--rw-r--r--   0        0        0     9735 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/body-nested-models.md
--rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/body-updates.md
--rw-r--r--   0        0        0     7443 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/body.md
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/cookie-params.md
--rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/cors.md
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/debugging.md
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/encoder.md
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/extra-data-types.md
--rw-r--r--   0        0        0     7567 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/extra-models.md
--rw-r--r--   0        0        0     9445 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/first-steps.md
--rw-r--r--   0        0        0     9368 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/handling-errors.md
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/header-params.md
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/index.md
--rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/metadata.md
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/middleware.md
--rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/path-operation-configuration.md
--rw-r--r--   0        0        0     9281 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/path-params-numeric-validations.md
--rw-r--r--   0        0        0     9279 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/path-params.md
--rw-r--r--   0        0        0    26454 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/query-params-str-validations.md
--rw-r--r--   0        0        0     5210 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/query-params.md
--rw-r--r--   0        0        0    10449 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/request-files.md
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/request-forms-and-files.md
--rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/request-forms.md
--rw-r--r--   0        0        0    18046 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/response-model.md
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/response-status-code.md
--rw-r--r--   0        0        0     7356 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/schema-extra-example.md
--rw-r--r--   0        0        0    29642 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/sql-databases.md
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/static-files.md
--rw-r--r--   0        0        0     6380 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/testing.md
--rw-r--r--   0        0        0    11622 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/dependencies/classes-as-dependencies.md
--rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/dependencies/dependencies-in-path-operation-decorators.md
--rw-r--r--   0        0        0    10848 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/dependencies/dependencies-with-yield.md
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/dependencies/global-dependencies.md
--rw-r--r--   0        0        0    11871 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/dependencies/index.md
--rw-r--r--   0        0        0     5742 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/dependencies/sub-dependencies.md
--rw-r--r--   0        0        0     9112 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/security/first-steps.md
--rw-r--r--   0        0        0     7774 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/security/get-current-user.md
--rw-r--r--   0        0        0     4403 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/security/index.md
--rw-r--r--   0        0        0    13286 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/security/oauth2-jwt.md
--rw-r--r--   0        0        0    12787 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/docs/tutorial/security/simple-oauth2.md
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/en/overrides/main.html
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/es/mkdocs.yml
--rw-r--r--   0        0        0    25513 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/es/docs/async.md
--rw-r--r--   0        0        0    11468 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/es/docs/features.md
--rw-r--r--   0        0        0    19594 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/es/docs/index.md
--rw-r--r--   0        0        0     9390 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/es/docs/python-types.md
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/es/docs/advanced/additional-status-codes.md
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/es/docs/advanced/index.md
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/es/docs/advanced/path-operation-advanced-configuration.md
--rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/es/docs/advanced/response-directly.md
--rw-r--r--   0        0        0    10139 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/es/docs/tutorial/first-steps.md
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/es/docs/tutorial/index.md
--rw-r--r--   0        0        0     9681 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/es/docs/tutorial/path-params.md
--rw-r--r--   0        0        0     5207 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/es/docs/tutorial/query-params.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/es/overrides/.gitignore
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/fa/mkdocs.yml
--rw-r--r--   0        0        0    26736 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/fa/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/fa/overrides/.gitignore
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/fr/mkdocs.yml
--rw-r--r--   0        0        0    28159 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/fr/docs/alternatives.md
--rw-r--r--   0        0        0    24572 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/fr/docs/async.md
--rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/fr/docs/external-links.md
--rw-r--r--   0        0        0     6890 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/fr/docs/fastapi-people.md
--rw-r--r--   0        0        0    11587 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/fr/docs/features.md
--rw-r--r--   0        0        0     7339 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/fr/docs/help-fastapi.md
--rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/fr/docs/history-design-future.md
--rw-r--r--   0        0        0    22777 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/fr/docs/index.md
--rw-r--r--   0        0        0     6902 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/fr/docs/project-generation.md
--rw-r--r--   0        0        0    10567 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/fr/docs/python-types.md
--rw-r--r--   0        0        0     9841 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/fr/docs/advanced/additional-responses.md
--rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/fr/docs/advanced/additional-status-codes.md
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/fr/docs/advanced/index.md
--rw-r--r--   0        0        0     8141 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/fr/docs/advanced/path-operation-advanced-configuration.md
--rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/fr/docs/advanced/response-directly.md
--rw-r--r--   0        0        0     6356 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/fr/docs/deployment/deta.md
--rw-r--r--   0        0        0     7687 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/fr/docs/deployment/docker.md
--rw-r--r--   0        0        0     4236 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/fr/docs/deployment/https.md
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/fr/docs/deployment/index.md
--rw-r--r--   0        0        0     5515 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/fr/docs/deployment/manually.md
--rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/fr/docs/deployment/versions.md
--rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/fr/docs/tutorial/background-tasks.md
--rw-r--r--   0        0        0     7999 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/fr/docs/tutorial/body.md
--rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/fr/docs/tutorial/debugging.md
--rw-r--r--   0        0        0    10563 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/fr/docs/tutorial/first-steps.md
--rw-r--r--   0        0        0    10228 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/fr/docs/tutorial/path-params.md
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/fr/docs/tutorial/query-params.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/fr/overrides/.gitignore
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/he/mkdocs.yml
--rw-r--r--   0        0        0    21849 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/he/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/he/overrides/.gitignore
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/hy/mkdocs.yml
--rw-r--r--   0        0        0    18893 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/hy/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/hy/overrides/.gitignore
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/id/mkdocs.yml
--rw-r--r--   0        0        0    18622 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/id/docs/index.md
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/id/docs/tutorial/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/id/overrides/.gitignore
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/it/mkdocs.yml
--rw-r--r--   0        0        0    18542 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/it/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/it/overrides/.gitignore
--rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/mkdocs.yml
--rw-r--r--   0        0        0    32353 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/alternatives.md
--rw-r--r--   0        0        0    28468 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/async.md
--rw-r--r--   0        0        0     4465 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/benchmarks.md
--rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/contributing.md
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/external-links.md
--rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/fastapi-people.md
--rw-r--r--   0        0        0    12779 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/features.md
--rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/help-fastapi.md
--rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/history-design-future.md
--rw-r--r--   0        0        0    21628 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/index.md
--rw-r--r--   0        0        0     7264 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/project-generation.md
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/advanced/additional-status-codes.md
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/advanced/conditional-openapi.md
--rw-r--r--   0        0        0    10906 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/advanced/custom-response.md
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/advanced/index.md
--rw-r--r--   0        0        0     7142 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/advanced/nosql-databases.md
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/advanced/path-operation-advanced-configuration.md
--rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/advanced/response-directly.md
--rw-r--r--   0        0        0     7405 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/advanced/websockets.md
--rw-r--r--   0        0        0     6667 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/deployment/deta.md
--rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/deployment/docker.md
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/deployment/index.md
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/deployment/manually.md
--rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/deployment/versions.md
--rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/tutorial/body-updates.md
--rw-r--r--   0        0        0     8130 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/tutorial/body.md
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/tutorial/cookie-params.md
--rw-r--r--   0        0        0     6422 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/tutorial/cors.md
--rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/tutorial/debugging.md
--rw-r--r--   0        0        0    11456 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/tutorial/first-steps.md
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/tutorial/header-params.md
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/tutorial/index.md
--rw-r--r--   0        0        0     3905 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/tutorial/middleware.md
--rw-r--r--   0        0        0    10867 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/tutorial/path-params.md
--rw-r--r--   0        0        0    10789 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/tutorial/query-params-str-validations.md
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/tutorial/query-params.md
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/tutorial/request-forms.md
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/tutorial/static-files.md
--rw-r--r--   0        0        0     5977 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/tutorial/testing.md
--rw-r--r--   0        0        0    10737 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/tutorial/security/first-steps.md
--rw-r--r--   0        0        0    14484 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/docs/tutorial/security/oauth2-jwt.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ja/overrides/.gitignore
--rw-r--r--   0        0        0     3921 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ko/mkdocs.yml
--rw-r--r--   0        0        0    20074 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ko/docs/index.md
--rw-r--r--   0        0        0     4217 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ko/docs/deployment/versions.md
--rw-r--r--   0        0        0     5905 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ko/docs/tutorial/cors.md
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ko/docs/tutorial/encoder.md
--rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ko/docs/tutorial/first-steps.md
--rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ko/docs/tutorial/header-params.md
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ko/docs/tutorial/index.md
--rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ko/docs/tutorial/path-params-numeric-validations.md
--rw-r--r--   0        0        0     9880 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ko/docs/tutorial/path-params.md
--rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ko/docs/tutorial/query-params.md
--rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ko/docs/tutorial/request-files.md
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ko/docs/tutorial/request-forms-and-files.md
--rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ko/docs/tutorial/response-status-code.md
--rw-r--r--   0        0        0     8167 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ko/docs/tutorial/dependencies/classes-as-dependencies.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ko/overrides/.gitignore
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/lo/mkdocs.yml
--rw-r--r--   0        0        0    19423 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/lo/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/lo/overrides/.gitignore
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/nl/mkdocs.yml
--rw-r--r--   0        0        0    18863 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/nl/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/nl/overrides/.gitignore
--rw-r--r--   0        0        0     3542 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pl/mkdocs.yml
--rw-r--r--   0        0        0    20000 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pl/docs/index.md
--rw-r--r--   0        0        0    10055 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pl/docs/tutorial/first-steps.md
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pl/docs/tutorial/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pl/overrides/.gitignore
--rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/mkdocs.yml
--rw-r--r--   0        0        0    26158 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/alternatives.md
--rw-r--r--   0        0        0    22758 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/async.md
--rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/benchmarks.md
--rw-r--r--   0        0        0    15230 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/contributing.md
--rw-r--r--   0        0        0    17171 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/deployment.md
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/external-links.md
--rw-r--r--   0        0        0     6586 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/fastapi-people.md
--rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/features.md
--rw-r--r--   0        0        0     8848 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/help-fastapi.md
--rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/history-design-future.md
--rw-r--r--   0        0        0    19250 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/index.md
--rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/project-generation.md
--rw-r--r--   0        0        0     9892 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/python-types.md
--rw-r--r--   0        0        0     8854 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/advanced/events.md
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/advanced/index.md
--rw-r--r--   0        0        0     7211 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/deployment/deta.md
--rw-r--r--   0        0        0    38309 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/deployment/docker.md
--rw-r--r--   0        0        0     3979 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/deployment/https.md
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/deployment/index.md
--rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/deployment/versions.md
--rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/tutorial/background-tasks.md
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/tutorial/body-fields.md
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/tutorial/body-multiple-params.md
--rw-r--r--   0        0        0     7563 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/tutorial/body-nested-models.md
--rw-r--r--   0        0        0     7294 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/tutorial/body.md
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/tutorial/cookie-params.md
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/tutorial/encoder.md
--rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/tutorial/extra-data-types.md
--rw-r--r--   0        0        0     8000 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/tutorial/extra-models.md
--rw-r--r--   0        0        0     9849 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/tutorial/first-steps.md
--rw-r--r--   0        0        0    10274 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/tutorial/handling-errors.md
--rw-r--r--   0        0        0     3974 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/tutorial/header-params.md
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/tutorial/index.md
--rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/tutorial/path-operation-configuration.md
--rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/tutorial/path-params-numeric-validations.md
--rw-r--r--   0        0        0     9946 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/tutorial/path-params.md
--rw-r--r--   0        0        0     9547 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/tutorial/query-params-str-validations.md
--rw-r--r--   0        0        0     5688 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/tutorial/query-params.md
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/tutorial/request-forms-and-files.md
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/tutorial/request-forms.md
--rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/tutorial/response-status-code.md
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/tutorial/static-files.md
--rw-r--r--   0        0        0     8499 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/tutorial/security/first-steps.md
--rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/docs/tutorial/security/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/pt/overrides/.gitignore
--rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ru/mkdocs.yml
--rw-r--r--   0        0        0    40311 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ru/docs/alternatives.md
--rw-r--r--   0        0        0    40878 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ru/docs/async.md
--rw-r--r--   0        0        0     6201 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ru/docs/benchmarks.md
--rw-r--r--   0        0        0    23067 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ru/docs/contributing.md
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ru/docs/external-links.md
--rw-r--r--   0        0        0     8880 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ru/docs/fastapi-people.md
--rw-r--r--   0        0        0    16914 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ru/docs/features.md
--rw-r--r--   0        0        0    23415 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ru/docs/help-fastapi.md
--rw-r--r--   0        0        0     7421 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ru/docs/history-design-future.md
--rw-r--r--   0        0        0    26659 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ru/docs/index.md
--rw-r--r--   0        0        0    10763 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ru/docs/project-generation.md
--rw-r--r--   0        0        0    14967 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ru/docs/python-types.md
--rw-r--r--   0        0        0    33259 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ru/docs/deployment/concepts.md
--rw-r--r--   0        0        0    21137 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ru/docs/deployment/https.md
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ru/docs/deployment/index.md
--rw-r--r--   0        0        0     7961 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ru/docs/deployment/manually.md
--rw-r--r--   0        0        0     5793 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ru/docs/deployment/versions.md
--rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ru/docs/tutorial/background-tasks.md
--rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ru/docs/tutorial/body-fields.md
--rw-r--r--   0        0        0    11923 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ru/docs/tutorial/body-multiple-params.md
--rw-r--r--   0        0        0    11229 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ru/docs/tutorial/body.md
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ru/docs/tutorial/cookie-params.md
--rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ru/docs/tutorial/debugging.md
--rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ru/docs/tutorial/extra-data-types.md
--rw-r--r--   0        0        0    13423 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ru/docs/tutorial/first-steps.md
--rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ru/docs/tutorial/index.md
--rw-r--r--   0        0        0    14571 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ru/docs/tutorial/path-params-numeric-validations.md
--rw-r--r--   0        0        0    14436 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ru/docs/tutorial/path-params.md
--rw-r--r--   0        0        0    38884 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ru/docs/tutorial/query-params-str-validations.md
--rw-r--r--   0        0        0     8575 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ru/docs/tutorial/query-params.md
--rw-r--r--   0        0        0     7166 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ru/docs/tutorial/response-status-code.md
--rw-r--r--   0        0        0    11861 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ru/docs/tutorial/schema-extra-example.md
--rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ru/docs/tutorial/static-files.md
--rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ru/docs/tutorial/testing.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ru/overrides/.gitignore
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/sq/mkdocs.yml
--rw-r--r--   0        0        0    18625 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/sq/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/sq/overrides/.gitignore
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/sv/mkdocs.yml
--rw-r--r--   0        0        0    18863 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/sv/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/sv/overrides/.gitignore
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ta/mkdocs.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/ta/overrides/.gitignore
--rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/tr/mkdocs.yml
--rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/tr/docs/benchmarks.md
--rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/tr/docs/fastapi-people.md
--rw-r--r--   0        0        0    11579 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/tr/docs/features.md
--rw-r--r--   0        0        0    20806 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/tr/docs/index.md
--rw-r--r--   0        0        0     9971 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/tr/docs/python-types.md
--rw-r--r--   0        0        0    10004 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/tr/docs/tutorial/first_steps.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/tr/overrides/.gitignore
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/uk/mkdocs.yml
--rw-r--r--   0        0        0    18625 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/uk/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/uk/overrides/.gitignore
--rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/mkdocs.yml
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/benchmarks.md
--rw-r--r--   0        0        0    13648 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/contributing.md
--rw-r--r--   0        0        0     6177 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/fastapi-people.md
--rw-r--r--   0        0        0     9335 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/features.md
--rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/help-fastapi.md
--rw-r--r--   0        0        0    18563 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/index.md
--rw-r--r--   0        0        0     8827 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/python-types.md
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/advanced/additional-status-codes.md
--rw-r--r--   0        0        0     7939 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/advanced/custom-response.md
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/advanced/index.md
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/advanced/path-operation-advanced-configuration.md
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/advanced/response-change-status-code.md
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/advanced/response-cookies.md
--rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/advanced/response-directly.md
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/advanced/response-headers.md
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/advanced/wsgi.md
--rw-r--r--   0        0        0    18647 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/bigger-applications.md
--rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/body-fields.md
--rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/body-multiple-params.md
--rw-r--r--   0        0        0     7030 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/body-nested-models.md
--rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/body-updates.md
--rw-r--r--   0        0        0     5620 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/body.md
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/cookie-params.md
--rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/cors.md
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/debugging.md
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/encoder.md
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/extra-data-types.md
--rw-r--r--   0        0        0     6065 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/extra-models.md
--rw-r--r--   0        0        0     9408 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/first-steps.md
--rw-r--r--   0        0        0     8638 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/handling-errors.md
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/header-params.md
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/index.md
--rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/metadata.md
--rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/middleware.md
--rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/path-operation-configuration.md
--rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/path-params-numeric-validations.md
--rw-r--r--   0        0        0     8476 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/path-params.md
--rw-r--r--   0        0        0     9302 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/query-params-str-validations.md
--rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/query-params.md
--rw-r--r--   0        0        0     7072 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/request-files.md
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/request-forms-and-files.md
--rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/request-forms.md
--rw-r--r--   0        0        0     7297 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/response-model.md
--rw-r--r--   0        0        0     4110 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/response-status-code.md
--rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/schema-extra-example.md
--rw-r--r--   0        0        0    27546 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/sql-databases.md
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/static-files.md
--rw-r--r--   0        0        0     6650 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/dependencies/classes-as-dependencies.md
--rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/dependencies/dependencies-in-path-operation-decorators.md
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/dependencies/global-dependencies.md
--rw-r--r--   0        0        0     7202 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/dependencies/index.md
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/dependencies/sub-dependencies.md
--rw-r--r--   0        0        0     7256 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/security/first-steps.md
--rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/security/get-current-user.md
--rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/security/index.md
--rw-r--r--   0        0        0     9457 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/security/oauth2-jwt.md
--rw-r--r--   0        0        0     9566 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/docs/tutorial/security/simple-oauth2.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs/zh/overrides/.gitignore
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/additional_responses/tutorial001.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/additional_responses/tutorial002.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/additional_responses/tutorial003.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/additional_responses/tutorial004.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/additional_status_codes/tutorial001.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/additional_status_codes/tutorial001_an.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/additional_status_codes/tutorial001_an_py310.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/additional_status_codes/tutorial001_an_py39.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/additional_status_codes/tutorial001_py310.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/advanced_middleware/tutorial001.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/advanced_middleware/tutorial002.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/advanced_middleware/tutorial003.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/app_testing/__init__.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/app_testing/main.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/app_testing/test_main.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/app_testing/tutorial001.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/app_testing/tutorial002.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/app_testing/tutorial003.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/app_testing/app_b/__init__.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/app_testing/app_b/main.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/app_testing/app_b/test_main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/app_testing/app_b_an/__init__.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/app_testing/app_b_an/main.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/app_testing/app_b_an/test_main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/app_testing/app_b_an_py310/__init__.py
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/app_testing/app_b_an_py310/main.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/app_testing/app_b_an_py310/test_main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/app_testing/app_b_an_py39/__init__.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/app_testing/app_b_an_py39/main.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/app_testing/app_b_an_py39/test_main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/app_testing/app_b_py310/__init__.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/app_testing/app_b_py310/main.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/app_testing/app_b_py310/test_main.py
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/async_sql_databases/tutorial001.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/async_tests/__init__.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/async_tests/main.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/async_tests/test_main.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/background_tasks/tutorial001.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/background_tasks/tutorial002.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/background_tasks/tutorial002_an.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/background_tasks/tutorial002_an_py310.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/background_tasks/tutorial002_an_py39.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/background_tasks/tutorial002_py310.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/behind_a_proxy/tutorial001.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/behind_a_proxy/tutorial002.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/behind_a_proxy/tutorial003.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/behind_a_proxy/tutorial004.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/bigger_applications/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/bigger_applications/app/__init__.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/bigger_applications/app/dependencies.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/bigger_applications/app/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/bigger_applications/app/internal/__init__.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/bigger_applications/app/internal/admin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/bigger_applications/app/routers/__init__.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/bigger_applications/app/routers/items.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/bigger_applications/app/routers/users.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/bigger_applications/app_an/__init__.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/bigger_applications/app_an/dependencies.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/bigger_applications/app_an/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/bigger_applications/app_an/internal/__init__.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/bigger_applications/app_an/internal/admin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/bigger_applications/app_an/routers/__init__.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/bigger_applications/app_an/routers/items.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/bigger_applications/app_an/routers/users.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/bigger_applications/app_an_py39/__init__.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/bigger_applications/app_an_py39/dependencies.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/bigger_applications/app_an_py39/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/bigger_applications/app_an_py39/internal/__init__.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/bigger_applications/app_an_py39/internal/admin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/bigger_applications/app_an_py39/routers/__init__.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/bigger_applications/app_an_py39/routers/items.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/bigger_applications/app_an_py39/routers/users.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body/tutorial001.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body/tutorial001_py310.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body/tutorial002.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body/tutorial002_py310.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body/tutorial003.py
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body/tutorial003_py310.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body/tutorial004.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body/tutorial004_py310.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_fields/tutorial001.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_fields/tutorial001_an.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_fields/tutorial001_an_py310.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_fields/tutorial001_an_py39.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_fields/tutorial001_py310.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_multiple_params/tutorial001.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_multiple_params/tutorial001_an.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_multiple_params/tutorial001_an_py310.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_multiple_params/tutorial001_an_py39.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_multiple_params/tutorial001_py310.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_multiple_params/tutorial002.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_multiple_params/tutorial002_py310.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_multiple_params/tutorial003.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_multiple_params/tutorial003_an.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_multiple_params/tutorial003_an_py310.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_multiple_params/tutorial003_an_py39.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_multiple_params/tutorial003_py310.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_multiple_params/tutorial004.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_multiple_params/tutorial004_an.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_multiple_params/tutorial004_an_py310.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_multiple_params/tutorial004_an_py39.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_multiple_params/tutorial004_py310.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_multiple_params/tutorial005.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_multiple_params/tutorial005_an.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_multiple_params/tutorial005_an_py310.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_multiple_params/tutorial005_an_py39.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_multiple_params/tutorial005_py310.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_nested_models/tutorial001.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_nested_models/tutorial001_py310.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_nested_models/tutorial002.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_nested_models/tutorial002_py310.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_nested_models/tutorial002_py39.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_nested_models/tutorial003.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_nested_models/tutorial003_py310.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_nested_models/tutorial003_py39.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_nested_models/tutorial004.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_nested_models/tutorial004_py310.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_nested_models/tutorial004_py39.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_nested_models/tutorial005.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_nested_models/tutorial005_py310.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_nested_models/tutorial005_py39.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_nested_models/tutorial006.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_nested_models/tutorial006_py310.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_nested_models/tutorial006_py39.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_nested_models/tutorial007.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_nested_models/tutorial007_py310.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_nested_models/tutorial007_py39.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_nested_models/tutorial008.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_nested_models/tutorial008_py39.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_nested_models/tutorial009.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_nested_models/tutorial009_py39.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_updates/tutorial001.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_updates/tutorial001_py310.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_updates/tutorial001_py39.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_updates/tutorial002.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_updates/tutorial002_py310.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/body_updates/tutorial002_py39.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/conditional_openapi/tutorial001.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/cookie_params/tutorial001.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/cookie_params/tutorial001_an.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/cookie_params/tutorial001_an_py310.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/cookie_params/tutorial001_an_py39.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/cookie_params/tutorial001_py310.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/cors/tutorial001.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/custom_request_and_route/tutorial001.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/custom_request_and_route/tutorial002.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/custom_request_and_route/tutorial003.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/custom_response/tutorial001.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/custom_response/tutorial001b.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/custom_response/tutorial002.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/custom_response/tutorial003.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/custom_response/tutorial004.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/custom_response/tutorial005.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/custom_response/tutorial006.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/custom_response/tutorial006b.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/custom_response/tutorial006c.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/custom_response/tutorial007.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/custom_response/tutorial008.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/custom_response/tutorial009.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/custom_response/tutorial009b.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/custom_response/tutorial009c.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/custom_response/tutorial010.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dataclasses/tutorial001.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dataclasses/tutorial002.py
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dataclasses/tutorial003.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/debugging/tutorial001.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial001.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial001_02_an.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial001_02_an_py310.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial001_02_an_py39.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial001_an.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial001_an_py310.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial001_an_py39.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial001_py310.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial002.py
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial002_an.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial002_an_py310.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial002_an_py39.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial002_py310.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial003.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial003_an.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial003_an_py310.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial003_an_py39.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial003_py310.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial004.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial004_an.py
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial004_an_py310.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial004_an_py39.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial004_py310.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial005.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial005_an.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial005_an_py310.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial005_an_py39.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial005_py310.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial006.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial006_an.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial006_an_py39.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial007.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial008.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial008_an.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial008_an_py39.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial009.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial010.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial011.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial011_an.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial011_an_py39.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial012.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial012_an.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependencies/tutorial012_an_py39.py
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependency_testing/tutorial001.py
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependency_testing/tutorial001_an.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependency_testing/tutorial001_an_py310.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependency_testing/tutorial001_an_py39.py
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/dependency_testing/tutorial001_py310.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/encoder/tutorial001.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/encoder/tutorial001_py310.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/events/tutorial001.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/events/tutorial002.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/events/tutorial003.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/extending_openapi/tutorial001.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/extending_openapi/tutorial002.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/extending_openapi/tutorial003.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/extending_openapi/tutorial004.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/extending_openapi/tutorial005.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/extra_data_types/tutorial001.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/extra_data_types/tutorial001_an.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/extra_data_types/tutorial001_an_py310.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/extra_data_types/tutorial001_an_py39.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/extra_data_types/tutorial001_py310.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/extra_models/tutorial001.py
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/extra_models/tutorial001_py310.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/extra_models/tutorial002.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/extra_models/tutorial002_py310.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/extra_models/tutorial003.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/extra_models/tutorial003_py310.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/extra_models/tutorial004.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/extra_models/tutorial004_py39.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/extra_models/tutorial005.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/extra_models/tutorial005_py39.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/first_steps/tutorial001.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/first_steps/tutorial002.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/first_steps/tutorial003.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/generate_clients/tutorial001.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/generate_clients/tutorial001_py39.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/generate_clients/tutorial002.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/generate_clients/tutorial002_py39.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/generate_clients/tutorial003.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/generate_clients/tutorial003_py39.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/generate_clients/tutorial004.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/graphql/tutorial001.py
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/handling_errors/tutorial001.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/handling_errors/tutorial002.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/handling_errors/tutorial003.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/handling_errors/tutorial004.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/handling_errors/tutorial005.py
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/handling_errors/tutorial006.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/header_params/tutorial001.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/header_params/tutorial001_an.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/header_params/tutorial001_an_py310.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/header_params/tutorial001_an_py39.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/header_params/tutorial001_py310.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/header_params/tutorial002.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/header_params/tutorial002_an.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/header_params/tutorial002_an_py310.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/header_params/tutorial002_an_py39.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/header_params/tutorial002_py310.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/header_params/tutorial003.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/header_params/tutorial003_an.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/header_params/tutorial003_an_py310.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/header_params/tutorial003_an_py39.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/header_params/tutorial003_py310.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/header_params/tutorial003_py39.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/metadata/tutorial001.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/metadata/tutorial002.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/metadata/tutorial003.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/metadata/tutorial004.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/middleware/tutorial001.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/nosql_databases/tutorial001.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/openapi_callbacks/tutorial001.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_operation_advanced_configuration/tutorial001.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_operation_advanced_configuration/tutorial002.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_operation_advanced_configuration/tutorial003.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_operation_advanced_configuration/tutorial004.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_operation_advanced_configuration/tutorial005.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_operation_advanced_configuration/tutorial006.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_operation_advanced_configuration/tutorial007.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_operation_configuration/tutorial001.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_operation_configuration/tutorial001_py310.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_operation_configuration/tutorial001_py39.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_operation_configuration/tutorial002.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_operation_configuration/tutorial002_py310.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_operation_configuration/tutorial002_py39.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_operation_configuration/tutorial002b.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_operation_configuration/tutorial003.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_operation_configuration/tutorial003_py310.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_operation_configuration/tutorial003_py39.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_operation_configuration/tutorial004.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_operation_configuration/tutorial004_py310.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_operation_configuration/tutorial004_py39.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_operation_configuration/tutorial005.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_operation_configuration/tutorial005_py310.py
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_operation_configuration/tutorial005_py39.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_operation_configuration/tutorial006.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_params/tutorial001.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_params/tutorial002.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_params/tutorial003.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_params/tutorial003b.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_params/tutorial004.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_params/tutorial005.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_params_numeric_validations/tutorial001.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_params_numeric_validations/tutorial001_an.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_params_numeric_validations/tutorial001_an_py310.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_params_numeric_validations/tutorial001_an_py39.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_params_numeric_validations/tutorial001_py310.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_params_numeric_validations/tutorial002.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_params_numeric_validations/tutorial002_an.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_params_numeric_validations/tutorial002_an_py39.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_params_numeric_validations/tutorial003.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_params_numeric_validations/tutorial003_an.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_params_numeric_validations/tutorial003_an_py39.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_params_numeric_validations/tutorial004.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_params_numeric_validations/tutorial004_an.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_params_numeric_validations/tutorial004_an_py39.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_params_numeric_validations/tutorial005.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_params_numeric_validations/tutorial005_an.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_params_numeric_validations/tutorial005_an_py39.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_params_numeric_validations/tutorial006.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_params_numeric_validations/tutorial006_an.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/path_params_numeric_validations/tutorial006_an_py39.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/python_types/tutorial001.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/python_types/tutorial002.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/python_types/tutorial003.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/python_types/tutorial004.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/python_types/tutorial005.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/python_types/tutorial006.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/python_types/tutorial006_py39.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/python_types/tutorial007.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/python_types/tutorial007_py39.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/python_types/tutorial008.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/python_types/tutorial008_py39.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/python_types/tutorial008b.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/python_types/tutorial008b_py310.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/python_types/tutorial009.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/python_types/tutorial009_py310.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/python_types/tutorial009b.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/python_types/tutorial009c.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/python_types/tutorial009c_py310.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/python_types/tutorial010.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/python_types/tutorial011.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/python_types/tutorial011_py310.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/python_types/tutorial011_py39.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/python_types/tutorial012.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/python_types/tutorial013.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/python_types/tutorial013_py39.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params/tutorial001.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params/tutorial002.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params/tutorial002_py310.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params/tutorial003.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params/tutorial003_py310.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params/tutorial004.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params/tutorial004_py310.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params/tutorial005.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params/tutorial006.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params/tutorial006_py310.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params/tutorial006b.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial001.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial001_py310.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial002.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial002_an.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial002_an_py310.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial002_py310.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial003.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial003_an.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial003_an_py310.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial003_an_py39.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial003_py310.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial004.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial004_an.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial004_an_py310.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial004_an_py39.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial004_py310.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial005.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial005_an.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial005_an_py39.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial006.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial006_an.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial006_an_py39.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial006b.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial006b_an.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial006b_an_py39.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial006c.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial006c_an.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial006c_an_py310.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial006c_an_py39.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial006c_py310.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial006d.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial006d_an.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial006d_an_py39.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial007.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial007_an.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial007_an_py310.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial007_an_py39.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial007_py310.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial008.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial008_an.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial008_an_py310.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial008_an_py39.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial008_py310.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial009.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial009_an.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial009_an_py310.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial009_an_py39.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial009_py310.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial010.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial010_an.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial010_an_py310.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial010_an_py39.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial010_py310.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial011.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial011_an.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial011_an_py310.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial011_an_py39.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial011_py310.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial011_py39.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial012.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial012_an.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial012_an_py39.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial012_py39.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial013.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial013_an.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial013_an_py39.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial014.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial014_an.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial014_an_py310.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial014_an_py39.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/query_params_str_validations/tutorial014_py310.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/request_files/tutorial001.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/request_files/tutorial001_02.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/request_files/tutorial001_02_an.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/request_files/tutorial001_02_an_py310.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/request_files/tutorial001_02_an_py39.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/request_files/tutorial001_02_py310.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/request_files/tutorial001_03.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/request_files/tutorial001_03_an.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/request_files/tutorial001_03_an_py39.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/request_files/tutorial001_an.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/request_files/tutorial001_an_py39.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/request_files/tutorial002.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/request_files/tutorial002_an.py
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/request_files/tutorial002_an_py39.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/request_files/tutorial002_py39.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/request_files/tutorial003.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/request_files/tutorial003_an.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/request_files/tutorial003_an_py39.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/request_files/tutorial003_py39.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/request_forms/tutorial001.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/request_forms/tutorial001_an.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/request_forms/tutorial001_an_py39.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/request_forms_and_files/tutorial001.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/request_forms_and_files/tutorial001_an.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/request_forms_and_files/tutorial001_an_py39.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/response_change_status_code/tutorial001.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/response_cookies/tutorial001.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/response_cookies/tutorial002.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/response_directly/tutorial001.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/response_directly/tutorial002.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/response_headers/tutorial001.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/response_headers/tutorial002.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/response_model/tutorial001.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/response_model/tutorial001_01.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/response_model/tutorial001_01_py310.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/response_model/tutorial001_01_py39.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/response_model/tutorial001_py310.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/response_model/tutorial001_py39.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/response_model/tutorial002.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/response_model/tutorial002_py310.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/response_model/tutorial003.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/response_model/tutorial003_01.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/response_model/tutorial003_01_py310.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/response_model/tutorial003_02.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/response_model/tutorial003_03.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/response_model/tutorial003_04.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/response_model/tutorial003_04_py310.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/response_model/tutorial003_05.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/response_model/tutorial003_05_py310.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/response_model/tutorial003_py310.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/response_model/tutorial004.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/response_model/tutorial004_py310.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/response_model/tutorial004_py39.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/response_model/tutorial005.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/response_model/tutorial005_py310.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/response_model/tutorial006.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/response_model/tutorial006_py310.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/response_status_code/tutorial001.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/response_status_code/tutorial002.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/schema_extra_example/tutorial001.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/schema_extra_example/tutorial001_py310.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/schema_extra_example/tutorial002.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/schema_extra_example/tutorial002_py310.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/schema_extra_example/tutorial003.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/schema_extra_example/tutorial003_an.py
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/schema_extra_example/tutorial003_an_py310.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/schema_extra_example/tutorial003_an_py39.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/schema_extra_example/tutorial003_py310.py
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/schema_extra_example/tutorial004.py
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/schema_extra_example/tutorial004_an.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/schema_extra_example/tutorial004_an_py310.py
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/schema_extra_example/tutorial004_an_py39.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/schema_extra_example/tutorial004_py310.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/security/tutorial001.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/security/tutorial001_an.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/security/tutorial001_an_py39.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/security/tutorial002.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/security/tutorial002_an.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/security/tutorial002_an_py310.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/security/tutorial002_an_py39.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/security/tutorial002_py310.py
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/security/tutorial003.py
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/security/tutorial003_an.py
--rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/security/tutorial003_an_py310.py
--rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/security/tutorial003_an_py39.py
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/security/tutorial003_py310.py
--rw-r--r--   0        0        0     4113 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/security/tutorial004.py
--rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/security/tutorial004_an.py
--rw-r--r--   0        0        0     4161 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/security/tutorial004_an_py310.py
--rw-r--r--   0        0        0     4198 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/security/tutorial004_an_py39.py
--rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/security/tutorial004_py310.py
--rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/security/tutorial005.py
--rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/security/tutorial005_an.py
--rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/security/tutorial005_an_py310.py
--rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/security/tutorial005_an_py39.py
--rw-r--r--   0        0        0     5186 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/security/tutorial005_py310.py
--rw-r--r--   0        0        0     5241 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/security/tutorial005_py39.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/security/tutorial006.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/security/tutorial006_an.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/security/tutorial006_an_py39.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/security/tutorial007.py
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/security/tutorial007_an.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/security/tutorial007_an_py39.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/settings/tutorial001.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/settings/app01/__init__.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/settings/app01/config.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/settings/app01/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/settings/app02/__init__.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/settings/app02/config.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/settings/app02/main.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/settings/app02/test_main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/settings/app02_an/__init__.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/settings/app02_an/config.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/settings/app02_an/main.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/settings/app02_an/test_main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/settings/app02_an_py39/__init__.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/settings/app02_an_py39/config.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/settings/app02_an_py39/main.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/settings/app02_an_py39/test_main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/settings/app03/__init__.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/settings/app03/config.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/settings/app03/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/settings/app03_an/__init__.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/settings/app03_an/config.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/settings/app03_an/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/settings/app03_an_py39/__init__.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/settings/app03_an_py39/config.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/settings/app03_an_py39/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/sql_databases/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/sql_databases/sql_app/__init__.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/sql_databases/sql_app/alt_main.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/sql_databases/sql_app/crud.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/sql_databases/sql_app/database.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/sql_databases/sql_app/main.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/sql_databases/sql_app/models.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/sql_databases/sql_app/schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/sql_databases/sql_app/tests/__init__.py
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/sql_databases/sql_app/tests/test_sql_app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/sql_databases/sql_app_py310/__init__.py
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/sql_databases/sql_app_py310/alt_main.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/sql_databases/sql_app_py310/crud.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/sql_databases/sql_app_py310/database.py
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/sql_databases/sql_app_py310/main.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/sql_databases/sql_app_py310/models.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/sql_databases/sql_app_py310/schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/sql_databases/sql_app_py310/tests/__init__.py
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/sql_databases/sql_app_py310/tests/test_sql_app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/sql_databases/sql_app_py39/__init__.py
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/sql_databases/sql_app_py39/alt_main.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/sql_databases/sql_app_py39/crud.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/sql_databases/sql_app_py39/database.py
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/sql_databases/sql_app_py39/main.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/sql_databases/sql_app_py39/models.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/sql_databases/sql_app_py39/schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/sql_databases/sql_app_py39/tests/__init__.py
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/sql_databases/sql_app_py39/tests/test_sql_app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/sql_databases_peewee/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/sql_databases_peewee/sql_app/__init__.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/sql_databases_peewee/sql_app/crud.py
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/sql_databases_peewee/sql_app/database.py
--rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/sql_databases_peewee/sql_app/main.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/sql_databases_peewee/sql_app/models.py
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/sql_databases_peewee/sql_app/schemas.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/static_files/tutorial001.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/sub_applications/tutorial001.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/templates/tutorial001.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/templates/static/styles.css
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/templates/templates/item.html
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/using_request_directly/tutorial001.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/websockets/__init__.py
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/websockets/tutorial001.py
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/websockets/tutorial002.py
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/websockets/tutorial002_an.py
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/websockets/tutorial002_an_py310.py
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/websockets/tutorial002_an_py39.py
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/websockets/tutorial002_py310.py
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/websockets/tutorial003.py
--rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/websockets/tutorial003_py39.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 fastapi-0.96.1/docs_src/wsgi/tutorial001.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/__init__.py
--rw-r--r--   0        0        0    39525 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/applications.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/background.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/concurrency.py
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/datastructures.py
--rw-r--r--   0        0        0     5962 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/encoders.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/exception_handlers.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/exceptions.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/logger.py
--rw-r--r--   0        0        0     7515 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/param_functions.py
--rw-r--r--   0        0        0    10699 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/params.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/py.typed
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/requests.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/responses.py
--rw-r--r--   0        0        0    55563 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/routing.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/staticfiles.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/templating.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/testclient.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/types.py
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/utils.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/websockets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/dependencies/__init__.py
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/dependencies/models.py
--rw-r--r--   0        0        0    30908 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/dependencies/utils.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/middleware/__init__.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/middleware/asyncexitstack.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/middleware/cors.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/middleware/gzip.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/middleware/httpsredirect.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/middleware/trustedhost.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/middleware/wsgi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/openapi/__init__.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/openapi/constants.py
--rw-r--r--   0        0        0     6532 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/openapi/docs.py
--rw-r--r--   0        0        0    11021 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/openapi/models.py
--rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/openapi/utils.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/security/__init__.py
--rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/security/api_key.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/security/base.py
--rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/security/http.py
--rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/security/oauth2.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/security/open_id_connect_url.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 fastapi-0.96.1/fastapi/security/utils.py
--rwxr-xr-x   0        0        0       71 2020-02-02 00:00:00.000000 fastapi-0.96.1/scripts/build-docs.sh
--rwxr-xr-x   0        0        0       98 2020-02-02 00:00:00.000000 fastapi-0.96.1/scripts/clean.sh
--rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 fastapi-0.96.1/scripts/docs-live.sh
--rw-r--r--   0        0        0    15500 2020-02-02 00:00:00.000000 fastapi-0.96.1/scripts/docs.py
--rwxr-xr-x   0        0        0      137 2020-02-02 00:00:00.000000 fastapi-0.96.1/scripts/format.sh
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 fastapi-0.96.1/scripts/gitter_releases_bot.py
--rwxr-xr-x   0        0        0      163 2020-02-02 00:00:00.000000 fastapi-0.96.1/scripts/lint.sh
--rwxr-xr-x   0        0        0      337 2020-02-02 00:00:00.000000 fastapi-0.96.1/scripts/netlify-docs.sh
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 fastapi-0.96.1/scripts/notify.sh
--rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 fastapi-0.96.1/scripts/publish.sh
--rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 fastapi-0.96.1/scripts/test-cov-html.sh
--rwxr-xr-x   0        0        0      170 2020-02-02 00:00:00.000000 fastapi-0.96.1/scripts/test.sh
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 fastapi-0.96.1/scripts/zip-docs.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/__init__.py
--rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/main.py
--rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_additional_properties.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_additional_response_extra.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_additional_responses_bad.py
--rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_additional_responses_custom_model_in_callback.py
--rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_additional_responses_custom_validationerror.py
--rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_additional_responses_default_validationerror.py
--rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_additional_responses_response_class.py
--rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_additional_responses_router.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_ambiguous_params.py
--rw-r--r--   0        0        0     9779 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_annotated.py
--rw-r--r--   0        0        0    49052 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_application.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_callable_endpoint.py
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_custom_middleware_exception.py
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_custom_route_class.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_custom_schema_fields.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_custom_swagger_ui_redirect.py
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_datastructures.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_datetime_custom_encoder.py
--rw-r--r--   0        0        0     5365 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_default_response_class.py
--rw-r--r--   0        0        0     5117 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_default_response_class_router.py
--rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_dependency_cache.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_dependency_class.py
--rw-r--r--   0        0        0    11269 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_dependency_contextmanager.py
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_dependency_contextvars.py
--rw-r--r--   0        0        0     8164 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_dependency_duplicates.py
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_dependency_normal_exceptions.py
--rw-r--r--   0        0        0     9010 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_dependency_overrides.py
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_dependency_security_overrides.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_deprecated_openapi_prefix.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_duplicate_models_openapi.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_empty_router.py
--rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_enforce_once_required_parameter.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_exception_handlers.py
--rw-r--r--   0        0        0    13670 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_extra_routes.py
--rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_filter_pydantic_sub_model.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_forms_from_non_typing_sequences.py
--rw-r--r--   0        0        0    68172 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_generate_unique_id_function.py
--rw-r--r--   0        0        0     3744 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_get_request_body.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_http_connection_injection.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_include_route.py
--rw-r--r--   0        0        0   367192 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_include_router_defaults_overrides.py
--rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_infer_param_optionality.py
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_inherited_custom_class.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_invalid_path_param.py
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_invalid_sequence_param.py
--rw-r--r--   0        0        0     6861 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_jsonable_encoder.py
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_local_docs.py
--rw-r--r--   0        0        0     5391 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_multi_body_errors.py
--rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_multi_query_errors.py
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_multipart_installation.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_no_swagger_ui_redirect.py
--rw-r--r--   0        0        0     4311 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_openapi_query_parameter_extension.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_openapi_route_extensions.py
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_openapi_servers.py
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_operations_signatures.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_orjson_response_class.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_param_class.py
--rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_param_in_path_and_dependency.py
--rw-r--r--   0        0        0     7606 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_param_include_in_schema.py
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_params_repr.py
--rw-r--r--   0        0        0     7774 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_path.py
--rw-r--r--   0        0        0     3362 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_put_no_body.py
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_query.py
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_read_with_orm_mode.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_repeated_cookie_headers.py
--rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_repeated_dependency_schema.py
--rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_repeated_parameter_alias.py
--rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_reponse_set_reponse_code_empty.py
--rw-r--r--   0        0        0     6546 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_request_body_parameters_media_type.py
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_required_noneable.py
--rw-r--r--   0        0        0    10951 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_response_by_alias.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_response_change_status_code.py
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_response_class_no_mediatype.py
--rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_response_code_no_body.py
--rw-r--r--   0        0        0    48457 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_response_model_as_return_annotation.py
--rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_response_model_include_exclude.py
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_response_model_invalid.py
--rw-r--r--   0        0        0     5379 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_response_model_sub_types.py
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_route_scope.py
--rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_router_events.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_router_prefix_with_template.py
--rw-r--r--   0        0        0    33384 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_schema_extra_examples.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_security_api_key_cookie.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_security_api_key_cookie_description.py
--rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_security_api_key_cookie_optional.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_security_api_key_header.py
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_security_api_key_header_description.py
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_security_api_key_header_optional.py
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_security_api_key_query.py
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_security_api_key_query_description.py
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_security_api_key_query_optional.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_security_http_base.py
--rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_security_http_base_description.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_security_http_base_optional.py
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_security_http_basic_optional.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_security_http_basic_realm.py
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_security_http_basic_realm_description.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_security_http_bearer.py
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_security_http_bearer_description.py
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_security_http_bearer_optional.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_security_http_digest.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_security_http_digest_description.py
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_security_http_digest_optional.py
--rw-r--r--   0        0        0     8340 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_security_oauth2.py
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_security_oauth2_authorization_code_bearer.py
--rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_security_oauth2_authorization_code_bearer_description.py
--rw-r--r--   0        0        0     8387 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_security_oauth2_optional.py
--rw-r--r--   0        0        0     8490 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_security_oauth2_optional_description.py
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_security_oauth2_password_bearer_optional.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_security_oauth2_password_bearer_optional_description.py
--rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_security_openid_connect.py
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_security_openid_connect_description.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_security_openid_connect_optional.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_serialize_response.py
--rw-r--r--   0        0        0     4998 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_serialize_response_dataclass.py
--rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_serialize_response_model.py
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_skip_defaults.py
--rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_starlette_exception.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_starlette_urlconvertors.py
--rw-r--r--   0        0        0    12779 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_sub_callbacks.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_swagger_ui_init_oauth.py
--rw-r--r--   0        0        0     9847 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tuples.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_typing_python39.py
--rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_union_body.py
--rw-r--r--   0        0        0     4465 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_union_inherited_body.py
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_validate_response.py
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_validate_response_dataclass.py
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_validate_response_recursive.py
--rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_ws_router.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_modules_same_name_body/__init__.py
--rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_modules_same_name_body/test_main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_modules_same_name_body/app/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_modules_same_name_body/app/a.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_modules_same_name_body/app/b.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_modules_same_name_body/app/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_additional_responses/__init__.py
--rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_additional_responses/test_tutorial001.py
--rw-r--r--   0        0        0     4288 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_additional_responses/test_tutorial002.py
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_additional_responses/test_tutorial003.py
--rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_additional_responses/test_tutorial004.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_additional_status_codes/__init__.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_additional_status_codes/test_tutorial001.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_py310.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_advanced_middleware/__init__.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_advanced_middleware/test_tutorial001.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_advanced_middleware/test_tutorial002.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_advanced_middleware/test_tutorial003.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_async_sql_databases/__init__.py
--rw-r--r--   0        0        0     5833 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_async_sql_databases/test_tutorial001.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_async_tests/__init__.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_async_tests/test_main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_background_tasks/__init__.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_background_tasks/test_tutorial001.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_background_tasks/test_tutorial002.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_background_tasks/test_tutorial002_an.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py310.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py39.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_background_tasks/test_tutorial002_py310.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_behind_a_proxy/__init__.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_behind_a_proxy/test_tutorial001.py
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_behind_a_proxy/test_tutorial002.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_behind_a_proxy/test_tutorial003.py
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_behind_a_proxy/test_tutorial004.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_bigger_applications/__init__.py
--rw-r--r--   0        0        0    18714 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_bigger_applications/test_main.py
--rw-r--r--   0        0        0    18717 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_bigger_applications/test_main_an.py
--rw-r--r--   0        0        0    19078 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_bigger_applications/test_main_an_py39.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_body/__init__.py
--rw-r--r--   0        0        0     8723 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_body/test_tutorial001.py
--rw-r--r--   0        0        0     9101 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_body/test_tutorial001_py310.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_body_fields/__init__.py
--rw-r--r--   0        0        0     5961 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_body_fields/test_tutorial001.py
--rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_body_fields/test_tutorial001_an.py
--rw-r--r--   0        0        0     6144 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_body_fields/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_body_fields/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_body_fields/test_tutorial001_py310.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_body_multiple_params/__init__.py
--rw-r--r--   0        0        0     5239 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_body_multiple_params/test_tutorial001.py
--rw-r--r--   0        0        0     5242 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an.py
--rw-r--r--   0        0        0     5422 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     5418 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     5419 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_py310.py
--rw-r--r--   0        0        0     7217 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_body_multiple_params/test_tutorial003.py
--rw-r--r--   0        0        0     7220 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an.py
--rw-r--r--   0        0        0     7400 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py310.py
--rw-r--r--   0        0        0     7396 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py39.py
--rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_py310.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_body_nested_models/__init__.py
--rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_body_nested_models/test_tutorial009.py
--rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_body_nested_models/test_tutorial009_py39.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_body_updates/__init__.py
--rw-r--r--   0        0        0     6030 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_body_updates/test_tutorial001.py
--rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_body_updates/test_tutorial001_py310.py
--rw-r--r--   0        0        0     6248 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_body_updates/test_tutorial001_py39.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_conditional_openapi/__init__.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_conditional_openapi/test_tutorial001.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_cookie_params/__init__.py
--rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_cookie_params/test_tutorial001.py
--rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_cookie_params/test_tutorial001_an.py
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_cookie_params/test_tutorial001_py310.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_cors/__init__.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_cors/test_tutorial001.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_custom_request_and_route/__init__.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_custom_request_and_route/test_tutorial001.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_custom_request_and_route/test_tutorial002.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_custom_request_and_route/test_tutorial003.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_custom_response/__init__.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_custom_response/test_tutorial001.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_custom_response/test_tutorial001b.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_custom_response/test_tutorial004.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_custom_response/test_tutorial005.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_custom_response/test_tutorial006.py
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_custom_response/test_tutorial006b.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_custom_response/test_tutorial006c.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_custom_response/test_tutorial007.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_custom_response/test_tutorial008.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_custom_response/test_tutorial009.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_custom_response/test_tutorial009b.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_custom_response/test_tutorial009c.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_dataclasses/__init__.py
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_dataclasses/test_tutorial001.py
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_dataclasses/test_tutorial002.py
--rw-r--r--   0        0        0     6783 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_dataclasses/test_tutorial003.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_dependencies/__init__.py
--rw-r--r--   0        0        0     6353 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_dependencies/test_tutorial001.py
--rw-r--r--   0        0        0     6356 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_dependencies/test_tutorial001_an.py
--rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_dependencies/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     6532 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_dependencies/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     6533 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_dependencies/test_tutorial001_py310.py
--rw-r--r--   0        0        0     5102 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_dependencies/test_tutorial004.py
--rw-r--r--   0        0        0     5105 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_dependencies/test_tutorial004_an.py
--rw-r--r--   0        0        0     5285 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_dependencies/test_tutorial004_an_py310.py
--rw-r--r--   0        0        0     5281 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_dependencies/test_tutorial004_an_py39.py
--rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_dependencies/test_tutorial004_py310.py
--rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_dependencies/test_tutorial006.py
--rw-r--r--   0        0        0     4480 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_dependencies/test_tutorial006_an.py
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_dependencies/test_tutorial006_an_py39.py
--rw-r--r--   0        0        0     7386 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_dependencies/test_tutorial012.py
--rw-r--r--   0        0        0     7389 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_dependencies/test_tutorial012_an.py
--rw-r--r--   0        0        0     7787 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_dependencies/test_tutorial012_an_py39.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_events/__init__.py
--rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_events/test_tutorial001.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_events/test_tutorial002.py
--rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_events/test_tutorial003.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_extending_openapi/__init__.py
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_extending_openapi/test_tutorial001.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_extending_openapi/test_tutorial002.py
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_extending_openapi/test_tutorial003.py
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_extending_openapi/test_tutorial004.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_extending_openapi/test_tutorial005.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_extra_data_types/__init__.py
--rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_extra_data_types/test_tutorial001.py
--rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_extra_data_types/test_tutorial001_an.py
--rw-r--r--   0        0        0     5368 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     5364 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     5365 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_extra_data_types/test_tutorial001_py310.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_extra_models/__init__.py
--rw-r--r--   0        0        0     4808 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_extra_models/test_tutorial003.py
--rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_extra_models/test_tutorial003_py310.py
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_extra_models/test_tutorial004.py
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_extra_models/test_tutorial004_py39.py
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_extra_models/test_tutorial005.py
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_extra_models/test_tutorial005_py39.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_first_steps/__init__.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_first_steps/test_tutorial001.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_generate_clients/__init__.py
--rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_generate_clients/test_tutorial003.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_handling_errors/__init__.py
--rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_handling_errors/test_tutorial001.py
--rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_handling_errors/test_tutorial002.py
--rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_handling_errors/test_tutorial003.py
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_handling_errors/test_tutorial004.py
--rw-r--r--   0        0        0     3899 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_handling_errors/test_tutorial005.py
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_handling_errors/test_tutorial006.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_header_params/__init__.py
--rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_header_params/test_tutorial001.py
--rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_header_params/test_tutorial001_an.py
--rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_header_params/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_header_params/test_tutorial001_py310.py
--rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_header_params/test_tutorial002.py
--rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_header_params/test_tutorial002_an.py
--rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_header_params/test_tutorial002_an_py310.py
--rw-r--r--   0        0        0     3887 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_header_params/test_tutorial002_an_py39.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_header_params/test_tutorial002_py310.py
--rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_header_params/test_tutorial003.py
--rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_header_params/test_tutorial003_an.py
--rw-r--r--   0        0        0     3824 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_header_params/test_tutorial003_an_py310.py
--rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_header_params/test_tutorial003_an_py39.py
--rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_header_params/test_tutorial003_py310.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_metadata/__init__.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_metadata/test_tutorial001.py
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_metadata/test_tutorial004.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_openapi_callbacks/__init__.py
--rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_openapi_callbacks/test_tutorial001.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_path_operation_advanced_configurations/__init__.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial001.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial002.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial003.py
--rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial004.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial005.py
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial006.py
--rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial007.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_path_operation_configurations/__init__.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_path_operation_configurations/test_tutorial002b.py
--rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_path_operation_configurations/test_tutorial005.py
--rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py310.py
--rw-r--r--   0        0        0     4682 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py39.py
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_path_operation_configurations/test_tutorial006.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_path_params/__init__.py
--rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_path_params/test_tutorial004.py
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_path_params/test_tutorial005.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_query_params/__init__.py
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_query_params/test_tutorial005.py
--rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_query_params/test_tutorial006.py
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_query_params/test_tutorial006_py310.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/__init__.py
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010.py
--rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an.py
--rw-r--r--   0        0        0     4691 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py310.py
--rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py39.py
--rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_py310.py
--rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011.py
--rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an.py
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py310.py
--rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py39.py
--rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py310.py
--rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py39.py
--rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012.py
--rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an.py
--rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an_py39.py
--rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_py39.py
--rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial013.py
--rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an.py
--rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an_py39.py
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014.py
--rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an.py
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py310.py
--rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py39.py
--rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_py310.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_request_files/__init__.py
--rw-r--r--   0        0        0     6732 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_request_files/test_tutorial001.py
--rw-r--r--   0        0        0     5984 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_request_files/test_tutorial001_02.py
--rw-r--r--   0        0        0     5987 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_request_files/test_tutorial001_02_an.py
--rw-r--r--   0        0        0     6256 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py310.py
--rw-r--r--   0        0        0     6249 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py39.py
--rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_request_files/test_tutorial001_02_py310.py
--rw-r--r--   0        0        0     6133 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_request_files/test_tutorial001_03.py
--rw-r--r--   0        0        0     6136 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_request_files/test_tutorial001_03_an.py
--rw-r--r--   0        0        0     6300 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_request_files/test_tutorial001_03_an_py39.py
--rw-r--r--   0        0        0     6735 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_request_files/test_tutorial001_an.py
--rw-r--r--   0        0        0     6962 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_request_files/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     7703 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_request_files/test_tutorial002.py
--rw-r--r--   0        0        0     7706 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_request_files/test_tutorial002_an.py
--rw-r--r--   0        0        0     8100 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_request_files/test_tutorial002_an_py39.py
--rw-r--r--   0        0        0     8097 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_request_files/test_tutorial002_py39.py
--rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_request_files/test_tutorial003.py
--rw-r--r--   0        0        0     7314 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_request_files/test_tutorial003_an.py
--rw-r--r--   0        0        0     7830 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_request_files/test_tutorial003_an_py39.py
--rw-r--r--   0        0        0     7827 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_request_files/test_tutorial003_py39.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_request_forms/__init__.py
--rw-r--r--   0        0        0     5013 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_request_forms/test_tutorial001.py
--rw-r--r--   0        0        0     5016 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_request_forms/test_tutorial001_an.py
--rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_request_forms/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_request_forms_and_files/__init__.py
--rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_request_forms_and_files/test_tutorial001.py
--rw-r--r--   0        0        0     6418 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an.py
--rw-r--r--   0        0        0     6818 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_response_change_status_code/__init__.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_response_change_status_code/test_tutorial001.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_response_cookies/__init__.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_response_cookies/test_tutorial001.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_response_cookies/test_tutorial002.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_response_headers/__init__.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_response_headers/test_tutorial001.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_response_headers/test_tutorial002.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_response_model/__init__.py
--rw-r--r--   0        0        0     4761 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_response_model/test_tutorial003.py
--rw-r--r--   0        0        0     4767 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_response_model/test_tutorial003_01.py
--rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_response_model/test_tutorial003_01_py310.py
--rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_response_model/test_tutorial003_02.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_response_model/test_tutorial003_03.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_response_model/test_tutorial003_04.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_response_model/test_tutorial003_04_py310.py
--rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_response_model/test_tutorial003_05.py
--rw-r--r--   0        0        0     3699 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_response_model/test_tutorial003_05_py310.py
--rw-r--r--   0        0        0     4953 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_response_model/test_tutorial003_py310.py
--rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_response_model/test_tutorial004.py
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_response_model/test_tutorial004_py310.py
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_response_model/test_tutorial004_py39.py
--rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_response_model/test_tutorial005.py
--rw-r--r--   0        0        0     5756 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_response_model/test_tutorial005_py310.py
--rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_response_model/test_tutorial006.py
--rw-r--r--   0        0        0     5756 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_response_model/test_tutorial006_py310.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_schema_extra_example/__init__.py
--rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_schema_extra_example/test_tutorial004.py
--rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an.py
--rw-r--r--   0        0        0     5754 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py310.py
--rw-r--r--   0        0        0     5750 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py39.py
--rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_py310.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_security/__init__.py
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_security/test_tutorial001.py
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_security/test_tutorial001_an.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_security/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     6832 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_security/test_tutorial003.py
--rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_security/test_tutorial003_an.py
--rw-r--r--   0        0        0     7244 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_security/test_tutorial003_an_py310.py
--rw-r--r--   0        0        0     7233 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_security/test_tutorial003_an_py39.py
--rw-r--r--   0        0        0     7241 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_security/test_tutorial003_py310.py
--rw-r--r--   0        0        0    13084 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_security/test_tutorial005.py
--rw-r--r--   0        0        0    13087 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_security/test_tutorial005_an.py
--rw-r--r--   0        0        0    13992 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_security/test_tutorial005_an_py310.py
--rw-r--r--   0        0        0    13968 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_security/test_tutorial005_an_py39.py
--rw-r--r--   0        0        0    13980 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_security/test_tutorial005_py310.py
--rw-r--r--   0        0        0    13956 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_security/test_tutorial005_py39.py
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_security/test_tutorial006.py
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_security/test_tutorial006_an.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_security/test_tutorial006_an_py39.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_settings/__init__.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_settings/test_app02.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_sql_databases/__init__.py
--rw-r--r--   0        0        0    15205 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_sql_databases/test_sql_databases.py
--rw-r--r--   0        0        0    15384 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware.py
--rw-r--r--   0        0        0    15675 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py310.py
--rw-r--r--   0        0        0    15666 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py39.py
--rw-r--r--   0        0        0    15681 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_sql_databases/test_sql_databases_py310.py
--rw-r--r--   0        0        0    15672 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_sql_databases/test_sql_databases_py39.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_sql_databases/test_testing_databases.py
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_sql_databases/test_testing_databases_py310.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_sql_databases/test_testing_databases_py39.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_sql_databases_peewee/__init__.py
--rw-r--r--   0        0        0    17654 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_sql_databases_peewee/test_sql_databases_peewee.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_sub_applications/__init__.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_sub_applications/test_tutorial001.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_templates/__init__.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_templates/test_tutorial001.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_testing/__init__.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_testing/test_main.py
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_testing/test_main_b.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_testing/test_main_b_an.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_testing/test_main_b_an_py310.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_testing/test_main_b_an_py39.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_testing/test_main_b_py310.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_testing/test_tutorial001.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_testing/test_tutorial002.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_testing/test_tutorial003.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_testing_dependencies/__init__.py
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_testing_dependencies/test_tutorial001.py
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an.py
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_py310.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_websockets/__init__.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_websockets/test_tutorial001.py
--rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_websockets/test_tutorial002.py
--rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_websockets/test_tutorial002_an.py
--rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_websockets/test_tutorial002_an_py310.py
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_websockets/test_tutorial002_an_py39.py
--rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_websockets/test_tutorial002_py310.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_websockets/test_tutorial003.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_websockets/test_tutorial003_py39.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_wsgi/__init__.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 fastapi-0.96.1/tests/test_tutorial/test_wsgi/test_tutorial001.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 fastapi-0.96.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 fastapi-0.96.1/LICENSE
--rw-r--r--   0        0        0    20788 2020-02-02 00:00:00.000000 fastapi-0.96.1/README.md
--rw-r--r--   0        0        0     6330 2020-02-02 00:00:00.000000 fastapi-0.96.1/pyproject.toml
--rw-r--r--   0        0        0    24958 2020-02-02 00:00:00.000000 fastapi-0.96.1/PKG-INFO
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 fastapi-0.97.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fastapi-0.97.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 fastapi-0.97.0/SECURITY.md
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 fastapi-0.97.0/requirements-docs.txt
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 fastapi-0.97.0/requirements-tests.txt
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 fastapi-0.97.0/requirements.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 fastapi-0.97.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fastapi-0.97.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     5629 2020-02-02 00:00:00.000000 fastapi-0.97.0/.github/DISCUSSION_TEMPLATE/questions.yml
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 fastapi-0.97.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 fastapi-0.97.0/.github/ISSUE_TEMPLATE/privileged.yml
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 fastapi-0.97.0/.github/actions/comment-docs-preview-in-pr/Dockerfile
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 fastapi-0.97.0/.github/actions/comment-docs-preview-in-pr/action.yml
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 fastapi-0.97.0/.github/actions/comment-docs-preview-in-pr/app/main.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 fastapi-0.97.0/.github/actions/notify-translations/Dockerfile
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 fastapi-0.97.0/.github/actions/notify-translations/action.yml
+-rw-r--r--   0        0        0    12661 2020-02-02 00:00:00.000000 fastapi-0.97.0/.github/actions/notify-translations/app/main.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 fastapi-0.97.0/.github/actions/people/Dockerfile
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 fastapi-0.97.0/.github/actions/people/action.yml
+-rw-r--r--   0        0        0    19794 2020-02-02 00:00:00.000000 fastapi-0.97.0/.github/actions/people/app/main.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 fastapi-0.97.0/.github/actions/watch-previews/Dockerfile
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 fastapi-0.97.0/.github/actions/watch-previews/action.yml
+-rw-r--r--   0        0        0     3407 2020-02-02 00:00:00.000000 fastapi-0.97.0/.github/actions/watch-previews/app/main.py
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 fastapi-0.97.0/.github/workflows/build-docs.yml
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 fastapi-0.97.0/.github/workflows/issue-manager.yml
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fastapi-0.97.0/.github/workflows/label-approved.yml
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 fastapi-0.97.0/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 fastapi-0.97.0/.github/workflows/notify-translations.yml
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 fastapi-0.97.0/.github/workflows/people.yml
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 fastapi-0.97.0/.github/workflows/preview-docs.yml
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 fastapi-0.97.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 fastapi-0.97.0/.github/workflows/smokeshow.yml
+-rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 fastapi-0.97.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/missing-translation.md
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/az/mkdocs.yml
+-rw-r--r--   0        0        0    18627 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/az/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/az/overrides/.gitignore
+-rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/cs/mkdocs.yml
+-rw-r--r--   0        0        0    19467 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/cs/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/cs/overrides/.gitignore
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/de/mkdocs.yml
+-rw-r--r--   0        0        0    11231 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/de/docs/features.md
+-rw-r--r--   0        0        0    18492 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/de/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/de/overrides/.gitignore
+-rw-r--r--   0        0        0     6759 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/mkdocs.yml
+-rw-r--r--   0        0        0    19136 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/alternatives.md
+-rw-r--r--   0        0        0    19114 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/async.md
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/benchmarks.md
+-rw-r--r--   0        0        0    11702 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/contributing.md
+-rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/external-links.md
+-rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/fastapi-people.md
+-rw-r--r--   0        0        0     8409 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/features.md
+-rw-r--r--   0        0        0    12235 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/help-fastapi.md
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/history-design-future.md
+-rw-r--r--   0        0        0    17670 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/index.md
+-rw-r--r--   0        0        0     4978 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/project-generation.md
+-rw-r--r--   0        0        0    13966 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/python-types.md
+-rw-r--r--   0        0        0     8055 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/advanced/additional-responses.md
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/advanced/additional-status-codes.md
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/advanced/advanced-dependencies.md
+-rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/advanced/async-sql-databases.md
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/advanced/async-tests.md
+-rw-r--r--   0        0        0    10306 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/advanced/behind-a-proxy.md
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/advanced/conditional-openapi.md
+-rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/advanced/custom-request-and-route.md
+-rw-r--r--   0        0        0     9988 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/advanced/custom-response.md
+-rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/advanced/dataclasses.md
+-rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/advanced/events.md
+-rw-r--r--   0        0        0     9748 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/advanced/extending-openapi.md
+-rw-r--r--   0        0        0     8663 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/advanced/generate-clients.md
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/advanced/graphql.md
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/advanced/index.md
+-rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/advanced/middleware.md
+-rw-r--r--   0        0        0     4917 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/advanced/nosql-databases.md
+-rw-r--r--   0        0        0     6784 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/advanced/openapi-callbacks.md
+-rw-r--r--   0        0        0     5886 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/advanced/path-operation-advanced-configuration.md
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/advanced/response-change-status-code.md
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/advanced/response-cookies.md
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/advanced/response-directly.md
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/advanced/response-headers.md
+-rw-r--r--   0        0        0    11642 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/advanced/settings.md
+-rw-r--r--   0        0        0    19705 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/advanced/sql-databases-peewee.md
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/advanced/sub-applications.md
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/advanced/templates.md
+-rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/advanced/testing-database.md
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/advanced/testing-dependencies.md
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/advanced/testing-events.md
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/advanced/testing-websockets.md
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/advanced/using-request-directly.md
+-rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/advanced/websockets.md
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/advanced/wsgi.md
+-rw-r--r--   0        0        0     4160 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/advanced/security/http-basic-auth.md
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/advanced/security/index.md
+-rw-r--r--   0        0        0    11325 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/advanced/security/oauth2-scopes.md
+-rw-r--r--   0        0        0    14832 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/deployment/concepts.md
+-rw-r--r--   0        0        0     6087 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/deployment/deta.md
+-rw-r--r--   0        0        0    28740 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/deployment/docker.md
+-rw-r--r--   0        0        0     9658 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/deployment/https.md
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/deployment/index.md
+-rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/deployment/manually.md
+-rw-r--r--   0        0        0     8396 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/deployment/server-workers.md
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/deployment/versions.md
+-rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/background-tasks.md
+-rw-r--r--   0        0        0    15678 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/bigger-applications.md
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/body-fields.md
+-rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/body-multiple-params.md
+-rw-r--r--   0        0        0     9408 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/body-nested-models.md
+-rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/body-updates.md
+-rw-r--r--   0        0        0     6683 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/body.md
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/cookie-params.md
+-rw-r--r--   0        0        0     4170 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/cors.md
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/debugging.md
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/encoder.md
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/extra-data-types.md
+-rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/extra-models.md
+-rw-r--r--   0        0        0     8281 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/first-steps.md
+-rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/handling-errors.md
+-rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/header-params.md
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/index.md
+-rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/metadata.md
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/middleware.md
+-rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/path-operation-configuration.md
+-rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/path-params-numeric-validations.md
+-rw-r--r--   0        0        0     7878 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/path-params.md
+-rw-r--r--   0        0        0    12188 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/query-params-str-validations.md
+-rw-r--r--   0        0        0     4576 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/query-params.md
+-rw-r--r--   0        0        0     6803 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/request-files.md
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/request-forms-and-files.md
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/request-forms.md
+-rw-r--r--   0        0        0    16358 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/response-model.md
+-rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/response-status-code.md
+-rw-r--r--   0        0        0     5674 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/schema-extra-example.md
+-rw-r--r--   0        0        0    25882 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/sql-databases.md
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/static-files.md
+-rw-r--r--   0        0        0     5296 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/testing.md
+-rw-r--r--   0        0        0     6134 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/dependencies/classes-as-dependencies.md
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/dependencies/dependencies-in-path-operation-decorators.md
+-rw-r--r--   0        0        0     8941 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/dependencies/dependencies-with-yield.md
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/dependencies/global-dependencies.md
+-rw-r--r--   0        0        0     6888 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/dependencies/index.md
+-rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/dependencies/sub-dependencies.md
+-rw-r--r--   0        0        0     6946 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/security/first-steps.md
+-rw-r--r--   0        0        0     4474 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/security/get-current-user.md
+-rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/security/index.md
+-rw-r--r--   0        0        0     9718 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/security/oauth2-jwt.md
+-rw-r--r--   0        0        0     9107 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/docs/tutorial/security/simple-oauth2.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/em/overrides/.gitignore
+-rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/mkdocs.yml
+-rw-r--r--   0        0        0    18874 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/data/external_links.yml
+-rw-r--r--   0        0        0    25966 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/data/github_sponsors.yml
+-rw-r--r--   0        0        0    22157 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/data/people.yml
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/data/sponsors.yml
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/data/sponsors_badge.yml
+-rw-r--r--   0        0        0    23768 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/alternatives.md
+-rw-r--r--   0        0        0    23576 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/async.md
+-rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/benchmarks.md
+-rw-r--r--   0        0        0    14005 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/contributing.md
+-rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/external-links.md
+-rw-r--r--   0        0        0     6515 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/fastapi-people.md
+-rw-r--r--   0        0        0     9479 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/features.md
+-rw-r--r--   0        0        0    14258 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/help-fastapi.md
+-rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/history-design-future.md
+-rw-r--r--   0        0        0    19423 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/index.md
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/newsletter.md
+-rw-r--r--   0        0        0     5826 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/project-generation.md
+-rw-r--r--   0        0        0    17461 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/python-types.md
+-rw-r--r--   0        0        0   268398 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/release-notes.md
+-rw-r--r--   0        0        0     8996 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/advanced/additional-responses.md
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/advanced/additional-status-codes.md
+-rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/advanced/advanced-dependencies.md
+-rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/advanced/async-sql-databases.md
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/advanced/async-tests.md
+-rw-r--r--   0        0        0    11778 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/advanced/behind-a-proxy.md
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/advanced/conditional-openapi.md
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/advanced/custom-request-and-route.md
+-rw-r--r--   0        0        0    11981 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/advanced/custom-response.md
+-rw-r--r--   0        0        0     4248 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/advanced/dataclasses.md
+-rw-r--r--   0        0        0     7828 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/advanced/events.md
+-rw-r--r--   0        0        0    11429 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/advanced/extending-openapi.md
+-rw-r--r--   0        0        0     9756 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/advanced/generate-clients.md
+-rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/advanced/graphql.md
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/advanced/index.md
+-rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/advanced/middleware.md
+-rw-r--r--   0        0        0     5750 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/advanced/nosql-databases.md
+-rw-r--r--   0        0        0     7934 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/advanced/openapi-callbacks.md
+-rw-r--r--   0        0        0     7136 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/advanced/path-operation-advanced-configuration.md
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/advanced/response-change-status-code.md
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/advanced/response-cookies.md
+-rw-r--r--   0        0        0     3060 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/advanced/response-directly.md
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/advanced/response-headers.md
+-rw-r--r--   0        0        0    14584 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/advanced/settings.md
+-rw-r--r--   0        0        0    23622 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/advanced/sql-databases-peewee.md
+-rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/advanced/sub-applications.md
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/advanced/templates.md
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/advanced/testing-database.md
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/advanced/testing-dependencies.md
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/advanced/testing-events.md
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/advanced/testing-websockets.md
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/advanced/using-request-directly.md
+-rw-r--r--   0        0        0     6370 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/advanced/websockets.md
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/advanced/wsgi.md
+-rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/advanced/security/http-basic-auth.md
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/advanced/security/index.md
+-rw-r--r--   0        0        0    20945 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/advanced/security/oauth2-scopes.md
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/css/custom.css
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/css/termynal.css
+-rw-r--r--   0        0        0    18405 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/deployment/concepts.md
+-rw-r--r--   0        0        0    13815 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/deployment/deta.md
+-rw-r--r--   0        0        0    35157 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/deployment/docker.md
+-rw-r--r--   0        0        0    12240 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/deployment/https.md
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/deployment/index.md
+-rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/deployment/manually.md
+-rw-r--r--   0        0        0     9364 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/deployment/server-workers.md
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/deployment/versions.md
+-rwxr-xr-x   0        0        0      412 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/favicon.png
+-rw-r--r--   0        0        0    58136 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/github-social-preview.png
+-rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/github-social-preview.svg
+-rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/icon-transparent-bg.png
+-rw-r--r--   0        0        0     5210 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/icon-white-bg.png
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/icon-white.svg
+-rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/logo-teal-vector.svg
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/logo-teal.svg
+-rw-r--r--   0        0        0    51205 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/pycharm-completion.png
+-rw-r--r--   0        0        0    62417 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/vscode-completion.png
+-rw-r--r--   0        0        0   203390 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-01.png
+-rw-r--r--   0        0        0   166992 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-02.png
+-rw-r--r--   0        0        0   172943 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-03.png
+-rw-r--r--   0        0        0   163423 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-04.png
+-rw-r--r--   0        0        0   159869 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-05.png
+-rw-r--r--   0        0        0   164838 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-06.png
+-rw-r--r--   0        0        0   169968 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-07.png
+-rw-r--r--   0        0        0   225993 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/async/parallel-burgers/parallel-burgers-01.png
+-rw-r--r--   0        0        0   203644 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/async/parallel-burgers/parallel-burgers-02.png
+-rw-r--r--   0        0        0   168628 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/async/parallel-burgers/parallel-burgers-03.png
+-rw-r--r--   0        0        0   219429 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/async/parallel-burgers/parallel-burgers-04.png
+-rw-r--r--   0        0        0   185116 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/async/parallel-burgers/parallel-burgers-05.png
+-rw-r--r--   0        0        0   157113 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/async/parallel-burgers/parallel-burgers-06.png
+-rw-r--r--   0        0        0   124827 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/deployment/concepts/image01.png
+-rw-r--r--   0        0        0    10203 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/deployment/concepts/process-ram.drawio
+-rw-r--r--   0        0        0    16640 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/deployment/concepts/process-ram.svg
+-rw-r--r--   0        0        0    39996 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/deployment/deta/image01.png
+-rw-r--r--   0        0        0    48297 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/deployment/deta/image02.png
+-rw-r--r--   0        0        0    52704 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/deployment/deta/image03.png
+-rw-r--r--   0        0        0    49760 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/deployment/deta/image04.png
+-rw-r--r--   0        0        0    33130 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/deployment/deta/image05.png
+-rw-r--r--   0        0        0   105270 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/deployment/deta/image06.png
+-rw-r--r--   0        0        0    26363 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/deployment/https/https.drawio
+-rw-r--r--   0        0        0    40488 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/deployment/https/https.svg
+-rw-r--r--   0        0        0     6384 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/deployment/https/https01.drawio
+-rw-r--r--   0        0        0    10583 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/deployment/https/https01.svg
+-rw-r--r--   0        0        0     9636 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/deployment/https/https02.drawio
+-rw-r--r--   0        0        0    15794 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/deployment/https/https02.svg
+-rw-r--r--   0        0        0    12582 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/deployment/https/https03.drawio
+-rw-r--r--   0        0        0    21549 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/deployment/https/https03.svg
+-rw-r--r--   0        0        0    14291 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/deployment/https/https04.drawio
+-rw-r--r--   0        0        0    23265 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/deployment/https/https04.svg
+-rw-r--r--   0        0        0    15945 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/deployment/https/https05.drawio
+-rw-r--r--   0        0        0    26167 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/deployment/https/https05.svg
+-rw-r--r--   0        0        0    17470 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/deployment/https/https06.drawio
+-rw-r--r--   0        0        0    27919 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/deployment/https/https06.svg
+-rw-r--r--   0        0        0    19117 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/deployment/https/https07.drawio
+-rw-r--r--   0        0        0    29659 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/deployment/https/https07.svg
+-rw-r--r--   0        0        0    21427 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/deployment/https/https08.drawio
+-rw-r--r--   0        0        0    33876 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/deployment/https/https08.svg
+-rw-r--r--   0        0        0    74158 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/index/index-01-swagger-ui-simple.png
+-rw-r--r--   0        0        0    68468 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/index/index-02-redoc-simple.png
+-rw-r--r--   0        0        0    75099 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/index/index-03-swagger-02.png
+-rw-r--r--   0        0        0    67572 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/index/index-04-swagger-03.png
+-rw-r--r--   0        0        0    71441 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/index/index-05-swagger-04.png
+-rw-r--r--   0        0        0    78842 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/index/index-06-redoc-02.png
+-rw-r--r--   0        0        0     8036 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/logo-margin/logo-teal-vector.svg
+-rw-r--r--   0        0        0    17680 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/logo-margin/logo-teal.png
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/logo-margin/logo-teal.svg
+-rw-r--r--   0        0        0    21502 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/logo-margin/logo-white-bg.png
+-rw-r--r--   0        0        0    17722 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/python-types/image01.png
+-rw-r--r--   0        0        0    47799 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/python-types/image02.png
+-rw-r--r--   0        0        0    42872 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/python-types/image03.png
+-rw-r--r--   0        0        0    18604 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/python-types/image04.png
+-rw-r--r--   0        0        0    42637 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/python-types/image05.png
+-rw-r--r--   0        0        0    29581 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/python-types/image06.png
+-rw-r--r--   0        0        0    37057 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/budget-insight.svg
+-rw-r--r--   0        0        0    16949 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/calmcode.jpg
+-rw-r--r--   0        0        0     5321 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/classiq-banner.png
+-rw-r--r--   0        0        0     6286 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/classiq.png
+-rw-r--r--   0        0        0   133690 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/cryptapi-banner.svg
+-rw-r--r--   0        0        0   111142 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/cryptapi.svg
+-rw-r--r--   0        0        0   122267 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/databento.svg
+-rw-r--r--   0        0        0    38162 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/deta-banner.svg
+-rw-r--r--   0        0        0    56518 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/deta.svg
+-rw-r--r--   0        0        0   110000 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/docarray-top-banner.svg
+-rw-r--r--   0        0        0   129629 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/docarray.svg
+-rw-r--r--   0        0        0    53417 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/doist-banner.svg
+-rw-r--r--   0        0        0    93166 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/doist.svg
+-rw-r--r--   0        0        0    21211 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/dropbase-banner.svg
+-rw-r--r--   0        0        0     7520 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/dropbase.svg
+-rw-r--r--   0        0        0    10556 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/exoflare.png
+-rw-r--r--   0        0        0    16235 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/fastapi-course-bundle-banner.png
+-rw-r--r--   0        0        0    34985 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/fastapi-course-bundle-banner.svg
+-rw-r--r--   0        0        0    31985 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/haystack-fastapi.svg
+-rw-r--r--   0        0        0   107893 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/imgwhale-banner.svg
+-rw-r--r--   0        0        0   108995 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/imgwhale.svg
+-rw-r--r--   0        0        0    11727 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/ines-course.jpg
+-rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/investsuite.svg
+-rw-r--r--   0        0        0    14153 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/jina-ai-banner.png
+-rw-r--r--   0        0        0    26112 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/jina-ai.png
+-rw-r--r--   0        0        0    42239 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/jina-banner.svg
+-rw-r--r--   0        0        0   162873 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/jina-top-banner.svg
+-rw-r--r--   0        0        0   220435 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/jina.svg
+-rw-r--r--   0        0        0   108837 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/jina2.svg
+-rw-r--r--   0        0        0     6313 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/platform-sh-banner.png
+-rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/platform-sh.png
+-rw-r--r--   0        0        0    15311 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/powens.png
+-rw-r--r--   0        0        0     9681 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/striveworks-banner.png
+-rw-r--r--   0        0        0    22639 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/striveworks.png
+-rw-r--r--   0        0        0    34780 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/striveworks2.png
+-rw-r--r--   0        0        0    22430 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/svix.svg
+-rw-r--r--   0        0        0    14807 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/talkpython.png
+-rw-r--r--   0        0        0    26425 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/testdriven.svg
+-rw-r--r--   0        0        0    15198 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/vimso.png
+-rw-r--r--   0        0        0     6944 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/sponsors/wetransfer.svg
+-rw-r--r--   0        0        0    72424 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/additional-responses/image01.png
+-rw-r--r--   0        0        0    70687 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/async-sql-databases/image01.png
+-rw-r--r--   0        0        0    29123 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/behind-a-proxy/image01.png
+-rw-r--r--   0        0        0    62026 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/behind-a-proxy/image02.png
+-rw-r--r--   0        0        0    74280 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/behind-a-proxy/image03.png
+-rw-r--r--   0        0        0    74516 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/bigger-applications/image01.png
+-rw-r--r--   0        0        0     6230 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/bigger-applications/package.drawio
+-rw-r--r--   0        0        0    14368 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/bigger-applications/package.svg
+-rw-r--r--   0        0        0    55506 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/body/image01.png
+-rw-r--r--   0        0        0    81208 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/body/image02.png
+-rw-r--r--   0        0        0    66011 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/body/image03.png
+-rw-r--r--   0        0        0    40151 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/body/image04.png
+-rw-r--r--   0        0        0    52951 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/body/image05.png
+-rw-r--r--   0        0        0    78746 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/body-fields/image01.png
+-rw-r--r--   0        0        0    93828 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/body-fields/image02.png
+-rw-r--r--   0        0        0    40992 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/body-nested-models/image01.png
+-rw-r--r--   0        0        0    54866 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/custom-response/image01.png
+-rw-r--r--   0        0        0    72574 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/dataclasses/image01.png
+-rw-r--r--   0        0        0   173614 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/debugging/image01.png
+-rw-r--r--   0        0        0    99443 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/debugging/image02.png
+-rw-r--r--   0        0        0    79658 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/dependencies/image01.png
+-rw-r--r--   0        0        0    66817 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/dependencies/image02.png
+-rw-r--r--   0        0        0    64786 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/extending-openapi/image01.png
+-rw-r--r--   0        0        0    11292 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/extending-openapi/image02.png
+-rw-r--r--   0        0        0    11176 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/extending-openapi/image03.png
+-rw-r--r--   0        0        0    11180 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/extending-openapi/image04.png
+-rw-r--r--   0        0        0    78022 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/generate-clients/image01.png
+-rw-r--r--   0        0        0    59828 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/generate-clients/image02.png
+-rw-r--r--   0        0        0    61043 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/generate-clients/image03.png
+-rw-r--r--   0        0        0    53853 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/generate-clients/image04.png
+-rw-r--r--   0        0        0    31091 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/generate-clients/image05.png
+-rw-r--r--   0        0        0    43434 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/generate-clients/image06.png
+-rw-r--r--   0        0        0    49947 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/generate-clients/image07.png
+-rw-r--r--   0        0        0    30019 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/generate-clients/image08.png
+-rw-r--r--   0        0        0    95541 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/graphql/image01.png
+-rw-r--r--   0        0        0    90062 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/metadata/image01.png
+-rw-r--r--   0        0        0    47719 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/metadata/image02.png
+-rw-r--r--   0        0        0    99295 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/openapi-callbacks/image01.png
+-rw-r--r--   0        0        0    68080 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/path-operation-advanced-configuration/image01.png
+-rw-r--r--   0        0        0    41919 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/path-operation-configuration/image01.png
+-rw-r--r--   0        0        0    86975 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/path-operation-configuration/image02.png
+-rw-r--r--   0        0        0    71050 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/path-operation-configuration/image03.png
+-rw-r--r--   0        0        0    38687 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/path-operation-configuration/image04.png
+-rw-r--r--   0        0        0    74423 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/path-operation-configuration/image05.png
+-rw-r--r--   0        0        0    79109 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/path-params/image01.png
+-rw-r--r--   0        0        0    67289 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/path-params/image02.png
+-rw-r--r--   0        0        0   118540 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/path-params/image03.png
+-rw-r--r--   0        0        0    86345 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/query-params-str-validations/image01.png
+-rw-r--r--   0        0        0    72770 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/query-params-str-validations/image02.png
+-rw-r--r--   0        0        0    76191 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/response-model/image01.png
+-rw-r--r--   0        0        0    89115 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/response-model/image02.png
+-rw-r--r--   0        0        0    74275 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/response-status-code/image01.png
+-rw-r--r--   0        0        0    30455 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/response-status-code/image02.png
+-rw-r--r--   0        0        0    53959 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/security/image01.png
+-rw-r--r--   0        0        0    90212 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/security/image02.png
+-rw-r--r--   0        0        0    92466 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/security/image03.png
+-rw-r--r--   0        0        0    84481 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/security/image04.png
+-rw-r--r--   0        0        0    81962 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/security/image05.png
+-rw-r--r--   0        0        0    91545 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/security/image06.png
+-rw-r--r--   0        0        0    61135 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/security/image07.png
+-rw-r--r--   0        0        0    88705 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/security/image08.png
+-rw-r--r--   0        0        0   110760 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/security/image09.png
+-rw-r--r--   0        0        0   159081 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/security/image10.png
+-rw-r--r--   0        0        0    77654 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/security/image11.png
+-rw-r--r--   0        0        0    69280 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/security/image12.png
+-rw-r--r--   0        0        0    78949 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/sql-databases/image01.png
+-rw-r--r--   0        0        0    83482 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/sql-databases/image02.png
+-rw-r--r--   0        0        0    50472 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/sub-applications/image01.png
+-rw-r--r--   0        0        0    53366 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/sub-applications/image02.png
+-rw-r--r--   0        0        0    17229 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/websockets/image01.png
+-rw-r--r--   0        0        0    18326 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/websockets/image02.png
+-rw-r--r--   0        0        0    21283 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/websockets/image03.png
+-rw-r--r--   0        0        0    30900 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/websockets/image04.png
+-rw-r--r--   0        0        0    53330 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/img/tutorial/websockets/image05.png
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/js/chat.js
+-rw-r--r--   0        0        0     6734 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/js/custom.js
+-rw-r--r--   0        0        0     9540 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/js/termynal.js
+-rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/background-tasks.md
+-rw-r--r--   0        0        0    18654 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/bigger-applications.md
+-rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/body-fields.md
+-rw-r--r--   0        0        0     7858 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/body-multiple-params.md
+-rw-r--r--   0        0        0     9735 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/body-nested-models.md
+-rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/body-updates.md
+-rw-r--r--   0        0        0     7443 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/body.md
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/cookie-params.md
+-rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/cors.md
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/debugging.md
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/encoder.md
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/extra-data-types.md
+-rw-r--r--   0        0        0     7567 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/extra-models.md
+-rw-r--r--   0        0        0     9445 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/first-steps.md
+-rw-r--r--   0        0        0     9368 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/handling-errors.md
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/header-params.md
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/index.md
+-rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/metadata.md
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/middleware.md
+-rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/path-operation-configuration.md
+-rw-r--r--   0        0        0     9281 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/path-params-numeric-validations.md
+-rw-r--r--   0        0        0     9279 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/path-params.md
+-rw-r--r--   0        0        0    26454 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/query-params-str-validations.md
+-rw-r--r--   0        0        0     5210 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/query-params.md
+-rw-r--r--   0        0        0    10449 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/request-files.md
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/request-forms-and-files.md
+-rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/request-forms.md
+-rw-r--r--   0        0        0    18046 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/response-model.md
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/response-status-code.md
+-rw-r--r--   0        0        0     7356 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/schema-extra-example.md
+-rw-r--r--   0        0        0    29642 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/sql-databases.md
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/static-files.md
+-rw-r--r--   0        0        0     6380 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/testing.md
+-rw-r--r--   0        0        0    11622 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/dependencies/classes-as-dependencies.md
+-rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/dependencies/dependencies-in-path-operation-decorators.md
+-rw-r--r--   0        0        0    10848 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/dependencies/dependencies-with-yield.md
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/dependencies/global-dependencies.md
+-rw-r--r--   0        0        0    11871 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/dependencies/index.md
+-rw-r--r--   0        0        0     5742 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/dependencies/sub-dependencies.md
+-rw-r--r--   0        0        0     9112 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/security/first-steps.md
+-rw-r--r--   0        0        0     7774 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/security/get-current-user.md
+-rw-r--r--   0        0        0     4403 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/security/index.md
+-rw-r--r--   0        0        0    13286 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/security/oauth2-jwt.md
+-rw-r--r--   0        0        0    12787 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/docs/tutorial/security/simple-oauth2.md
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/en/overrides/main.html
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/es/mkdocs.yml
+-rw-r--r--   0        0        0    25513 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/es/docs/async.md
+-rw-r--r--   0        0        0    11468 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/es/docs/features.md
+-rw-r--r--   0        0        0    19594 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/es/docs/index.md
+-rw-r--r--   0        0        0     9390 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/es/docs/python-types.md
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/es/docs/advanced/additional-status-codes.md
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/es/docs/advanced/index.md
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/es/docs/advanced/path-operation-advanced-configuration.md
+-rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/es/docs/advanced/response-directly.md
+-rw-r--r--   0        0        0    10139 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/es/docs/tutorial/first-steps.md
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/es/docs/tutorial/index.md
+-rw-r--r--   0        0        0     9681 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/es/docs/tutorial/path-params.md
+-rw-r--r--   0        0        0     5207 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/es/docs/tutorial/query-params.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/es/overrides/.gitignore
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/fa/mkdocs.yml
+-rw-r--r--   0        0        0    26736 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/fa/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/fa/overrides/.gitignore
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/fr/mkdocs.yml
+-rw-r--r--   0        0        0    28159 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/fr/docs/alternatives.md
+-rw-r--r--   0        0        0    24572 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/fr/docs/async.md
+-rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/fr/docs/external-links.md
+-rw-r--r--   0        0        0     6890 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/fr/docs/fastapi-people.md
+-rw-r--r--   0        0        0    11587 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/fr/docs/features.md
+-rw-r--r--   0        0        0     7339 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/fr/docs/help-fastapi.md
+-rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/fr/docs/history-design-future.md
+-rw-r--r--   0        0        0    22777 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/fr/docs/index.md
+-rw-r--r--   0        0        0     6902 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/fr/docs/project-generation.md
+-rw-r--r--   0        0        0    10567 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/fr/docs/python-types.md
+-rw-r--r--   0        0        0     9841 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/fr/docs/advanced/additional-responses.md
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/fr/docs/advanced/additional-status-codes.md
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/fr/docs/advanced/index.md
+-rw-r--r--   0        0        0     8141 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/fr/docs/advanced/path-operation-advanced-configuration.md
+-rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/fr/docs/advanced/response-directly.md
+-rw-r--r--   0        0        0     6356 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/fr/docs/deployment/deta.md
+-rw-r--r--   0        0        0     7687 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/fr/docs/deployment/docker.md
+-rw-r--r--   0        0        0     4236 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/fr/docs/deployment/https.md
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/fr/docs/deployment/index.md
+-rw-r--r--   0        0        0     5515 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/fr/docs/deployment/manually.md
+-rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/fr/docs/deployment/versions.md
+-rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/fr/docs/tutorial/background-tasks.md
+-rw-r--r--   0        0        0     7999 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/fr/docs/tutorial/body.md
+-rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/fr/docs/tutorial/debugging.md
+-rw-r--r--   0        0        0    10563 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/fr/docs/tutorial/first-steps.md
+-rw-r--r--   0        0        0    10228 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/fr/docs/tutorial/path-params.md
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/fr/docs/tutorial/query-params.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/fr/overrides/.gitignore
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/he/mkdocs.yml
+-rw-r--r--   0        0        0    21849 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/he/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/he/overrides/.gitignore
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/hy/mkdocs.yml
+-rw-r--r--   0        0        0    18893 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/hy/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/hy/overrides/.gitignore
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/id/mkdocs.yml
+-rw-r--r--   0        0        0    18622 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/id/docs/index.md
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/id/docs/tutorial/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/id/overrides/.gitignore
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/it/mkdocs.yml
+-rw-r--r--   0        0        0    18542 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/it/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/it/overrides/.gitignore
+-rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/mkdocs.yml
+-rw-r--r--   0        0        0    32353 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/alternatives.md
+-rw-r--r--   0        0        0    28468 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/async.md
+-rw-r--r--   0        0        0     4465 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/benchmarks.md
+-rw-r--r--   0        0        0    17028 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/contributing.md
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/external-links.md
+-rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/fastapi-people.md
+-rw-r--r--   0        0        0    12779 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/features.md
+-rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/help-fastapi.md
+-rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/history-design-future.md
+-rw-r--r--   0        0        0    21628 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/index.md
+-rw-r--r--   0        0        0     7264 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/project-generation.md
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/advanced/additional-status-codes.md
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/advanced/conditional-openapi.md
+-rw-r--r--   0        0        0    10906 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/advanced/custom-response.md
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/advanced/index.md
+-rw-r--r--   0        0        0     7142 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/advanced/nosql-databases.md
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/advanced/path-operation-advanced-configuration.md
+-rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/advanced/response-directly.md
+-rw-r--r--   0        0        0     7405 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/advanced/websockets.md
+-rw-r--r--   0        0        0     6667 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/deployment/deta.md
+-rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/deployment/docker.md
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/deployment/index.md
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/deployment/manually.md
+-rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/deployment/versions.md
+-rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/tutorial/body-updates.md
+-rw-r--r--   0        0        0     8130 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/tutorial/body.md
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/tutorial/cookie-params.md
+-rw-r--r--   0        0        0     6422 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/tutorial/cors.md
+-rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/tutorial/debugging.md
+-rw-r--r--   0        0        0    11456 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/tutorial/first-steps.md
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/tutorial/header-params.md
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/tutorial/index.md
+-rw-r--r--   0        0        0     3905 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/tutorial/middleware.md
+-rw-r--r--   0        0        0    10867 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/tutorial/path-params.md
+-rw-r--r--   0        0        0    10789 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/tutorial/query-params-str-validations.md
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/tutorial/query-params.md
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/tutorial/request-forms.md
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/tutorial/static-files.md
+-rw-r--r--   0        0        0     5977 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/tutorial/testing.md
+-rw-r--r--   0        0        0    10737 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/tutorial/security/first-steps.md
+-rw-r--r--   0        0        0    14484 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/docs/tutorial/security/oauth2-jwt.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ja/overrides/.gitignore
+-rw-r--r--   0        0        0     3921 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ko/mkdocs.yml
+-rw-r--r--   0        0        0    20074 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ko/docs/index.md
+-rw-r--r--   0        0        0     4217 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ko/docs/deployment/versions.md
+-rw-r--r--   0        0        0     5905 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ko/docs/tutorial/cors.md
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ko/docs/tutorial/encoder.md
+-rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ko/docs/tutorial/first-steps.md
+-rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ko/docs/tutorial/header-params.md
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ko/docs/tutorial/index.md
+-rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ko/docs/tutorial/path-params-numeric-validations.md
+-rw-r--r--   0        0        0     9880 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ko/docs/tutorial/path-params.md
+-rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ko/docs/tutorial/query-params.md
+-rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ko/docs/tutorial/request-files.md
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ko/docs/tutorial/request-forms-and-files.md
+-rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ko/docs/tutorial/response-status-code.md
+-rw-r--r--   0        0        0     8167 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ko/docs/tutorial/dependencies/classes-as-dependencies.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ko/overrides/.gitignore
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/lo/mkdocs.yml
+-rw-r--r--   0        0        0    19423 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/lo/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/lo/overrides/.gitignore
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/nl/mkdocs.yml
+-rw-r--r--   0        0        0    18863 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/nl/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/nl/overrides/.gitignore
+-rw-r--r--   0        0        0     3542 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pl/mkdocs.yml
+-rw-r--r--   0        0        0    20000 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pl/docs/index.md
+-rw-r--r--   0        0        0    10055 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pl/docs/tutorial/first-steps.md
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pl/docs/tutorial/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pl/overrides/.gitignore
+-rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/mkdocs.yml
+-rw-r--r--   0        0        0    26158 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/alternatives.md
+-rw-r--r--   0        0        0    22758 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/async.md
+-rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/benchmarks.md
+-rw-r--r--   0        0        0    15229 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/contributing.md
+-rw-r--r--   0        0        0    17171 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/deployment.md
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/external-links.md
+-rw-r--r--   0        0        0     6586 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/fastapi-people.md
+-rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/features.md
+-rw-r--r--   0        0        0     8848 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/help-fastapi.md
+-rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/history-design-future.md
+-rw-r--r--   0        0        0    19250 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/index.md
+-rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/project-generation.md
+-rw-r--r--   0        0        0     9892 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/python-types.md
+-rw-r--r--   0        0        0     8854 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/advanced/events.md
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/advanced/index.md
+-rw-r--r--   0        0        0     7211 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/deployment/deta.md
+-rw-r--r--   0        0        0    38309 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/deployment/docker.md
+-rw-r--r--   0        0        0     3979 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/deployment/https.md
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/deployment/index.md
+-rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/deployment/versions.md
+-rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/tutorial/background-tasks.md
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/tutorial/body-fields.md
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/tutorial/body-multiple-params.md
+-rw-r--r--   0        0        0     7563 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/tutorial/body-nested-models.md
+-rw-r--r--   0        0        0     7294 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/tutorial/body.md
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/tutorial/cookie-params.md
+-rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/tutorial/encoder.md
+-rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/tutorial/extra-data-types.md
+-rw-r--r--   0        0        0     8000 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/tutorial/extra-models.md
+-rw-r--r--   0        0        0     9849 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/tutorial/first-steps.md
+-rw-r--r--   0        0        0    10274 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/tutorial/handling-errors.md
+-rw-r--r--   0        0        0     3974 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/tutorial/header-params.md
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/tutorial/index.md
+-rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/tutorial/path-operation-configuration.md
+-rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/tutorial/path-params-numeric-validations.md
+-rw-r--r--   0        0        0     9946 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/tutorial/path-params.md
+-rw-r--r--   0        0        0     9547 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/tutorial/query-params-str-validations.md
+-rw-r--r--   0        0        0     5688 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/tutorial/query-params.md
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/tutorial/request-forms-and-files.md
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/tutorial/request-forms.md
+-rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/tutorial/response-status-code.md
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/tutorial/static-files.md
+-rw-r--r--   0        0        0     8499 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/tutorial/security/first-steps.md
+-rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/docs/tutorial/security/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/pt/overrides/.gitignore
+-rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ru/mkdocs.yml
+-rw-r--r--   0        0        0    40311 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ru/docs/alternatives.md
+-rw-r--r--   0        0        0    40878 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ru/docs/async.md
+-rw-r--r--   0        0        0     6201 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ru/docs/benchmarks.md
+-rw-r--r--   0        0        0    23066 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ru/docs/contributing.md
+-rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ru/docs/external-links.md
+-rw-r--r--   0        0        0     8880 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ru/docs/fastapi-people.md
+-rw-r--r--   0        0        0    16914 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ru/docs/features.md
+-rw-r--r--   0        0        0    23415 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ru/docs/help-fastapi.md
+-rw-r--r--   0        0        0     7421 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ru/docs/history-design-future.md
+-rw-r--r--   0        0        0    26659 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ru/docs/index.md
+-rw-r--r--   0        0        0    10763 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ru/docs/project-generation.md
+-rw-r--r--   0        0        0    14967 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ru/docs/python-types.md
+-rw-r--r--   0        0        0    33259 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ru/docs/deployment/concepts.md
+-rw-r--r--   0        0        0    21137 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ru/docs/deployment/https.md
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ru/docs/deployment/index.md
+-rw-r--r--   0        0        0     7961 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ru/docs/deployment/manually.md
+-rw-r--r--   0        0        0     5793 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ru/docs/deployment/versions.md
+-rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ru/docs/tutorial/background-tasks.md
+-rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ru/docs/tutorial/body-fields.md
+-rw-r--r--   0        0        0    11923 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ru/docs/tutorial/body-multiple-params.md
+-rw-r--r--   0        0        0    11229 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ru/docs/tutorial/body.md
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ru/docs/tutorial/cookie-params.md
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ru/docs/tutorial/debugging.md
+-rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ru/docs/tutorial/extra-data-types.md
+-rw-r--r--   0        0        0    13423 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ru/docs/tutorial/first-steps.md
+-rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ru/docs/tutorial/index.md
+-rw-r--r--   0        0        0    14571 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ru/docs/tutorial/path-params-numeric-validations.md
+-rw-r--r--   0        0        0    14436 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ru/docs/tutorial/path-params.md
+-rw-r--r--   0        0        0    38884 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ru/docs/tutorial/query-params-str-validations.md
+-rw-r--r--   0        0        0     8575 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ru/docs/tutorial/query-params.md
+-rw-r--r--   0        0        0     7166 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ru/docs/tutorial/response-status-code.md
+-rw-r--r--   0        0        0    11861 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ru/docs/tutorial/schema-extra-example.md
+-rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ru/docs/tutorial/static-files.md
+-rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ru/docs/tutorial/testing.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ru/overrides/.gitignore
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/sq/mkdocs.yml
+-rw-r--r--   0        0        0    18625 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/sq/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/sq/overrides/.gitignore
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/sv/mkdocs.yml
+-rw-r--r--   0        0        0    18863 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/sv/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/sv/overrides/.gitignore
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ta/mkdocs.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/ta/overrides/.gitignore
+-rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/tr/mkdocs.yml
+-rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/tr/docs/benchmarks.md
+-rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/tr/docs/fastapi-people.md
+-rw-r--r--   0        0        0    11579 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/tr/docs/features.md
+-rw-r--r--   0        0        0    20806 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/tr/docs/index.md
+-rw-r--r--   0        0        0     9971 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/tr/docs/python-types.md
+-rw-r--r--   0        0        0    10004 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/tr/docs/tutorial/first_steps.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/tr/overrides/.gitignore
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/uk/mkdocs.yml
+-rw-r--r--   0        0        0    18625 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/uk/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/uk/overrides/.gitignore
+-rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/mkdocs.yml
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/benchmarks.md
+-rw-r--r--   0        0        0    13647 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/contributing.md
+-rw-r--r--   0        0        0     6177 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/fastapi-people.md
+-rw-r--r--   0        0        0     9335 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/features.md
+-rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/help-fastapi.md
+-rw-r--r--   0        0        0    18563 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/index.md
+-rw-r--r--   0        0        0     8827 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/python-types.md
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/advanced/additional-status-codes.md
+-rw-r--r--   0        0        0     7939 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/advanced/custom-response.md
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/advanced/index.md
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/advanced/path-operation-advanced-configuration.md
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/advanced/response-change-status-code.md
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/advanced/response-cookies.md
+-rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/advanced/response-directly.md
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/advanced/response-headers.md
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/advanced/wsgi.md
+-rw-r--r--   0        0        0    18647 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/bigger-applications.md
+-rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/body-fields.md
+-rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/body-multiple-params.md
+-rw-r--r--   0        0        0     7030 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/body-nested-models.md
+-rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/body-updates.md
+-rw-r--r--   0        0        0     5620 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/body.md
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/cookie-params.md
+-rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/cors.md
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/debugging.md
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/encoder.md
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/extra-data-types.md
+-rw-r--r--   0        0        0     6065 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/extra-models.md
+-rw-r--r--   0        0        0     9408 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/first-steps.md
+-rw-r--r--   0        0        0     8638 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/handling-errors.md
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/header-params.md
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/index.md
+-rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/metadata.md
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/middleware.md
+-rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/path-operation-configuration.md
+-rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/path-params-numeric-validations.md
+-rw-r--r--   0        0        0     8476 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/path-params.md
+-rw-r--r--   0        0        0     9302 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/query-params-str-validations.md
+-rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/query-params.md
+-rw-r--r--   0        0        0     7072 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/request-files.md
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/request-forms-and-files.md
+-rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/request-forms.md
+-rw-r--r--   0        0        0     7297 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/response-model.md
+-rw-r--r--   0        0        0     4110 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/response-status-code.md
+-rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/schema-extra-example.md
+-rw-r--r--   0        0        0    27546 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/sql-databases.md
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/static-files.md
+-rw-r--r--   0        0        0     6650 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/dependencies/classes-as-dependencies.md
+-rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/dependencies/dependencies-in-path-operation-decorators.md
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/dependencies/global-dependencies.md
+-rw-r--r--   0        0        0     7202 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/dependencies/index.md
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/dependencies/sub-dependencies.md
+-rw-r--r--   0        0        0     7256 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/security/first-steps.md
+-rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/security/get-current-user.md
+-rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/security/index.md
+-rw-r--r--   0        0        0     9457 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/security/oauth2-jwt.md
+-rw-r--r--   0        0        0     9566 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/docs/tutorial/security/simple-oauth2.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs/zh/overrides/.gitignore
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/additional_responses/tutorial001.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/additional_responses/tutorial002.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/additional_responses/tutorial003.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/additional_responses/tutorial004.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/additional_status_codes/tutorial001.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/additional_status_codes/tutorial001_an.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/additional_status_codes/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/additional_status_codes/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/additional_status_codes/tutorial001_py310.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/advanced_middleware/tutorial001.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/advanced_middleware/tutorial002.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/advanced_middleware/tutorial003.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/app_testing/__init__.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/app_testing/main.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/app_testing/test_main.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/app_testing/tutorial001.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/app_testing/tutorial002.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/app_testing/tutorial003.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/app_testing/app_b/__init__.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/app_testing/app_b/main.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/app_testing/app_b/test_main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/app_testing/app_b_an/__init__.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/app_testing/app_b_an/main.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/app_testing/app_b_an/test_main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/app_testing/app_b_an_py310/__init__.py
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/app_testing/app_b_an_py310/main.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/app_testing/app_b_an_py310/test_main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/app_testing/app_b_an_py39/__init__.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/app_testing/app_b_an_py39/main.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/app_testing/app_b_an_py39/test_main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/app_testing/app_b_py310/__init__.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/app_testing/app_b_py310/main.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/app_testing/app_b_py310/test_main.py
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/async_sql_databases/tutorial001.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/async_tests/__init__.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/async_tests/main.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/async_tests/test_main.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/background_tasks/tutorial001.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/background_tasks/tutorial002.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/background_tasks/tutorial002_an.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/background_tasks/tutorial002_an_py310.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/background_tasks/tutorial002_an_py39.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/background_tasks/tutorial002_py310.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/behind_a_proxy/tutorial001.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/behind_a_proxy/tutorial002.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/behind_a_proxy/tutorial003.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/behind_a_proxy/tutorial004.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/bigger_applications/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/bigger_applications/app/__init__.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/bigger_applications/app/dependencies.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/bigger_applications/app/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/bigger_applications/app/internal/__init__.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/bigger_applications/app/internal/admin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/bigger_applications/app/routers/__init__.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/bigger_applications/app/routers/items.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/bigger_applications/app/routers/users.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/bigger_applications/app_an/__init__.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/bigger_applications/app_an/dependencies.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/bigger_applications/app_an/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/bigger_applications/app_an/internal/__init__.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/bigger_applications/app_an/internal/admin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/bigger_applications/app_an/routers/__init__.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/bigger_applications/app_an/routers/items.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/bigger_applications/app_an/routers/users.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/bigger_applications/app_an_py39/__init__.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/bigger_applications/app_an_py39/dependencies.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/bigger_applications/app_an_py39/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/bigger_applications/app_an_py39/internal/__init__.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/bigger_applications/app_an_py39/internal/admin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/bigger_applications/app_an_py39/routers/__init__.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/bigger_applications/app_an_py39/routers/items.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/bigger_applications/app_an_py39/routers/users.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body/tutorial001.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body/tutorial001_py310.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body/tutorial002.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body/tutorial002_py310.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body/tutorial003.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body/tutorial003_py310.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body/tutorial004.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body/tutorial004_py310.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_fields/tutorial001.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_fields/tutorial001_an.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_fields/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_fields/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_fields/tutorial001_py310.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_multiple_params/tutorial001.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_multiple_params/tutorial001_an.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_multiple_params/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_multiple_params/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_multiple_params/tutorial001_py310.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_multiple_params/tutorial002.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_multiple_params/tutorial002_py310.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_multiple_params/tutorial003.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_multiple_params/tutorial003_an.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_multiple_params/tutorial003_an_py310.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_multiple_params/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_multiple_params/tutorial003_py310.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_multiple_params/tutorial004.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_multiple_params/tutorial004_an.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_multiple_params/tutorial004_an_py310.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_multiple_params/tutorial004_an_py39.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_multiple_params/tutorial004_py310.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_multiple_params/tutorial005.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_multiple_params/tutorial005_an.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_multiple_params/tutorial005_an_py310.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_multiple_params/tutorial005_an_py39.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_multiple_params/tutorial005_py310.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_nested_models/tutorial001.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_nested_models/tutorial001_py310.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_nested_models/tutorial002.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_nested_models/tutorial002_py310.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_nested_models/tutorial002_py39.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_nested_models/tutorial003.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_nested_models/tutorial003_py310.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_nested_models/tutorial003_py39.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_nested_models/tutorial004.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_nested_models/tutorial004_py310.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_nested_models/tutorial004_py39.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_nested_models/tutorial005.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_nested_models/tutorial005_py310.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_nested_models/tutorial005_py39.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_nested_models/tutorial006.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_nested_models/tutorial006_py310.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_nested_models/tutorial006_py39.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_nested_models/tutorial007.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_nested_models/tutorial007_py310.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_nested_models/tutorial007_py39.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_nested_models/tutorial008.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_nested_models/tutorial008_py39.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_nested_models/tutorial009.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_nested_models/tutorial009_py39.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_updates/tutorial001.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_updates/tutorial001_py310.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_updates/tutorial001_py39.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_updates/tutorial002.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_updates/tutorial002_py310.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/body_updates/tutorial002_py39.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/conditional_openapi/tutorial001.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/cookie_params/tutorial001.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/cookie_params/tutorial001_an.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/cookie_params/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/cookie_params/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/cookie_params/tutorial001_py310.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/cors/tutorial001.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/custom_request_and_route/tutorial001.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/custom_request_and_route/tutorial002.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/custom_request_and_route/tutorial003.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/custom_response/tutorial001.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/custom_response/tutorial001b.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/custom_response/tutorial002.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/custom_response/tutorial003.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/custom_response/tutorial004.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/custom_response/tutorial005.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/custom_response/tutorial006.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/custom_response/tutorial006b.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/custom_response/tutorial006c.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/custom_response/tutorial007.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/custom_response/tutorial008.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/custom_response/tutorial009.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/custom_response/tutorial009b.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/custom_response/tutorial009c.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/custom_response/tutorial010.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dataclasses/tutorial001.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dataclasses/tutorial002.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dataclasses/tutorial003.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/debugging/tutorial001.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial001.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial001_02_an.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial001_02_an_py310.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial001_02_an_py39.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial001_an.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial001_py310.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial002.py
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial002_an.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial002_an_py310.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial002_an_py39.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial002_py310.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial003.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial003_an.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial003_an_py310.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial003_py310.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial004.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial004_an.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial004_an_py310.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial004_an_py39.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial004_py310.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial005.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial005_an.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial005_an_py310.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial005_an_py39.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial005_py310.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial006.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial006_an.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial006_an_py39.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial007.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial008.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial008_an.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial008_an_py39.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial009.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial010.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial011.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial011_an.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial011_an_py39.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial012.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial012_an.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependencies/tutorial012_an_py39.py
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependency_testing/tutorial001.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependency_testing/tutorial001_an.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependency_testing/tutorial001_an_py310.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependency_testing/tutorial001_an_py39.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/dependency_testing/tutorial001_py310.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/encoder/tutorial001.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/encoder/tutorial001_py310.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/events/tutorial001.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/events/tutorial002.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/events/tutorial003.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/extending_openapi/tutorial001.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/extending_openapi/tutorial002.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/extending_openapi/tutorial003.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/extending_openapi/tutorial004.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/extending_openapi/tutorial005.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/extra_data_types/tutorial001.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/extra_data_types/tutorial001_an.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/extra_data_types/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/extra_data_types/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/extra_data_types/tutorial001_py310.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/extra_models/tutorial001.py
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/extra_models/tutorial001_py310.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/extra_models/tutorial002.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/extra_models/tutorial002_py310.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/extra_models/tutorial003.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/extra_models/tutorial003_py310.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/extra_models/tutorial004.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/extra_models/tutorial004_py39.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/extra_models/tutorial005.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/extra_models/tutorial005_py39.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/first_steps/tutorial001.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/first_steps/tutorial002.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/first_steps/tutorial003.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/generate_clients/tutorial001.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/generate_clients/tutorial001_py39.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/generate_clients/tutorial002.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/generate_clients/tutorial002_py39.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/generate_clients/tutorial003.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/generate_clients/tutorial003_py39.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/generate_clients/tutorial004.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/graphql/tutorial001.py
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/handling_errors/tutorial001.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/handling_errors/tutorial002.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/handling_errors/tutorial003.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/handling_errors/tutorial004.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/handling_errors/tutorial005.py
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/handling_errors/tutorial006.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/header_params/tutorial001.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/header_params/tutorial001_an.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/header_params/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/header_params/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/header_params/tutorial001_py310.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/header_params/tutorial002.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/header_params/tutorial002_an.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/header_params/tutorial002_an_py310.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/header_params/tutorial002_an_py39.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/header_params/tutorial002_py310.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/header_params/tutorial003.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/header_params/tutorial003_an.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/header_params/tutorial003_an_py310.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/header_params/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/header_params/tutorial003_py310.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/header_params/tutorial003_py39.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/metadata/tutorial001.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/metadata/tutorial002.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/metadata/tutorial003.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/metadata/tutorial004.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/middleware/tutorial001.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/nosql_databases/tutorial001.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/openapi_callbacks/tutorial001.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_operation_advanced_configuration/tutorial001.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_operation_advanced_configuration/tutorial002.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_operation_advanced_configuration/tutorial003.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_operation_advanced_configuration/tutorial004.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_operation_advanced_configuration/tutorial005.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_operation_advanced_configuration/tutorial006.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_operation_advanced_configuration/tutorial007.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_operation_configuration/tutorial001.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_operation_configuration/tutorial001_py310.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_operation_configuration/tutorial001_py39.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_operation_configuration/tutorial002.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_operation_configuration/tutorial002_py310.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_operation_configuration/tutorial002_py39.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_operation_configuration/tutorial002b.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_operation_configuration/tutorial003.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_operation_configuration/tutorial003_py310.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_operation_configuration/tutorial003_py39.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_operation_configuration/tutorial004.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_operation_configuration/tutorial004_py310.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_operation_configuration/tutorial004_py39.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_operation_configuration/tutorial005.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_operation_configuration/tutorial005_py310.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_operation_configuration/tutorial005_py39.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_operation_configuration/tutorial006.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_params/tutorial001.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_params/tutorial002.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_params/tutorial003.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_params/tutorial003b.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_params/tutorial004.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_params/tutorial005.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_params_numeric_validations/tutorial001.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_params_numeric_validations/tutorial001_an.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_params_numeric_validations/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_params_numeric_validations/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_params_numeric_validations/tutorial001_py310.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_params_numeric_validations/tutorial002.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_params_numeric_validations/tutorial002_an.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_params_numeric_validations/tutorial002_an_py39.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_params_numeric_validations/tutorial003.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_params_numeric_validations/tutorial003_an.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_params_numeric_validations/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_params_numeric_validations/tutorial004.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_params_numeric_validations/tutorial004_an.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_params_numeric_validations/tutorial004_an_py39.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_params_numeric_validations/tutorial005.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_params_numeric_validations/tutorial005_an.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_params_numeric_validations/tutorial005_an_py39.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_params_numeric_validations/tutorial006.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_params_numeric_validations/tutorial006_an.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/path_params_numeric_validations/tutorial006_an_py39.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/python_types/tutorial001.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/python_types/tutorial002.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/python_types/tutorial003.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/python_types/tutorial004.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/python_types/tutorial005.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/python_types/tutorial006.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/python_types/tutorial006_py39.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/python_types/tutorial007.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/python_types/tutorial007_py39.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/python_types/tutorial008.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/python_types/tutorial008_py39.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/python_types/tutorial008b.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/python_types/tutorial008b_py310.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/python_types/tutorial009.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/python_types/tutorial009_py310.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/python_types/tutorial009b.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/python_types/tutorial009c.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/python_types/tutorial009c_py310.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/python_types/tutorial010.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/python_types/tutorial011.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/python_types/tutorial011_py310.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/python_types/tutorial011_py39.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/python_types/tutorial012.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/python_types/tutorial013.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/python_types/tutorial013_py39.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params/tutorial001.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params/tutorial002.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params/tutorial002_py310.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params/tutorial003.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params/tutorial003_py310.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params/tutorial004.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params/tutorial004_py310.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params/tutorial005.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params/tutorial006.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params/tutorial006_py310.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params/tutorial006b.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial001.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial001_py310.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial002.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial002_an.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial002_an_py310.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial002_py310.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial003.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial003_an.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial003_an_py310.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial003_py310.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial004.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial004_an.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial004_an_py310.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial004_an_py39.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial004_py310.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial005.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial005_an.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial005_an_py39.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial006.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial006_an.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial006_an_py39.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial006b.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial006b_an.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial006b_an_py39.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial006c.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial006c_an.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial006c_an_py310.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial006c_an_py39.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial006c_py310.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial006d.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial006d_an.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial006d_an_py39.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial007.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial007_an.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial007_an_py310.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial007_an_py39.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial007_py310.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial008.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial008_an.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial008_an_py310.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial008_an_py39.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial008_py310.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial009.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial009_an.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial009_an_py310.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial009_an_py39.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial009_py310.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial010.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial010_an.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial010_an_py310.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial010_an_py39.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial010_py310.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial011.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial011_an.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial011_an_py310.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial011_an_py39.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial011_py310.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial011_py39.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial012.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial012_an.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial012_an_py39.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial012_py39.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial013.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial013_an.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial013_an_py39.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial014.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial014_an.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial014_an_py310.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial014_an_py39.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/query_params_str_validations/tutorial014_py310.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/request_files/tutorial001.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/request_files/tutorial001_02.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/request_files/tutorial001_02_an.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/request_files/tutorial001_02_an_py310.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/request_files/tutorial001_02_an_py39.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/request_files/tutorial001_02_py310.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/request_files/tutorial001_03.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/request_files/tutorial001_03_an.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/request_files/tutorial001_03_an_py39.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/request_files/tutorial001_an.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/request_files/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/request_files/tutorial002.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/request_files/tutorial002_an.py
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/request_files/tutorial002_an_py39.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/request_files/tutorial002_py39.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/request_files/tutorial003.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/request_files/tutorial003_an.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/request_files/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/request_files/tutorial003_py39.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/request_forms/tutorial001.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/request_forms/tutorial001_an.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/request_forms/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/request_forms_and_files/tutorial001.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/request_forms_and_files/tutorial001_an.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/request_forms_and_files/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/response_change_status_code/tutorial001.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/response_cookies/tutorial001.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/response_cookies/tutorial002.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/response_directly/tutorial001.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/response_directly/tutorial002.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/response_headers/tutorial001.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/response_headers/tutorial002.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/response_model/tutorial001.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/response_model/tutorial001_01.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/response_model/tutorial001_01_py310.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/response_model/tutorial001_01_py39.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/response_model/tutorial001_py310.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/response_model/tutorial001_py39.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/response_model/tutorial002.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/response_model/tutorial002_py310.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/response_model/tutorial003.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/response_model/tutorial003_01.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/response_model/tutorial003_01_py310.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/response_model/tutorial003_02.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/response_model/tutorial003_03.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/response_model/tutorial003_04.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/response_model/tutorial003_04_py310.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/response_model/tutorial003_05.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/response_model/tutorial003_05_py310.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/response_model/tutorial003_py310.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/response_model/tutorial004.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/response_model/tutorial004_py310.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/response_model/tutorial004_py39.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/response_model/tutorial005.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/response_model/tutorial005_py310.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/response_model/tutorial006.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/response_model/tutorial006_py310.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/response_status_code/tutorial001.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/response_status_code/tutorial002.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/schema_extra_example/tutorial001.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/schema_extra_example/tutorial001_py310.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/schema_extra_example/tutorial002.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/schema_extra_example/tutorial002_py310.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/schema_extra_example/tutorial003.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/schema_extra_example/tutorial003_an.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/schema_extra_example/tutorial003_an_py310.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/schema_extra_example/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/schema_extra_example/tutorial003_py310.py
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/schema_extra_example/tutorial004.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/schema_extra_example/tutorial004_an.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/schema_extra_example/tutorial004_an_py310.py
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/schema_extra_example/tutorial004_an_py39.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/schema_extra_example/tutorial004_py310.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/security/tutorial001.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/security/tutorial001_an.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/security/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/security/tutorial002.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/security/tutorial002_an.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/security/tutorial002_an_py310.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/security/tutorial002_an_py39.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/security/tutorial002_py310.py
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/security/tutorial003.py
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/security/tutorial003_an.py
+-rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/security/tutorial003_an_py310.py
+-rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/security/tutorial003_an_py39.py
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/security/tutorial003_py310.py
+-rw-r--r--   0        0        0     4113 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/security/tutorial004.py
+-rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/security/tutorial004_an.py
+-rw-r--r--   0        0        0     4161 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/security/tutorial004_an_py310.py
+-rw-r--r--   0        0        0     4198 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/security/tutorial004_an_py39.py
+-rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/security/tutorial004_py310.py
+-rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/security/tutorial005.py
+-rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/security/tutorial005_an.py
+-rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/security/tutorial005_an_py310.py
+-rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/security/tutorial005_an_py39.py
+-rw-r--r--   0        0        0     5186 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/security/tutorial005_py310.py
+-rw-r--r--   0        0        0     5241 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/security/tutorial005_py39.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/security/tutorial006.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/security/tutorial006_an.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/security/tutorial006_an_py39.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/security/tutorial007.py
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/security/tutorial007_an.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/security/tutorial007_an_py39.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/settings/tutorial001.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/settings/app01/__init__.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/settings/app01/config.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/settings/app01/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/settings/app02/__init__.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/settings/app02/config.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/settings/app02/main.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/settings/app02/test_main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/settings/app02_an/__init__.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/settings/app02_an/config.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/settings/app02_an/main.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/settings/app02_an/test_main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/settings/app02_an_py39/__init__.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/settings/app02_an_py39/config.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/settings/app02_an_py39/main.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/settings/app02_an_py39/test_main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/settings/app03/__init__.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/settings/app03/config.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/settings/app03/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/settings/app03_an/__init__.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/settings/app03_an/config.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/settings/app03_an/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/settings/app03_an_py39/__init__.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/settings/app03_an_py39/config.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/settings/app03_an_py39/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/sql_databases/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/sql_databases/sql_app/__init__.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/sql_databases/sql_app/alt_main.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/sql_databases/sql_app/crud.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/sql_databases/sql_app/database.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/sql_databases/sql_app/main.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/sql_databases/sql_app/models.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/sql_databases/sql_app/schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/sql_databases/sql_app/tests/__init__.py
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/sql_databases/sql_app/tests/test_sql_app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/sql_databases/sql_app_py310/__init__.py
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/sql_databases/sql_app_py310/alt_main.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/sql_databases/sql_app_py310/crud.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/sql_databases/sql_app_py310/database.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/sql_databases/sql_app_py310/main.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/sql_databases/sql_app_py310/models.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/sql_databases/sql_app_py310/schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/sql_databases/sql_app_py310/tests/__init__.py
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/sql_databases/sql_app_py310/tests/test_sql_app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/sql_databases/sql_app_py39/__init__.py
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/sql_databases/sql_app_py39/alt_main.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/sql_databases/sql_app_py39/crud.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/sql_databases/sql_app_py39/database.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/sql_databases/sql_app_py39/main.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/sql_databases/sql_app_py39/models.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/sql_databases/sql_app_py39/schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/sql_databases/sql_app_py39/tests/__init__.py
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/sql_databases/sql_app_py39/tests/test_sql_app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/sql_databases_peewee/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/sql_databases_peewee/sql_app/__init__.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/sql_databases_peewee/sql_app/crud.py
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/sql_databases_peewee/sql_app/database.py
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/sql_databases_peewee/sql_app/main.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/sql_databases_peewee/sql_app/models.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/sql_databases_peewee/sql_app/schemas.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/static_files/tutorial001.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/sub_applications/tutorial001.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/templates/tutorial001.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/templates/static/styles.css
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/templates/templates/item.html
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/using_request_directly/tutorial001.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/websockets/__init__.py
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/websockets/tutorial001.py
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/websockets/tutorial002.py
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/websockets/tutorial002_an.py
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/websockets/tutorial002_an_py310.py
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/websockets/tutorial002_an_py39.py
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/websockets/tutorial002_py310.py
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/websockets/tutorial003.py
+-rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/websockets/tutorial003_py39.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 fastapi-0.97.0/docs_src/wsgi/tutorial001.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/__init__.py
+-rw-r--r--   0        0        0    40237 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/applications.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/background.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/concurrency.py
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/datastructures.py
+-rw-r--r--   0        0        0     5962 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/encoders.py
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/exception_handlers.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/exceptions.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/logger.py
+-rw-r--r--   0        0        0     7515 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/param_functions.py
+-rw-r--r--   0        0        0    10699 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/params.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/py.typed
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/requests.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/responses.py
+-rw-r--r--   0        0        0    56490 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/routing.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/staticfiles.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/templating.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/testclient.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/types.py
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/utils.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/websockets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/dependencies/__init__.py
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/dependencies/models.py
+-rw-r--r--   0        0        0    30908 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/dependencies/utils.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/middleware/__init__.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/middleware/asyncexitstack.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/middleware/cors.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/middleware/gzip.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/middleware/httpsredirect.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/middleware/trustedhost.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/middleware/wsgi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/openapi/__init__.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/openapi/constants.py
+-rw-r--r--   0        0        0     6532 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/openapi/docs.py
+-rw-r--r--   0        0        0    11204 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/openapi/models.py
+-rw-r--r--   0        0        0    18778 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/openapi/utils.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/security/__init__.py
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/security/api_key.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/security/base.py
+-rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/security/http.py
+-rw-r--r--   0        0        0     8360 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/security/oauth2.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/security/open_id_connect_url.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 fastapi-0.97.0/fastapi/security/utils.py
+-rwxr-xr-x   0        0        0      142 2020-02-02 00:00:00.000000 fastapi-0.97.0/scripts/build-docs.sh
+-rwxr-xr-x   0        0        0       98 2020-02-02 00:00:00.000000 fastapi-0.97.0/scripts/clean.sh
+-rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 fastapi-0.97.0/scripts/docs-live.sh
+-rw-r--r--   0        0        0    15500 2020-02-02 00:00:00.000000 fastapi-0.97.0/scripts/docs.py
+-rwxr-xr-x   0        0        0      100 2020-02-02 00:00:00.000000 fastapi-0.97.0/scripts/format.sh
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 fastapi-0.97.0/scripts/gitter_releases_bot.py
+-rwxr-xr-x   0        0        0      113 2020-02-02 00:00:00.000000 fastapi-0.97.0/scripts/lint.sh
+-rwxr-xr-x   0        0        0      337 2020-02-02 00:00:00.000000 fastapi-0.97.0/scripts/netlify-docs.sh
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 fastapi-0.97.0/scripts/notify.sh
+-rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 fastapi-0.97.0/scripts/publish.sh
+-rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 fastapi-0.97.0/scripts/test-cov-html.sh
+-rwxr-xr-x   0        0        0       99 2020-02-02 00:00:00.000000 fastapi-0.97.0/scripts/test.sh
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 fastapi-0.97.0/scripts/zip-docs.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/__init__.py
+-rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/main.py
+-rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_additional_properties.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_additional_response_extra.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_additional_responses_bad.py
+-rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_additional_responses_custom_model_in_callback.py
+-rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_additional_responses_custom_validationerror.py
+-rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_additional_responses_default_validationerror.py
+-rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_additional_responses_response_class.py
+-rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_additional_responses_router.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_ambiguous_params.py
+-rw-r--r--   0        0        0     9779 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_annotated.py
+-rw-r--r--   0        0        0    49052 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_application.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_callable_endpoint.py
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_custom_middleware_exception.py
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_custom_route_class.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_custom_schema_fields.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_custom_swagger_ui_redirect.py
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_datastructures.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_datetime_custom_encoder.py
+-rw-r--r--   0        0        0     5365 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_default_response_class.py
+-rw-r--r--   0        0        0     5117 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_default_response_class_router.py
+-rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_dependency_cache.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_dependency_class.py
+-rw-r--r--   0        0        0    11269 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_dependency_contextmanager.py
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_dependency_contextvars.py
+-rw-r--r--   0        0        0     8164 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_dependency_duplicates.py
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_dependency_normal_exceptions.py
+-rw-r--r--   0        0        0     9010 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_dependency_overrides.py
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_dependency_security_overrides.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_deprecated_openapi_prefix.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_duplicate_models_openapi.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_empty_router.py
+-rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_enforce_once_required_parameter.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_exception_handlers.py
+-rw-r--r--   0        0        0    13670 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_extra_routes.py
+-rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_filter_pydantic_sub_model.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_forms_from_non_typing_sequences.py
+-rw-r--r--   0        0        0    68172 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_generate_unique_id_function.py
+-rw-r--r--   0        0        0     3744 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_get_request_body.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_http_connection_injection.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_include_route.py
+-rw-r--r--   0        0        0   367192 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_include_router_defaults_overrides.py
+-rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_infer_param_optionality.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_inherited_custom_class.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_invalid_path_param.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_invalid_sequence_param.py
+-rw-r--r--   0        0        0     6861 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_jsonable_encoder.py
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_local_docs.py
+-rw-r--r--   0        0        0     5391 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_multi_body_errors.py
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_multi_query_errors.py
+-rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_multipart_installation.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_no_swagger_ui_redirect.py
+-rw-r--r--   0        0        0     4311 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_openapi_query_parameter_extension.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_openapi_route_extensions.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_openapi_servers.py
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_operations_signatures.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_orjson_response_class.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_param_class.py
+-rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_param_in_path_and_dependency.py
+-rw-r--r--   0        0        0     7606 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_param_include_in_schema.py
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_params_repr.py
+-rw-r--r--   0        0        0     7774 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_path.py
+-rw-r--r--   0        0        0     3362 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_put_no_body.py
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_query.py
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_read_with_orm_mode.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_repeated_cookie_headers.py
+-rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_repeated_dependency_schema.py
+-rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_repeated_parameter_alias.py
+-rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_reponse_set_reponse_code_empty.py
+-rw-r--r--   0        0        0     6546 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_request_body_parameters_media_type.py
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_required_noneable.py
+-rw-r--r--   0        0        0    10951 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_response_by_alias.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_response_change_status_code.py
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_response_class_no_mediatype.py
+-rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_response_code_no_body.py
+-rw-r--r--   0        0        0    48457 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_response_model_as_return_annotation.py
+-rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_response_model_include_exclude.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_response_model_invalid.py
+-rw-r--r--   0        0        0     5379 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_response_model_sub_types.py
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_route_scope.py
+-rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_router_events.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_router_prefix_with_template.py
+-rw-r--r--   0        0        0    33384 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_schema_extra_examples.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_security_api_key_cookie.py
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_security_api_key_cookie_description.py
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_security_api_key_cookie_optional.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_security_api_key_header.py
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_security_api_key_header_description.py
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_security_api_key_header_optional.py
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_security_api_key_query.py
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_security_api_key_query_description.py
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_security_api_key_query_optional.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_security_http_base.py
+-rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_security_http_base_description.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_security_http_base_optional.py
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_security_http_basic_optional.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_security_http_basic_realm.py
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_security_http_basic_realm_description.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_security_http_bearer.py
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_security_http_bearer_description.py
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_security_http_bearer_optional.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_security_http_digest.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_security_http_digest_description.py
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_security_http_digest_optional.py
+-rw-r--r--   0        0        0     8340 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_security_oauth2.py
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_security_oauth2_authorization_code_bearer.py
+-rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_security_oauth2_authorization_code_bearer_description.py
+-rw-r--r--   0        0        0     8387 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_security_oauth2_optional.py
+-rw-r--r--   0        0        0     8490 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_security_oauth2_optional_description.py
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_security_oauth2_password_bearer_optional.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_security_oauth2_password_bearer_optional_description.py
+-rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_security_openid_connect.py
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_security_openid_connect_description.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_security_openid_connect_optional.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_serialize_response.py
+-rw-r--r--   0        0        0     4998 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_serialize_response_dataclass.py
+-rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_serialize_response_model.py
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_skip_defaults.py
+-rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_starlette_exception.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_starlette_urlconvertors.py
+-rw-r--r--   0        0        0    12779 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_sub_callbacks.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_swagger_ui_init_oauth.py
+-rw-r--r--   0        0        0     9847 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tuples.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_typing_python39.py
+-rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_union_body.py
+-rw-r--r--   0        0        0     4465 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_union_inherited_body.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_validate_response.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_validate_response_dataclass.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_validate_response_recursive.py
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_ws_dependencies.py
+-rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_ws_router.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_modules_same_name_body/__init__.py
+-rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_modules_same_name_body/test_main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_modules_same_name_body/app/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_modules_same_name_body/app/a.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_modules_same_name_body/app/b.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_modules_same_name_body/app/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_additional_responses/__init__.py
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_additional_responses/test_tutorial001.py
+-rw-r--r--   0        0        0     4288 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_additional_responses/test_tutorial002.py
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_additional_responses/test_tutorial003.py
+-rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_additional_responses/test_tutorial004.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_additional_status_codes/__init__.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_advanced_middleware/__init__.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_advanced_middleware/test_tutorial001.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_advanced_middleware/test_tutorial002.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_advanced_middleware/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_async_sql_databases/__init__.py
+-rw-r--r--   0        0        0     5833 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_async_sql_databases/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_async_tests/__init__.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_async_tests/test_main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_background_tasks/__init__.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_background_tasks/test_tutorial001.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_background_tasks/test_tutorial002.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_background_tasks/test_tutorial002_an.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py310.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py39.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_background_tasks/test_tutorial002_py310.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_behind_a_proxy/__init__.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_behind_a_proxy/test_tutorial001.py
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_behind_a_proxy/test_tutorial002.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_behind_a_proxy/test_tutorial003.py
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_behind_a_proxy/test_tutorial004.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_bigger_applications/__init__.py
+-rw-r--r--   0        0        0    18714 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_bigger_applications/test_main.py
+-rw-r--r--   0        0        0    18717 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_bigger_applications/test_main_an.py
+-rw-r--r--   0        0        0    19078 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_bigger_applications/test_main_an_py39.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_body/__init__.py
+-rw-r--r--   0        0        0     8723 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_body/test_tutorial001.py
+-rw-r--r--   0        0        0     9101 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_body/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_body_fields/__init__.py
+-rw-r--r--   0        0        0     5961 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_body_fields/test_tutorial001.py
+-rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_body_fields/test_tutorial001_an.py
+-rw-r--r--   0        0        0     6144 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_body_fields/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_body_fields/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_body_fields/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_body_multiple_params/__init__.py
+-rw-r--r--   0        0        0     5239 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001.py
+-rw-r--r--   0        0        0     5242 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an.py
+-rw-r--r--   0        0        0     5422 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     5418 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     5419 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001_py310.py
+-rw-r--r--   0        0        0     7217 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003.py
+-rw-r--r--   0        0        0     7220 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an.py
+-rw-r--r--   0        0        0     7400 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py310.py
+-rw-r--r--   0        0        0     7396 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py39.py
+-rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003_py310.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_body_nested_models/__init__.py
+-rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_body_nested_models/test_tutorial009.py
+-rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_body_nested_models/test_tutorial009_py39.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_body_updates/__init__.py
+-rw-r--r--   0        0        0     6030 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_body_updates/test_tutorial001.py
+-rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_body_updates/test_tutorial001_py310.py
+-rw-r--r--   0        0        0     6248 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_body_updates/test_tutorial001_py39.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_conditional_openapi/__init__.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_conditional_openapi/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_cookie_params/__init__.py
+-rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_cookie_params/test_tutorial001.py
+-rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_cookie_params/test_tutorial001_an.py
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_cookie_params/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_cors/__init__.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_cors/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_custom_request_and_route/__init__.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_custom_request_and_route/test_tutorial001.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_custom_request_and_route/test_tutorial002.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_custom_request_and_route/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_custom_response/__init__.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_custom_response/test_tutorial001.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_custom_response/test_tutorial001b.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_custom_response/test_tutorial004.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_custom_response/test_tutorial005.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_custom_response/test_tutorial006.py
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_custom_response/test_tutorial006b.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_custom_response/test_tutorial006c.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_custom_response/test_tutorial007.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_custom_response/test_tutorial008.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_custom_response/test_tutorial009.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_custom_response/test_tutorial009b.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_custom_response/test_tutorial009c.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_dataclasses/__init__.py
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_dataclasses/test_tutorial001.py
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_dataclasses/test_tutorial002.py
+-rw-r--r--   0        0        0     6783 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_dataclasses/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_dependencies/__init__.py
+-rw-r--r--   0        0        0     6353 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_dependencies/test_tutorial001.py
+-rw-r--r--   0        0        0     6356 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_dependencies/test_tutorial001_an.py
+-rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_dependencies/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     6532 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_dependencies/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     6533 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_dependencies/test_tutorial001_py310.py
+-rw-r--r--   0        0        0     5102 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_dependencies/test_tutorial004.py
+-rw-r--r--   0        0        0     5105 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_dependencies/test_tutorial004_an.py
+-rw-r--r--   0        0        0     5285 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_dependencies/test_tutorial004_an_py310.py
+-rw-r--r--   0        0        0     5281 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_dependencies/test_tutorial004_an_py39.py
+-rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_dependencies/test_tutorial004_py310.py
+-rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_dependencies/test_tutorial006.py
+-rw-r--r--   0        0        0     4480 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_dependencies/test_tutorial006_an.py
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_dependencies/test_tutorial006_an_py39.py
+-rw-r--r--   0        0        0     7386 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_dependencies/test_tutorial012.py
+-rw-r--r--   0        0        0     7389 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_dependencies/test_tutorial012_an.py
+-rw-r--r--   0        0        0     7787 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_dependencies/test_tutorial012_an_py39.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_events/__init__.py
+-rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_events/test_tutorial001.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_events/test_tutorial002.py
+-rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_events/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_extending_openapi/__init__.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_extending_openapi/test_tutorial001.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_extending_openapi/test_tutorial002.py
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_extending_openapi/test_tutorial003.py
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_extending_openapi/test_tutorial004.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_extending_openapi/test_tutorial005.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_extra_data_types/__init__.py
+-rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_extra_data_types/test_tutorial001.py
+-rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_extra_data_types/test_tutorial001_an.py
+-rw-r--r--   0        0        0     5368 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     5364 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     5365 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_extra_data_types/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_extra_models/__init__.py
+-rw-r--r--   0        0        0     4808 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_extra_models/test_tutorial003.py
+-rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_extra_models/test_tutorial003_py310.py
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_extra_models/test_tutorial004.py
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_extra_models/test_tutorial004_py39.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_extra_models/test_tutorial005.py
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_extra_models/test_tutorial005_py39.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_first_steps/__init__.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_first_steps/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_generate_clients/__init__.py
+-rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_generate_clients/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_handling_errors/__init__.py
+-rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_handling_errors/test_tutorial001.py
+-rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_handling_errors/test_tutorial002.py
+-rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_handling_errors/test_tutorial003.py
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_handling_errors/test_tutorial004.py
+-rw-r--r--   0        0        0     3899 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_handling_errors/test_tutorial005.py
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_handling_errors/test_tutorial006.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_header_params/__init__.py
+-rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_header_params/test_tutorial001.py
+-rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_header_params/test_tutorial001_an.py
+-rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_header_params/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_header_params/test_tutorial001_py310.py
+-rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_header_params/test_tutorial002.py
+-rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_header_params/test_tutorial002_an.py
+-rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_header_params/test_tutorial002_an_py310.py
+-rw-r--r--   0        0        0     3887 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_header_params/test_tutorial002_an_py39.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_header_params/test_tutorial002_py310.py
+-rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_header_params/test_tutorial003.py
+-rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_header_params/test_tutorial003_an.py
+-rw-r--r--   0        0        0     3824 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_header_params/test_tutorial003_an_py310.py
+-rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_header_params/test_tutorial003_an_py39.py
+-rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_header_params/test_tutorial003_py310.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_metadata/__init__.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_metadata/test_tutorial001.py
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_metadata/test_tutorial004.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_openapi_callbacks/__init__.py
+-rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_openapi_callbacks/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_path_operation_advanced_configurations/__init__.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial001.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial002.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial003.py
+-rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial004.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial005.py
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial006.py
+-rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial007.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_path_operation_configurations/__init__.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial002b.py
+-rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial005.py
+-rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py310.py
+-rw-r--r--   0        0        0     4682 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py39.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial006.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_path_params/__init__.py
+-rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_path_params/test_tutorial004.py
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_path_params/test_tutorial005.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_query_params/__init__.py
+-rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_query_params/test_tutorial005.py
+-rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_query_params/test_tutorial006.py
+-rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_query_params/test_tutorial006_py310.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/__init__.py
+-rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010.py
+-rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an.py
+-rw-r--r--   0        0        0     4691 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py310.py
+-rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py39.py
+-rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_py310.py
+-rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011.py
+-rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an.py
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py310.py
+-rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py39.py
+-rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py310.py
+-rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py39.py
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial012.py
+-rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an.py
+-rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an_py39.py
+-rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_py39.py
+-rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial013.py
+-rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an.py
+-rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an_py39.py
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014.py
+-rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py310.py
+-rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py39.py
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_py310.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_request_files/__init__.py
+-rw-r--r--   0        0        0     6732 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_request_files/test_tutorial001.py
+-rw-r--r--   0        0        0     5984 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_request_files/test_tutorial001_02.py
+-rw-r--r--   0        0        0     5987 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_request_files/test_tutorial001_02_an.py
+-rw-r--r--   0        0        0     6256 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py310.py
+-rw-r--r--   0        0        0     6249 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py39.py
+-rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_request_files/test_tutorial001_02_py310.py
+-rw-r--r--   0        0        0     6133 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_request_files/test_tutorial001_03.py
+-rw-r--r--   0        0        0     6136 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_request_files/test_tutorial001_03_an.py
+-rw-r--r--   0        0        0     6300 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_request_files/test_tutorial001_03_an_py39.py
+-rw-r--r--   0        0        0     6735 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_request_files/test_tutorial001_an.py
+-rw-r--r--   0        0        0     6962 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_request_files/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     7703 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_request_files/test_tutorial002.py
+-rw-r--r--   0        0        0     7706 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_request_files/test_tutorial002_an.py
+-rw-r--r--   0        0        0     8100 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_request_files/test_tutorial002_an_py39.py
+-rw-r--r--   0        0        0     8097 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_request_files/test_tutorial002_py39.py
+-rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_request_files/test_tutorial003.py
+-rw-r--r--   0        0        0     7314 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_request_files/test_tutorial003_an.py
+-rw-r--r--   0        0        0     7830 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_request_files/test_tutorial003_an_py39.py
+-rw-r--r--   0        0        0     7827 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_request_files/test_tutorial003_py39.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_request_forms/__init__.py
+-rw-r--r--   0        0        0     5013 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_request_forms/test_tutorial001.py
+-rw-r--r--   0        0        0     5016 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_request_forms/test_tutorial001_an.py
+-rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_request_forms/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_request_forms_and_files/__init__.py
+-rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_request_forms_and_files/test_tutorial001.py
+-rw-r--r--   0        0        0     6418 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an.py
+-rw-r--r--   0        0        0     6818 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_response_change_status_code/__init__.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_response_change_status_code/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_response_cookies/__init__.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_response_cookies/test_tutorial001.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_response_cookies/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_response_headers/__init__.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_response_headers/test_tutorial001.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_response_headers/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_response_model/__init__.py
+-rw-r--r--   0        0        0     4761 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_response_model/test_tutorial003.py
+-rw-r--r--   0        0        0     4767 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_response_model/test_tutorial003_01.py
+-rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_response_model/test_tutorial003_01_py310.py
+-rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_response_model/test_tutorial003_02.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_response_model/test_tutorial003_03.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_response_model/test_tutorial003_04.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_response_model/test_tutorial003_04_py310.py
+-rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_response_model/test_tutorial003_05.py
+-rw-r--r--   0        0        0     3699 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_response_model/test_tutorial003_05_py310.py
+-rw-r--r--   0        0        0     4953 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_response_model/test_tutorial003_py310.py
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_response_model/test_tutorial004.py
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_response_model/test_tutorial004_py310.py
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_response_model/test_tutorial004_py39.py
+-rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_response_model/test_tutorial005.py
+-rw-r--r--   0        0        0     5756 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_response_model/test_tutorial005_py310.py
+-rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_response_model/test_tutorial006.py
+-rw-r--r--   0        0        0     5756 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_response_model/test_tutorial006_py310.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_schema_extra_example/__init__.py
+-rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004.py
+-rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an.py
+-rw-r--r--   0        0        0     5754 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py310.py
+-rw-r--r--   0        0        0     5750 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py39.py
+-rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004_py310.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_security/__init__.py
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_security/test_tutorial001.py
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_security/test_tutorial001_an.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_security/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     6832 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_security/test_tutorial003.py
+-rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_security/test_tutorial003_an.py
+-rw-r--r--   0        0        0     7244 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_security/test_tutorial003_an_py310.py
+-rw-r--r--   0        0        0     7233 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_security/test_tutorial003_an_py39.py
+-rw-r--r--   0        0        0     7241 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_security/test_tutorial003_py310.py
+-rw-r--r--   0        0        0    13084 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_security/test_tutorial005.py
+-rw-r--r--   0        0        0    13087 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_security/test_tutorial005_an.py
+-rw-r--r--   0        0        0    13992 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_security/test_tutorial005_an_py310.py
+-rw-r--r--   0        0        0    13968 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_security/test_tutorial005_an_py39.py
+-rw-r--r--   0        0        0    13980 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_security/test_tutorial005_py310.py
+-rw-r--r--   0        0        0    13956 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_security/test_tutorial005_py39.py
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_security/test_tutorial006.py
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_security/test_tutorial006_an.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_security/test_tutorial006_an_py39.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_settings/__init__.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_settings/test_app02.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_sql_databases/__init__.py
+-rw-r--r--   0        0        0    15205 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_sql_databases/test_sql_databases.py
+-rw-r--r--   0        0        0    15384 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware.py
+-rw-r--r--   0        0        0    15675 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py310.py
+-rw-r--r--   0        0        0    15666 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py39.py
+-rw-r--r--   0        0        0    15681 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_sql_databases/test_sql_databases_py310.py
+-rw-r--r--   0        0        0    15672 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_sql_databases/test_sql_databases_py39.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_sql_databases/test_testing_databases.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_sql_databases/test_testing_databases_py310.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_sql_databases/test_testing_databases_py39.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_sql_databases_peewee/__init__.py
+-rw-r--r--   0        0        0    17654 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_sql_databases_peewee/test_sql_databases_peewee.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_sub_applications/__init__.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_sub_applications/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_templates/__init__.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_templates/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_testing/__init__.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_testing/test_main.py
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_testing/test_main_b.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_testing/test_main_b_an.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_testing/test_main_b_an_py310.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_testing/test_main_b_an_py39.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_testing/test_main_b_py310.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_testing/test_tutorial001.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_testing/test_tutorial002.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_testing/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_testing_dependencies/__init__.py
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001.py
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an.py
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_websockets/__init__.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_websockets/test_tutorial001.py
+-rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_websockets/test_tutorial002.py
+-rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_websockets/test_tutorial002_an.py
+-rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_websockets/test_tutorial002_an_py310.py
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_websockets/test_tutorial002_an_py39.py
+-rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_websockets/test_tutorial002_py310.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_websockets/test_tutorial003.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_websockets/test_tutorial003_py39.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_wsgi/__init__.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 fastapi-0.97.0/tests/test_tutorial/test_wsgi/test_tutorial001.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 fastapi-0.97.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 fastapi-0.97.0/LICENSE
+-rw-r--r--   0        0        0    20788 2020-02-02 00:00:00.000000 fastapi-0.97.0/README.md
+-rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 fastapi-0.97.0/pyproject.toml
+-rw-r--r--   0        0        0    23107 2020-02-02 00:00:00.000000 fastapi-0.97.0/PKG-INFO
```

### Comparing `fastapi-0.96.1/.pre-commit-config.yaml` & `fastapi-0.97.0/.pre-commit-config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -17,30 +17,19 @@
     rev: v3.3.1
     hooks:
     -   id: pyupgrade
         args:
         - --py3-plus
         - --keep-runtime-typing
 -   repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.254
+    rev: v0.0.272
     hooks:
     -   id: ruff
         args:
         - --fix
--   repo: https://github.com/pycqa/isort
-    rev: 5.12.0
-    hooks:
-    -   id: isort
-        name: isort (python)
-    -   id: isort
-        name: isort (cython)
-        types: [cython]
-    -   id: isort
-        name: isort (pyi)
-        types: [pyi]
 -   repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
     -   id: black
 ci:
     autofix_commit_msg: 🎨 [pre-commit.ci] Auto format from pre-commit.com hooks
     autoupdate_commit_msg: ⬆ [pre-commit.ci] pre-commit autoupdate
```

### Comparing `fastapi-0.96.1/SECURITY.md` & `fastapi-0.97.0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/.github/DISCUSSION_TEMPLATE/questions.yml` & `fastapi-0.97.0/.github/DISCUSSION_TEMPLATE/questions.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/.github/ISSUE_TEMPLATE/config.yml` & `fastapi-0.97.0/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/.github/ISSUE_TEMPLATE/privileged.yml` & `fastapi-0.97.0/.github/ISSUE_TEMPLATE/privileged.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/.github/actions/comment-docs-preview-in-pr/app/main.py` & `fastapi-0.97.0/.github/actions/comment-docs-preview-in-pr/app/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/.github/actions/notify-translations/app/main.py` & `fastapi-0.97.0/.github/actions/notify-translations/app/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/.github/actions/people/app/main.py` & `fastapi-0.97.0/.github/actions/people/app/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/.github/actions/watch-previews/app/main.py` & `fastapi-0.97.0/.github/actions/watch-previews/app/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/.github/workflows/build-docs.yml` & `fastapi-0.97.0/.github/workflows/build-docs.yml`

 * *Files 11% similar despite different names*

```diff
@@ -18,18 +18,18 @@
         uses: actions/setup-python@v4
         with:
           python-version: "3.11"
       - uses: actions/cache@v3
         id: cache
         with:
           path: ${{ env.pythonLocation }}
-          key: ${{ runner.os }}-python-docs-${{ env.pythonLocation }}-${{ hashFiles('pyproject.toml') }}-v03
+          key: ${{ runner.os }}-python-docs-${{ env.pythonLocation }}-${{ hashFiles('pyproject.toml', 'requirements-docs.txt') }}-v03
       - name: Install docs extras
         if: steps.cache.outputs.cache-hit != 'true'
-        run: pip install .[doc]
+        run: pip install -r requirements-docs.txt
       - name: Install Material for MkDocs Insiders
         if: ( github.event_name != 'pull_request' || github.event.pull_request.head.repo.fork == false ) && steps.cache.outputs.cache-hit != 'true'
         run: pip install git+https://${{ secrets.ACTIONS_TOKEN }}@github.com/squidfunk/mkdocs-material-insiders.git
       - name: Build Docs
         run: python ./scripts/docs.py build-all
       - name: Zip docs
         run: bash ./scripts/zip-docs.sh
```

### Comparing `fastapi-0.96.1/.github/workflows/issue-manager.yml` & `fastapi-0.97.0/.github/workflows/issue-manager.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/.github/workflows/latest-changes.yml` & `fastapi-0.97.0/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/.github/workflows/notify-translations.yml` & `fastapi-0.97.0/.github/workflows/notify-translations.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/.github/workflows/people.yml` & `fastapi-0.97.0/.github/workflows/people.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/.github/workflows/preview-docs.yml` & `fastapi-0.97.0/.github/workflows/preview-docs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/.github/workflows/publish.yml` & `fastapi-0.97.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/.github/workflows/smokeshow.yml` & `fastapi-0.97.0/.github/workflows/smokeshow.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/.github/workflows/test.yml` & `fastapi-0.97.0/.github/workflows/test.yml`

 * *Files 9% similar despite different names*

```diff
@@ -19,23 +19,23 @@
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
           # Issue ref: https://github.com/actions/setup-python/issues/436
           # cache: "pip"
-          cache-dependency-path: pyproject.toml
+          # cache-dependency-path: pyproject.toml
       - uses: actions/cache@v3
         id: cache
         with:
           path: ${{ env.pythonLocation }}
-          key: ${{ runner.os }}-python-${{ env.pythonLocation }}-${{ hashFiles('pyproject.toml') }}-test-v03
+          key: ${{ runner.os }}-python-${{ env.pythonLocation }}-${{ hashFiles('pyproject.toml', 'requirements-tests.txt') }}-test-v03
       - name: Install Dependencies
         if: steps.cache.outputs.cache-hit != 'true'
-        run: pip install -e .[all,dev,doc,test]
+        run: pip install -r requirements-tests.txt
       - name: Lint
         run: bash scripts/lint.sh
       - run: mkdir coverage
       - name: Test
         run: bash scripts/test.sh
         env:
           COVERAGE_FILE: coverage/.coverage.${{ runner.os }}-py${{ matrix.python-version }}
@@ -53,15 +53,15 @@
       - uses: actions/checkout@v3
 
       - uses: actions/setup-python@v4
         with:
           python-version: '3.8'
           # Issue ref: https://github.com/actions/setup-python/issues/436
           # cache: "pip"
-          cache-dependency-path: pyproject.toml
+          # cache-dependency-path: pyproject.toml
 
       - name: Get coverage files
         uses: actions/download-artifact@v3
         with:
           name: coverage
           path: coverage
```

### Comparing `fastapi-0.96.1/docs/az/mkdocs.yml` & `fastapi-0.97.0/docs/az/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/az/docs/index.md` & `fastapi-0.97.0/docs/az/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/cs/mkdocs.yml` & `fastapi-0.97.0/docs/cs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/cs/docs/index.md` & `fastapi-0.97.0/docs/cs/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/de/mkdocs.yml` & `fastapi-0.97.0/docs/de/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/de/docs/features.md` & `fastapi-0.97.0/docs/de/docs/features.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/de/docs/index.md` & `fastapi-0.97.0/docs/de/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/mkdocs.yml` & `fastapi-0.97.0/docs/em/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/alternatives.md` & `fastapi-0.97.0/docs/em/docs/alternatives.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/async.md` & `fastapi-0.97.0/docs/em/docs/async.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/benchmarks.md` & `fastapi-0.97.0/docs/em/docs/benchmarks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/contributing.md` & `fastapi-0.97.0/docs/em/docs/contributing.md`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 ### 🐖
 
 ⏮️ 🔓 🌐 🔬 🔛:
 
 <div class="termy">
 
 ```console
-$ pip install -e ."[dev,doc,test]"
+$ pip install -r requirements.txt
 
 ---> 100%
 ```
 
 </div>
 
 ⚫️ 🔜 ❎ 🌐 🔗 &amp; 👆 🇧🇿 FastAPI 👆 🇧🇿 🌐.
```

#### html2text {}

```diff
@@ -18,15 +18,15 @@
 ð¥ â«ï¸ ð¦ `pip` ð± `env/bin/pip` â¤´ï¸ â«ï¸ ð·. ð¶ â ð­
 ð âï¸ ð° ð â¬ ð ð ð¹ ð â â ð â­ ð¶:
 ```console $ python -m pip install --upgrade pip ---> 100% ```
 !!! tip ð  ð° ð â ð ð¦ â®ï¸ `pip` ð½ ð ð, ð ð
 ð. ð â ð­ ð ð¥ ð âï¸ ð¶ ð â ð ð¦, ð âï¸
 1ï¸â£ âªï¸â¡ï¸ ð ð§ð¿ ð & ð« ð ð ð ðª â ð.
 ### ð â®ï¸ ð ð ð¬ ð:
-```console $ pip install -e ."[dev,doc,test]" ---> 100% ```
+```console $ pip install -r requirements.txt ---> 100% ```
 â«ï¸ ð â ð ð & ð ð§ð¿ FastAPI ð ð§ð¿ ð. ####
 âï¸ ð ð§ð¿ FastAPI ð¥ ð â ð ð ð ð & âï¸
 FastAPI, & ð â«ï¸ â®ï¸ ð âªï¸â¡ï¸ ð ð§ð¿ ð, â«ï¸ ð
 âï¸ ð ð§ð¿ FastAPI â¹ ð. & ð¥ ð â¹ ð ð§ð¿ FastAPI
 â¹ ð, â«ï¸ â â®ï¸ `-e`, ðâ ð ð ð ð ð ð, â«ï¸
 ð âï¸ ð â¬ FastAPI ð â. ð ð, ð ð« âï¸ "â" ð
 ð§ð¿ â¬ ðª ð¯ ð  ð. ### ð ð¤ â ð ð ðª ð ð
```

### Comparing `fastapi-0.96.1/docs/em/docs/external-links.md` & `fastapi-0.97.0/docs/em/docs/external-links.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/fastapi-people.md` & `fastapi-0.97.0/docs/em/docs/fastapi-people.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/features.md` & `fastapi-0.97.0/docs/em/docs/features.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/help-fastapi.md` & `fastapi-0.97.0/docs/em/docs/help-fastapi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/history-design-future.md` & `fastapi-0.97.0/docs/em/docs/history-design-future.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/index.md` & `fastapi-0.97.0/docs/em/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/project-generation.md` & `fastapi-0.97.0/docs/em/docs/project-generation.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/python-types.md` & `fastapi-0.97.0/docs/em/docs/python-types.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/advanced/additional-responses.md` & `fastapi-0.97.0/docs/em/docs/advanced/additional-responses.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/advanced/additional-status-codes.md` & `fastapi-0.97.0/docs/em/docs/advanced/additional-status-codes.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/advanced/advanced-dependencies.md` & `fastapi-0.97.0/docs/em/docs/advanced/advanced-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/advanced/async-sql-databases.md` & `fastapi-0.97.0/docs/em/docs/advanced/async-sql-databases.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/advanced/async-tests.md` & `fastapi-0.97.0/docs/em/docs/advanced/async-tests.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/advanced/behind-a-proxy.md` & `fastapi-0.97.0/docs/em/docs/advanced/behind-a-proxy.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/advanced/conditional-openapi.md` & `fastapi-0.97.0/docs/em/docs/advanced/conditional-openapi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/advanced/custom-request-and-route.md` & `fastapi-0.97.0/docs/em/docs/advanced/custom-request-and-route.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/advanced/custom-response.md` & `fastapi-0.97.0/docs/em/docs/advanced/custom-response.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/advanced/dataclasses.md` & `fastapi-0.97.0/docs/em/docs/advanced/dataclasses.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/advanced/events.md` & `fastapi-0.97.0/docs/em/docs/advanced/events.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/advanced/extending-openapi.md` & `fastapi-0.97.0/docs/em/docs/advanced/extending-openapi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/advanced/generate-clients.md` & `fastapi-0.97.0/docs/em/docs/advanced/generate-clients.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/advanced/graphql.md` & `fastapi-0.97.0/docs/em/docs/advanced/graphql.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/advanced/index.md` & `fastapi-0.97.0/docs/em/docs/advanced/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/advanced/middleware.md` & `fastapi-0.97.0/docs/em/docs/advanced/middleware.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/advanced/nosql-databases.md` & `fastapi-0.97.0/docs/em/docs/advanced/nosql-databases.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/advanced/openapi-callbacks.md` & `fastapi-0.97.0/docs/em/docs/advanced/openapi-callbacks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/advanced/path-operation-advanced-configuration.md` & `fastapi-0.97.0/docs/em/docs/advanced/path-operation-advanced-configuration.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/advanced/response-change-status-code.md` & `fastapi-0.97.0/docs/em/docs/advanced/response-change-status-code.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/advanced/response-cookies.md` & `fastapi-0.97.0/docs/em/docs/advanced/response-cookies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/advanced/response-directly.md` & `fastapi-0.97.0/docs/em/docs/advanced/response-directly.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/advanced/response-headers.md` & `fastapi-0.97.0/docs/em/docs/advanced/response-headers.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/advanced/settings.md` & `fastapi-0.97.0/docs/em/docs/advanced/settings.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/advanced/sql-databases-peewee.md` & `fastapi-0.97.0/docs/em/docs/advanced/sql-databases-peewee.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/advanced/sub-applications.md` & `fastapi-0.97.0/docs/em/docs/advanced/sub-applications.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/advanced/templates.md` & `fastapi-0.97.0/docs/em/docs/advanced/templates.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/advanced/testing-database.md` & `fastapi-0.97.0/docs/em/docs/advanced/testing-database.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/advanced/testing-dependencies.md` & `fastapi-0.97.0/docs/em/docs/advanced/testing-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/advanced/using-request-directly.md` & `fastapi-0.97.0/docs/em/docs/advanced/using-request-directly.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/advanced/websockets.md` & `fastapi-0.97.0/docs/em/docs/advanced/websockets.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/advanced/wsgi.md` & `fastapi-0.97.0/docs/em/docs/advanced/wsgi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/advanced/security/http-basic-auth.md` & `fastapi-0.97.0/docs/em/docs/advanced/security/http-basic-auth.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/advanced/security/oauth2-scopes.md` & `fastapi-0.97.0/docs/em/docs/advanced/security/oauth2-scopes.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/deployment/concepts.md` & `fastapi-0.97.0/docs/em/docs/deployment/concepts.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/deployment/deta.md` & `fastapi-0.97.0/docs/em/docs/deployment/deta.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/deployment/docker.md` & `fastapi-0.97.0/docs/em/docs/deployment/docker.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/deployment/https.md` & `fastapi-0.97.0/docs/em/docs/deployment/https.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/deployment/index.md` & `fastapi-0.97.0/docs/em/docs/deployment/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/deployment/manually.md` & `fastapi-0.97.0/docs/em/docs/deployment/manually.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/deployment/server-workers.md` & `fastapi-0.97.0/docs/em/docs/deployment/server-workers.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/deployment/versions.md` & `fastapi-0.97.0/docs/em/docs/deployment/versions.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/background-tasks.md` & `fastapi-0.97.0/docs/em/docs/tutorial/background-tasks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/bigger-applications.md` & `fastapi-0.97.0/docs/em/docs/tutorial/bigger-applications.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/body-fields.md` & `fastapi-0.97.0/docs/em/docs/tutorial/body-fields.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/body-multiple-params.md` & `fastapi-0.97.0/docs/em/docs/tutorial/body-multiple-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/body-nested-models.md` & `fastapi-0.97.0/docs/em/docs/tutorial/body-nested-models.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/body-updates.md` & `fastapi-0.97.0/docs/em/docs/tutorial/body-updates.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/body.md` & `fastapi-0.97.0/docs/em/docs/tutorial/body.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/cookie-params.md` & `fastapi-0.97.0/docs/em/docs/tutorial/cookie-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/cors.md` & `fastapi-0.97.0/docs/em/docs/tutorial/cors.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/debugging.md` & `fastapi-0.97.0/docs/em/docs/tutorial/debugging.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/encoder.md` & `fastapi-0.97.0/docs/em/docs/tutorial/encoder.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/extra-data-types.md` & `fastapi-0.97.0/docs/em/docs/tutorial/extra-data-types.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/extra-models.md` & `fastapi-0.97.0/docs/em/docs/tutorial/extra-models.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/first-steps.md` & `fastapi-0.97.0/docs/em/docs/tutorial/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/handling-errors.md` & `fastapi-0.97.0/docs/em/docs/tutorial/handling-errors.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/header-params.md` & `fastapi-0.97.0/docs/em/docs/tutorial/header-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/index.md` & `fastapi-0.97.0/docs/em/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/metadata.md` & `fastapi-0.97.0/docs/em/docs/tutorial/metadata.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/middleware.md` & `fastapi-0.97.0/docs/em/docs/tutorial/middleware.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/path-operation-configuration.md` & `fastapi-0.97.0/docs/em/docs/tutorial/path-operation-configuration.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/path-params-numeric-validations.md` & `fastapi-0.97.0/docs/em/docs/tutorial/path-params-numeric-validations.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/path-params.md` & `fastapi-0.97.0/docs/em/docs/tutorial/path-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/query-params-str-validations.md` & `fastapi-0.97.0/docs/em/docs/tutorial/query-params-str-validations.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/query-params.md` & `fastapi-0.97.0/docs/em/docs/tutorial/query-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/request-files.md` & `fastapi-0.97.0/docs/em/docs/tutorial/request-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/request-forms-and-files.md` & `fastapi-0.97.0/docs/em/docs/tutorial/request-forms-and-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/request-forms.md` & `fastapi-0.97.0/docs/em/docs/tutorial/request-forms.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/response-model.md` & `fastapi-0.97.0/docs/em/docs/tutorial/response-model.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/response-status-code.md` & `fastapi-0.97.0/docs/em/docs/tutorial/response-status-code.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/schema-extra-example.md` & `fastapi-0.97.0/docs/em/docs/tutorial/schema-extra-example.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/sql-databases.md` & `fastapi-0.97.0/docs/em/docs/tutorial/sql-databases.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/static-files.md` & `fastapi-0.97.0/docs/em/docs/tutorial/static-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/testing.md` & `fastapi-0.97.0/docs/em/docs/tutorial/testing.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/dependencies/classes-as-dependencies.md` & `fastapi-0.97.0/docs/em/docs/tutorial/dependencies/classes-as-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/dependencies/dependencies-in-path-operation-decorators.md` & `fastapi-0.97.0/docs/em/docs/tutorial/dependencies/dependencies-in-path-operation-decorators.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/dependencies/dependencies-with-yield.md` & `fastapi-0.97.0/docs/em/docs/tutorial/dependencies/dependencies-with-yield.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/dependencies/global-dependencies.md` & `fastapi-0.97.0/docs/em/docs/tutorial/dependencies/global-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/dependencies/index.md` & `fastapi-0.97.0/docs/em/docs/tutorial/dependencies/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/dependencies/sub-dependencies.md` & `fastapi-0.97.0/docs/em/docs/tutorial/dependencies/sub-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/security/first-steps.md` & `fastapi-0.97.0/docs/em/docs/tutorial/security/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/security/get-current-user.md` & `fastapi-0.97.0/docs/em/docs/tutorial/security/get-current-user.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/security/index.md` & `fastapi-0.97.0/docs/em/docs/tutorial/security/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/security/oauth2-jwt.md` & `fastapi-0.97.0/docs/em/docs/tutorial/security/oauth2-jwt.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/em/docs/tutorial/security/simple-oauth2.md` & `fastapi-0.97.0/docs/em/docs/tutorial/security/simple-oauth2.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/mkdocs.yml` & `fastapi-0.97.0/docs/en/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/data/external_links.yml` & `fastapi-0.97.0/docs/en/data/external_links.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/data/github_sponsors.yml` & `fastapi-0.97.0/docs/en/data/github_sponsors.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/data/people.yml` & `fastapi-0.97.0/docs/en/data/people.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/data/sponsors.yml` & `fastapi-0.97.0/docs/en/data/sponsors.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/alternatives.md` & `fastapi-0.97.0/docs/en/docs/alternatives.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/async.md` & `fastapi-0.97.0/docs/en/docs/async.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/benchmarks.md` & `fastapi-0.97.0/docs/en/docs/benchmarks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/contributing.md` & `fastapi-0.97.0/docs/en/docs/contributing.md`

 * *Files 2% similar despite different names*

```diff
@@ -104,31 +104,36 @@
 ### pip
 
 After activating the environment as described above:
 
 <div class="termy">
 
 ```console
-$ pip install -e ".[dev,doc,test]"
+$ pip install -r requirements.txt
 
 ---> 100%
 ```
 
 </div>
 
 It will install all the dependencies and your local FastAPI in your local environment.
 
 #### Using your local FastAPI
 
 If you create a Python file that imports and uses FastAPI, and run it with the Python from your local environment, it will use your local FastAPI source code.
 
-And if you update that local FastAPI source code, as it is installed with `-e`, when you run that Python file again, it will use the fresh version of FastAPI you just edited.
+And if you update that local FastAPI source code when you run that Python file again, it will use the fresh version of FastAPI you just edited.
 
 That way, you don't have to "install" your local version to be able to test every change.
 
+!!! note "Technical Details"
+    This only happens when you install using this included `requiements.txt` instead of installing `pip install fastapi` directly.
+
+    That is because inside of the `requirements.txt` file, the local version of FastAPI is marked to be installed in "editable" mode, with the `-e` option.
+
 ### Format
 
 There is a script that you can run that will format and clean all your code:
 
 <div class="termy">
 
 ```console
```

#### html2text {}

```diff
@@ -22,24 +22,27 @@
 the next steps:
 ```console $ python -m pip install --upgrade pip ---> 100% ```
 !!! tip Every time you install a new package with `pip` under that environment,
 activate the environment again. This makes sure that if you use a terminal
 program installed by that package, you use the one from your local environment
 and not any other that could be installed globally. ### pip After activating
 the environment as described above:
-```console $ pip install -e ".[dev,doc,test]" ---> 100% ```
+```console $ pip install -r requirements.txt ---> 100% ```
 It will install all the dependencies and your local FastAPI in your local
 environment. #### Using your local FastAPI If you create a Python file that
 imports and uses FastAPI, and run it with the Python from your local
 environment, it will use your local FastAPI source code. And if you update that
-local FastAPI source code, as it is installed with `-e`, when you run that
-Python file again, it will use the fresh version of FastAPI you just edited.
-That way, you don't have to "install" your local version to be able to test
-every change. ### Format There is a script that you can run that will format
-and clean all your code:
+local FastAPI source code when you run that Python file again, it will use the
+fresh version of FastAPI you just edited. That way, you don't have to "install"
+your local version to be able to test every change. !!! note "Technical
+Details" This only happens when you install using this included
+`requiements.txt` instead of installing `pip install fastapi` directly. That is
+because inside of the `requirements.txt` file, the local version of FastAPI is
+marked to be installed in "editable" mode, with the `-e` option. ### Format
+There is a script that you can run that will format and clean all your code:
 ```console $ bash scripts/format.sh ```
 It will also auto-sort all your imports. For it to sort them correctly, you
 need to have FastAPI installed locally in your environment, with the command in
 the section above using `-e`. ## Docs First, make sure you set up your
 environment as described above, that will install all the requirements. The
 documentation uses MkDocs. And there are extra tools/scripts in place to handle
 translations in `./scripts/docs.py`. !!! tip You don't need to see the code in
```

### Comparing `fastapi-0.96.1/docs/en/docs/external-links.md` & `fastapi-0.97.0/docs/en/docs/external-links.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/fastapi-people.md` & `fastapi-0.97.0/docs/en/docs/fastapi-people.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/features.md` & `fastapi-0.97.0/docs/en/docs/features.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/help-fastapi.md` & `fastapi-0.97.0/docs/en/docs/help-fastapi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/history-design-future.md` & `fastapi-0.97.0/docs/en/docs/history-design-future.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/index.md` & `fastapi-0.97.0/docs/en/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/project-generation.md` & `fastapi-0.97.0/docs/en/docs/project-generation.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/python-types.md` & `fastapi-0.97.0/docs/en/docs/python-types.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/release-notes.md` & `fastapi-0.97.0/docs/en/docs/release-notes.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,41 +1,66 @@
 # Release Notes
 
 ## Latest Changes
 
 
+## 0.97.0
+
+### Features
+
+* ✨ Add support for `dependencies` in WebSocket routes. PR [#4534](https://github.com/tiangolo/fastapi/pull/4534) by [@paulo-raca](https://github.com/paulo-raca).
+* ✨ Add exception handler for `WebSocketRequestValidationError` (which also allows to override it). PR [#6030](https://github.com/tiangolo/fastapi/pull/6030) by [@kristjanvalur](https://github.com/kristjanvalur).
+
+### Refactors
+
+* ⬆️ Upgrade and fully migrate to Ruff, remove isort, includes a couple of tweaks suggested by the new version of Ruff. PR [#9660](https://github.com/tiangolo/fastapi/pull/9660) by [@tiangolo](https://github.com/tiangolo).
+* ♻️ Update internal type annotations and upgrade mypy. PR [#9658](https://github.com/tiangolo/fastapi/pull/9658) by [@tiangolo](https://github.com/tiangolo).
+* ♻️ Simplify `AsyncExitStackMiddleware` as without Python 3.6 `AsyncExitStack` is always available. PR [#9657](https://github.com/tiangolo/fastapi/pull/9657) by [@tiangolo](https://github.com/tiangolo).
+
+### Upgrades
+
+* ⬆️ Upgrade Black. PR [#9661](https://github.com/tiangolo/fastapi/pull/9661) by [@tiangolo](https://github.com/tiangolo).
+
+### Internal
+
+* 💚 Update CI cache to fix installs when dependencies change. PR [#9659](https://github.com/tiangolo/fastapi/pull/9659) by [@tiangolo](https://github.com/tiangolo).
+* ⬇️ Separate requirements for development into their own requirements.txt files, they shouldn't be extras. PR [#9655](https://github.com/tiangolo/fastapi/pull/9655) by [@tiangolo](https://github.com/tiangolo).
+
 ## 0.96.1
 
 ### Fixes
 
 * 🐛 Fix `HTTPException` header type annotations. PR [#9648](https://github.com/tiangolo/fastapi/pull/9648) by [@tiangolo](https://github.com/tiangolo).
 * 🐛 Fix OpenAPI model fields int validations, `gte` to `ge`. PR [#9635](https://github.com/tiangolo/fastapi/pull/9635) by [@tiangolo](https://github.com/tiangolo).
 
 ### Upgrades
 
 * 📌 Update minimum version of Pydantic to >=1.7.4. This fixes an issue when trying to use an old version of Pydantic. PR [#9567](https://github.com/tiangolo/fastapi/pull/9567) by [@Kludex](https://github.com/Kludex).
 
+### Refactors
+
+* ♻ Remove `media_type` from `ORJSONResponse` as it's inherited from the parent class. PR [#5805](https://github.com/tiangolo/fastapi/pull/5805) by [@Kludex](https://github.com/Kludex).
+* ♻ Instantiate `HTTPException` only when needed, optimization refactor. PR [#5356](https://github.com/tiangolo/fastapi/pull/5356) by [@pawamoy](https://github.com/pawamoy).
+
 ### Docs
 
 * 🔥 Remove link to Pydantic's benchmark, as it was removed there. PR [#5811](https://github.com/tiangolo/fastapi/pull/5811) by [@Kludex](https://github.com/Kludex).
 
 ### Translations
 
 * 🌐 Fix spelling in Indonesian translation of `docs/id/docs/tutorial/index.md`. PR [#5635](https://github.com/tiangolo/fastapi/pull/5635) by [@purwowd](https://github.com/purwowd).
 * 🌐 Add Russian translation for `docs/ru/docs/tutorial/index.md`. PR [#5896](https://github.com/tiangolo/fastapi/pull/5896) by [@Wilidon](https://github.com/Wilidon).
 * 🌐 Add Chinese translations for `docs/zh/docs/advanced/response-change-status-code.md` and `docs/zh/docs/advanced/response-headers.md`. PR [#9544](https://github.com/tiangolo/fastapi/pull/9544) by [@ChoyeonChern](https://github.com/ChoyeonChern).
 * 🌐 Add Russian translation for `docs/ru/docs/tutorial/schema-extra-example.md`. PR [#9621](https://github.com/tiangolo/fastapi/pull/9621) by [@Alexandrhub](https://github.com/Alexandrhub).
 
 ### Internal
 
 * 🔧 Add sponsor Platform.sh. PR [#9650](https://github.com/tiangolo/fastapi/pull/9650) by [@tiangolo](https://github.com/tiangolo).
-* ♻ Remove `media_type` from `ORJSONResponse` as it's inherited from the parent class. PR [#5805](https://github.com/tiangolo/fastapi/pull/5805) by [@Kludex](https://github.com/Kludex).
 * 👷 Add custom token to Smokeshow and Preview Docs for download-artifact, to prevent API rate limits. PR [#9646](https://github.com/tiangolo/fastapi/pull/9646) by [@tiangolo](https://github.com/tiangolo).
 * 👷 Add custom tokens for GitHub Actions to avoid rate limits. PR [#9647](https://github.com/tiangolo/fastapi/pull/9647) by [@tiangolo](https://github.com/tiangolo).
-* ♻ Instantiate `HTTPException` only when needed, optimization refactor. PR [#5356](https://github.com/tiangolo/fastapi/pull/5356) by [@pawamoy](https://github.com/pawamoy).
 
 ## 0.96.0
 
 ### Features
 
 * ⚡ Update `create_cloned_field` to use a global cache and improve startup performance. PR [#4645](https://github.com/tiangolo/fastapi/pull/4645) by [@madkinsz](https://github.com/madkinsz) and previous original PR by [@huonw](https://github.com/huonw).
```

### Comparing `fastapi-0.96.1/docs/en/docs/advanced/additional-responses.md` & `fastapi-0.97.0/docs/en/docs/advanced/additional-responses.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/advanced/additional-status-codes.md` & `fastapi-0.97.0/docs/en/docs/advanced/additional-status-codes.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/advanced/advanced-dependencies.md` & `fastapi-0.97.0/docs/en/docs/advanced/advanced-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/advanced/async-sql-databases.md` & `fastapi-0.97.0/docs/en/docs/advanced/async-sql-databases.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/advanced/async-tests.md` & `fastapi-0.97.0/docs/en/docs/advanced/async-tests.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/advanced/behind-a-proxy.md` & `fastapi-0.97.0/docs/en/docs/advanced/behind-a-proxy.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/advanced/conditional-openapi.md` & `fastapi-0.97.0/docs/en/docs/advanced/conditional-openapi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/advanced/custom-request-and-route.md` & `fastapi-0.97.0/docs/en/docs/advanced/custom-request-and-route.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/advanced/custom-response.md` & `fastapi-0.97.0/docs/en/docs/advanced/custom-response.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/advanced/dataclasses.md` & `fastapi-0.97.0/docs/en/docs/advanced/dataclasses.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/advanced/events.md` & `fastapi-0.97.0/docs/en/docs/advanced/events.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/advanced/extending-openapi.md` & `fastapi-0.97.0/docs/en/docs/advanced/extending-openapi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/advanced/generate-clients.md` & `fastapi-0.97.0/docs/en/docs/advanced/generate-clients.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/advanced/graphql.md` & `fastapi-0.97.0/docs/en/docs/advanced/graphql.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/advanced/index.md` & `fastapi-0.97.0/docs/en/docs/advanced/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/advanced/middleware.md` & `fastapi-0.97.0/docs/en/docs/advanced/middleware.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/advanced/nosql-databases.md` & `fastapi-0.97.0/docs/en/docs/advanced/nosql-databases.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/advanced/openapi-callbacks.md` & `fastapi-0.97.0/docs/en/docs/advanced/openapi-callbacks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/advanced/path-operation-advanced-configuration.md` & `fastapi-0.97.0/docs/en/docs/advanced/path-operation-advanced-configuration.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/advanced/response-change-status-code.md` & `fastapi-0.97.0/docs/en/docs/advanced/response-change-status-code.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/advanced/response-cookies.md` & `fastapi-0.97.0/docs/en/docs/advanced/response-cookies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/advanced/response-directly.md` & `fastapi-0.97.0/docs/en/docs/advanced/response-directly.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/advanced/response-headers.md` & `fastapi-0.97.0/docs/en/docs/advanced/response-headers.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/advanced/settings.md` & `fastapi-0.97.0/docs/en/docs/advanced/settings.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/advanced/sql-databases-peewee.md` & `fastapi-0.97.0/docs/en/docs/advanced/sql-databases-peewee.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/advanced/sub-applications.md` & `fastapi-0.97.0/docs/en/docs/advanced/sub-applications.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/advanced/templates.md` & `fastapi-0.97.0/docs/en/docs/advanced/templates.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/advanced/testing-database.md` & `fastapi-0.97.0/docs/en/docs/advanced/testing-database.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/advanced/testing-dependencies.md` & `fastapi-0.97.0/docs/en/docs/advanced/testing-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/advanced/using-request-directly.md` & `fastapi-0.97.0/docs/en/docs/advanced/using-request-directly.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/advanced/websockets.md` & `fastapi-0.97.0/docs/en/docs/advanced/websockets.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/advanced/wsgi.md` & `fastapi-0.97.0/docs/en/docs/advanced/wsgi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/advanced/security/http-basic-auth.md` & `fastapi-0.97.0/docs/en/docs/advanced/security/http-basic-auth.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/advanced/security/index.md` & `fastapi-0.97.0/docs/en/docs/advanced/security/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/advanced/security/oauth2-scopes.md` & `fastapi-0.97.0/docs/en/docs/advanced/security/oauth2-scopes.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/css/custom.css` & `fastapi-0.97.0/docs/en/docs/css/custom.css`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/css/termynal.css` & `fastapi-0.97.0/docs/en/docs/css/termynal.css`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/deployment/concepts.md` & `fastapi-0.97.0/docs/en/docs/deployment/concepts.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/deployment/deta.md` & `fastapi-0.97.0/docs/en/docs/deployment/deta.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/deployment/docker.md` & `fastapi-0.97.0/docs/en/docs/deployment/docker.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/deployment/https.md` & `fastapi-0.97.0/docs/en/docs/deployment/https.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/deployment/index.md` & `fastapi-0.97.0/docs/en/docs/deployment/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/deployment/manually.md` & `fastapi-0.97.0/docs/en/docs/deployment/manually.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/deployment/server-workers.md` & `fastapi-0.97.0/docs/en/docs/deployment/server-workers.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/deployment/versions.md` & `fastapi-0.97.0/docs/en/docs/deployment/versions.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/github-social-preview.png` & `fastapi-0.97.0/docs/en/docs/img/github-social-preview.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/github-social-preview.svg` & `fastapi-0.97.0/docs/en/docs/img/github-social-preview.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/icon-transparent-bg.png` & `fastapi-0.97.0/docs/en/docs/img/icon-transparent-bg.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/icon-white-bg.png` & `fastapi-0.97.0/docs/en/docs/img/icon-white-bg.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/icon-white.svg` & `fastapi-0.97.0/docs/en/docs/img/icon-white.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/logo-teal-vector.svg` & `fastapi-0.97.0/docs/en/docs/img/logo-teal-vector.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/logo-teal.svg` & `fastapi-0.97.0/docs/en/docs/img/logo-teal.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/pycharm-completion.png` & `fastapi-0.97.0/docs/en/docs/img/pycharm-completion.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/vscode-completion.png` & `fastapi-0.97.0/docs/en/docs/img/vscode-completion.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-01.png` & `fastapi-0.97.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-02.png` & `fastapi-0.97.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-03.png` & `fastapi-0.97.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-03.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-04.png` & `fastapi-0.97.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-04.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-05.png` & `fastapi-0.97.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-05.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-06.png` & `fastapi-0.97.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-06.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-07.png` & `fastapi-0.97.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-07.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/async/parallel-burgers/parallel-burgers-01.png` & `fastapi-0.97.0/docs/en/docs/img/async/parallel-burgers/parallel-burgers-01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/async/parallel-burgers/parallel-burgers-02.png` & `fastapi-0.97.0/docs/en/docs/img/async/parallel-burgers/parallel-burgers-02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/async/parallel-burgers/parallel-burgers-03.png` & `fastapi-0.97.0/docs/en/docs/img/async/parallel-burgers/parallel-burgers-03.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/async/parallel-burgers/parallel-burgers-04.png` & `fastapi-0.97.0/docs/en/docs/img/async/parallel-burgers/parallel-burgers-04.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/async/parallel-burgers/parallel-burgers-05.png` & `fastapi-0.97.0/docs/en/docs/img/async/parallel-burgers/parallel-burgers-05.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/async/parallel-burgers/parallel-burgers-06.png` & `fastapi-0.97.0/docs/en/docs/img/async/parallel-burgers/parallel-burgers-06.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/deployment/concepts/image01.png` & `fastapi-0.97.0/docs/en/docs/img/deployment/concepts/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/deployment/concepts/process-ram.drawio` & `fastapi-0.97.0/docs/en/docs/img/deployment/concepts/process-ram.drawio`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/deployment/concepts/process-ram.svg` & `fastapi-0.97.0/docs/en/docs/img/deployment/concepts/process-ram.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/deployment/deta/image01.png` & `fastapi-0.97.0/docs/en/docs/img/deployment/deta/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/deployment/deta/image02.png` & `fastapi-0.97.0/docs/en/docs/img/deployment/deta/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/deployment/deta/image03.png` & `fastapi-0.97.0/docs/en/docs/img/deployment/deta/image03.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/deployment/deta/image04.png` & `fastapi-0.97.0/docs/en/docs/img/deployment/deta/image04.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/deployment/deta/image05.png` & `fastapi-0.97.0/docs/en/docs/img/deployment/deta/image05.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/deployment/deta/image06.png` & `fastapi-0.97.0/docs/en/docs/img/deployment/deta/image06.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/deployment/https/https.drawio` & `fastapi-0.97.0/docs/en/docs/img/deployment/https/https.drawio`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/deployment/https/https.svg` & `fastapi-0.97.0/docs/en/docs/img/deployment/https/https.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/deployment/https/https01.drawio` & `fastapi-0.97.0/docs/en/docs/img/deployment/https/https01.drawio`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/deployment/https/https01.svg` & `fastapi-0.97.0/docs/en/docs/img/deployment/https/https01.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/deployment/https/https02.drawio` & `fastapi-0.97.0/docs/en/docs/img/deployment/https/https02.drawio`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/deployment/https/https02.svg` & `fastapi-0.97.0/docs/en/docs/img/deployment/https/https02.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/deployment/https/https03.drawio` & `fastapi-0.97.0/docs/en/docs/img/deployment/https/https03.drawio`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/deployment/https/https03.svg` & `fastapi-0.97.0/docs/en/docs/img/deployment/https/https03.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/deployment/https/https04.drawio` & `fastapi-0.97.0/docs/en/docs/img/deployment/https/https04.drawio`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/deployment/https/https04.svg` & `fastapi-0.97.0/docs/en/docs/img/deployment/https/https04.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/deployment/https/https05.drawio` & `fastapi-0.97.0/docs/en/docs/img/deployment/https/https05.drawio`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/deployment/https/https05.svg` & `fastapi-0.97.0/docs/en/docs/img/deployment/https/https05.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/deployment/https/https06.drawio` & `fastapi-0.97.0/docs/en/docs/img/deployment/https/https06.drawio`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/deployment/https/https06.svg` & `fastapi-0.97.0/docs/en/docs/img/deployment/https/https06.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/deployment/https/https07.drawio` & `fastapi-0.97.0/docs/en/docs/img/deployment/https/https07.drawio`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/deployment/https/https07.svg` & `fastapi-0.97.0/docs/en/docs/img/deployment/https/https07.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/deployment/https/https08.drawio` & `fastapi-0.97.0/docs/en/docs/img/deployment/https/https08.drawio`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/deployment/https/https08.svg` & `fastapi-0.97.0/docs/en/docs/img/deployment/https/https08.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/index/index-01-swagger-ui-simple.png` & `fastapi-0.97.0/docs/en/docs/img/index/index-01-swagger-ui-simple.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/index/index-02-redoc-simple.png` & `fastapi-0.97.0/docs/en/docs/img/index/index-02-redoc-simple.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/index/index-03-swagger-02.png` & `fastapi-0.97.0/docs/en/docs/img/index/index-03-swagger-02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/index/index-04-swagger-03.png` & `fastapi-0.97.0/docs/en/docs/img/index/index-04-swagger-03.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/index/index-05-swagger-04.png` & `fastapi-0.97.0/docs/en/docs/img/index/index-05-swagger-04.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/index/index-06-redoc-02.png` & `fastapi-0.97.0/docs/en/docs/img/index/index-06-redoc-02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/logo-margin/logo-teal-vector.svg` & `fastapi-0.97.0/docs/en/docs/img/logo-margin/logo-teal-vector.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/logo-margin/logo-teal.png` & `fastapi-0.97.0/docs/en/docs/img/logo-margin/logo-teal.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/logo-margin/logo-teal.svg` & `fastapi-0.97.0/docs/en/docs/img/logo-margin/logo-teal.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/logo-margin/logo-white-bg.png` & `fastapi-0.97.0/docs/en/docs/img/logo-margin/logo-white-bg.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/python-types/image01.png` & `fastapi-0.97.0/docs/en/docs/img/python-types/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/python-types/image02.png` & `fastapi-0.97.0/docs/en/docs/img/python-types/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/python-types/image03.png` & `fastapi-0.97.0/docs/en/docs/img/python-types/image03.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/python-types/image04.png` & `fastapi-0.97.0/docs/en/docs/img/python-types/image04.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/python-types/image05.png` & `fastapi-0.97.0/docs/en/docs/img/python-types/image05.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/python-types/image06.png` & `fastapi-0.97.0/docs/en/docs/img/python-types/image06.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/budget-insight.svg` & `fastapi-0.97.0/docs/en/docs/img/sponsors/budget-insight.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/calmcode.jpg` & `fastapi-0.97.0/docs/en/docs/img/sponsors/calmcode.jpg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/classiq-banner.png` & `fastapi-0.97.0/docs/en/docs/img/sponsors/classiq-banner.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/classiq.png` & `fastapi-0.97.0/docs/en/docs/img/sponsors/classiq.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/cryptapi-banner.svg` & `fastapi-0.97.0/docs/en/docs/img/sponsors/cryptapi-banner.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/cryptapi.svg` & `fastapi-0.97.0/docs/en/docs/img/sponsors/cryptapi.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/databento.svg` & `fastapi-0.97.0/docs/en/docs/img/sponsors/databento.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/deta-banner.svg` & `fastapi-0.97.0/docs/en/docs/img/sponsors/deta-banner.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/deta.svg` & `fastapi-0.97.0/docs/en/docs/img/sponsors/deta.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/docarray-top-banner.svg` & `fastapi-0.97.0/docs/en/docs/img/sponsors/docarray-top-banner.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/docarray.svg` & `fastapi-0.97.0/docs/en/docs/img/sponsors/docarray.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/doist-banner.svg` & `fastapi-0.97.0/docs/en/docs/img/sponsors/doist-banner.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/doist.svg` & `fastapi-0.97.0/docs/en/docs/img/sponsors/doist.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/dropbase-banner.svg` & `fastapi-0.97.0/docs/en/docs/img/sponsors/dropbase-banner.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/dropbase.svg` & `fastapi-0.97.0/docs/en/docs/img/sponsors/dropbase.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/exoflare.png` & `fastapi-0.97.0/docs/en/docs/img/sponsors/exoflare.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/fastapi-course-bundle-banner.png` & `fastapi-0.97.0/docs/en/docs/img/sponsors/fastapi-course-bundle-banner.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/fastapi-course-bundle-banner.svg` & `fastapi-0.97.0/docs/en/docs/img/sponsors/fastapi-course-bundle-banner.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/haystack-fastapi.svg` & `fastapi-0.97.0/docs/en/docs/img/sponsors/haystack-fastapi.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/imgwhale-banner.svg` & `fastapi-0.97.0/docs/en/docs/img/sponsors/imgwhale-banner.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/imgwhale.svg` & `fastapi-0.97.0/docs/en/docs/img/sponsors/imgwhale.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/ines-course.jpg` & `fastapi-0.97.0/docs/en/docs/img/sponsors/ines-course.jpg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/investsuite.svg` & `fastapi-0.97.0/docs/en/docs/img/sponsors/investsuite.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/jina-ai-banner.png` & `fastapi-0.97.0/docs/en/docs/img/sponsors/jina-ai-banner.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/jina-ai.png` & `fastapi-0.97.0/docs/en/docs/img/sponsors/jina-ai.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/jina-banner.svg` & `fastapi-0.97.0/docs/en/docs/img/sponsors/jina-banner.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/jina-top-banner.svg` & `fastapi-0.97.0/docs/en/docs/img/sponsors/jina-top-banner.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/jina.svg` & `fastapi-0.97.0/docs/en/docs/img/sponsors/jina.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/jina2.svg` & `fastapi-0.97.0/docs/en/docs/img/sponsors/jina2.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/platform-sh-banner.png` & `fastapi-0.97.0/docs/en/docs/img/sponsors/platform-sh-banner.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/platform-sh.png` & `fastapi-0.97.0/docs/en/docs/img/sponsors/platform-sh.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/powens.png` & `fastapi-0.97.0/docs/en/docs/img/sponsors/powens.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/striveworks-banner.png` & `fastapi-0.97.0/docs/en/docs/img/sponsors/striveworks-banner.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/striveworks.png` & `fastapi-0.97.0/docs/en/docs/img/sponsors/striveworks.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/striveworks2.png` & `fastapi-0.97.0/docs/en/docs/img/sponsors/striveworks2.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/svix.svg` & `fastapi-0.97.0/docs/en/docs/img/sponsors/svix.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/talkpython.png` & `fastapi-0.97.0/docs/en/docs/img/sponsors/talkpython.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/testdriven.svg` & `fastapi-0.97.0/docs/en/docs/img/sponsors/testdriven.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/vimso.png` & `fastapi-0.97.0/docs/en/docs/img/sponsors/vimso.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/sponsors/wetransfer.svg` & `fastapi-0.97.0/docs/en/docs/img/sponsors/wetransfer.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/additional-responses/image01.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/additional-responses/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/async-sql-databases/image01.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/async-sql-databases/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/behind-a-proxy/image01.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/behind-a-proxy/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/behind-a-proxy/image02.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/behind-a-proxy/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/behind-a-proxy/image03.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/behind-a-proxy/image03.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/bigger-applications/image01.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/bigger-applications/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/bigger-applications/package.drawio` & `fastapi-0.97.0/docs/en/docs/img/tutorial/bigger-applications/package.drawio`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/bigger-applications/package.svg` & `fastapi-0.97.0/docs/en/docs/img/tutorial/bigger-applications/package.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/body/image01.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/body/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/body/image02.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/body/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/body/image03.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/body/image03.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/body/image04.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/body/image04.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/body/image05.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/body/image05.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/body-fields/image01.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/body-fields/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/body-fields/image02.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/body-fields/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/body-nested-models/image01.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/body-nested-models/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/custom-response/image01.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/custom-response/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/dataclasses/image01.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/dataclasses/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/debugging/image01.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/debugging/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/debugging/image02.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/debugging/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/dependencies/image01.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/dependencies/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/dependencies/image02.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/dependencies/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/extending-openapi/image01.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/extending-openapi/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/extending-openapi/image02.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/extending-openapi/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/extending-openapi/image03.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/extending-openapi/image03.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/extending-openapi/image04.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/extending-openapi/image04.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/generate-clients/image01.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/generate-clients/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/generate-clients/image02.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/generate-clients/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/generate-clients/image03.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/generate-clients/image03.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/generate-clients/image04.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/generate-clients/image04.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/generate-clients/image05.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/generate-clients/image05.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/generate-clients/image06.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/generate-clients/image06.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/generate-clients/image07.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/generate-clients/image07.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/generate-clients/image08.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/generate-clients/image08.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/graphql/image01.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/graphql/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/metadata/image01.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/metadata/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/metadata/image02.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/metadata/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/openapi-callbacks/image01.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/openapi-callbacks/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/path-operation-advanced-configuration/image01.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/path-operation-advanced-configuration/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/path-operation-configuration/image01.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/path-operation-configuration/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/path-operation-configuration/image02.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/path-operation-configuration/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/path-operation-configuration/image03.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/path-operation-configuration/image03.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/path-operation-configuration/image04.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/path-operation-configuration/image04.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/path-operation-configuration/image05.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/path-operation-configuration/image05.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/path-params/image01.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/path-params/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/path-params/image02.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/path-params/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/path-params/image03.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/path-params/image03.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/query-params-str-validations/image01.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/query-params-str-validations/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/query-params-str-validations/image02.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/query-params-str-validations/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/response-model/image01.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/response-model/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/response-model/image02.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/response-model/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/response-status-code/image01.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/response-status-code/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/response-status-code/image02.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/response-status-code/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/security/image01.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/security/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/security/image02.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/security/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/security/image03.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/security/image03.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/security/image04.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/security/image04.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/security/image05.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/security/image05.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/security/image06.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/security/image06.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/security/image07.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/security/image07.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/security/image08.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/security/image08.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/security/image09.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/security/image09.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/security/image10.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/security/image10.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/security/image11.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/security/image11.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/security/image12.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/security/image12.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/sql-databases/image01.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/sql-databases/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/sql-databases/image02.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/sql-databases/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/sub-applications/image01.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/sub-applications/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/sub-applications/image02.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/sub-applications/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/websockets/image01.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/websockets/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/websockets/image02.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/websockets/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/websockets/image03.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/websockets/image03.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/websockets/image04.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/websockets/image04.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/img/tutorial/websockets/image05.png` & `fastapi-0.97.0/docs/en/docs/img/tutorial/websockets/image05.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/js/custom.js` & `fastapi-0.97.0/docs/en/docs/js/custom.js`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/js/termynal.js` & `fastapi-0.97.0/docs/en/docs/js/termynal.js`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/background-tasks.md` & `fastapi-0.97.0/docs/en/docs/tutorial/background-tasks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/bigger-applications.md` & `fastapi-0.97.0/docs/en/docs/tutorial/bigger-applications.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/body-fields.md` & `fastapi-0.97.0/docs/en/docs/tutorial/body-fields.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/body-multiple-params.md` & `fastapi-0.97.0/docs/en/docs/tutorial/body-multiple-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/body-nested-models.md` & `fastapi-0.97.0/docs/en/docs/tutorial/body-nested-models.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/body-updates.md` & `fastapi-0.97.0/docs/en/docs/tutorial/body-updates.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/body.md` & `fastapi-0.97.0/docs/en/docs/tutorial/body.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/cookie-params.md` & `fastapi-0.97.0/docs/en/docs/tutorial/cookie-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/cors.md` & `fastapi-0.97.0/docs/en/docs/tutorial/cors.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/debugging.md` & `fastapi-0.97.0/docs/en/docs/tutorial/debugging.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/encoder.md` & `fastapi-0.97.0/docs/en/docs/tutorial/encoder.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/extra-data-types.md` & `fastapi-0.97.0/docs/en/docs/tutorial/extra-data-types.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/extra-models.md` & `fastapi-0.97.0/docs/en/docs/tutorial/extra-models.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/first-steps.md` & `fastapi-0.97.0/docs/en/docs/tutorial/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/handling-errors.md` & `fastapi-0.97.0/docs/en/docs/tutorial/handling-errors.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/header-params.md` & `fastapi-0.97.0/docs/en/docs/tutorial/header-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/index.md` & `fastapi-0.97.0/docs/en/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/metadata.md` & `fastapi-0.97.0/docs/en/docs/tutorial/metadata.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/middleware.md` & `fastapi-0.97.0/docs/en/docs/tutorial/middleware.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/path-operation-configuration.md` & `fastapi-0.97.0/docs/en/docs/tutorial/path-operation-configuration.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/path-params-numeric-validations.md` & `fastapi-0.97.0/docs/en/docs/tutorial/path-params-numeric-validations.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/path-params.md` & `fastapi-0.97.0/docs/en/docs/tutorial/path-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/query-params-str-validations.md` & `fastapi-0.97.0/docs/en/docs/tutorial/query-params-str-validations.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/query-params.md` & `fastapi-0.97.0/docs/en/docs/tutorial/query-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/request-files.md` & `fastapi-0.97.0/docs/en/docs/tutorial/request-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/request-forms-and-files.md` & `fastapi-0.97.0/docs/en/docs/tutorial/request-forms-and-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/request-forms.md` & `fastapi-0.97.0/docs/en/docs/tutorial/request-forms.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/response-model.md` & `fastapi-0.97.0/docs/en/docs/tutorial/response-model.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/response-status-code.md` & `fastapi-0.97.0/docs/en/docs/tutorial/response-status-code.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/schema-extra-example.md` & `fastapi-0.97.0/docs/en/docs/tutorial/schema-extra-example.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/sql-databases.md` & `fastapi-0.97.0/docs/en/docs/tutorial/sql-databases.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/static-files.md` & `fastapi-0.97.0/docs/en/docs/tutorial/static-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/testing.md` & `fastapi-0.97.0/docs/en/docs/tutorial/testing.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/dependencies/classes-as-dependencies.md` & `fastapi-0.97.0/docs/en/docs/tutorial/dependencies/classes-as-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/dependencies/dependencies-in-path-operation-decorators.md` & `fastapi-0.97.0/docs/en/docs/tutorial/dependencies/dependencies-in-path-operation-decorators.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/dependencies/dependencies-with-yield.md` & `fastapi-0.97.0/docs/en/docs/tutorial/dependencies/dependencies-with-yield.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/dependencies/global-dependencies.md` & `fastapi-0.97.0/docs/en/docs/tutorial/dependencies/global-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/dependencies/index.md` & `fastapi-0.97.0/docs/en/docs/tutorial/dependencies/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/dependencies/sub-dependencies.md` & `fastapi-0.97.0/docs/en/docs/tutorial/dependencies/sub-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/security/first-steps.md` & `fastapi-0.97.0/docs/en/docs/tutorial/security/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/security/get-current-user.md` & `fastapi-0.97.0/docs/en/docs/tutorial/security/get-current-user.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/security/index.md` & `fastapi-0.97.0/docs/en/docs/tutorial/security/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/security/oauth2-jwt.md` & `fastapi-0.97.0/docs/en/docs/tutorial/security/oauth2-jwt.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/docs/tutorial/security/simple-oauth2.md` & `fastapi-0.97.0/docs/en/docs/tutorial/security/simple-oauth2.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/en/overrides/main.html` & `fastapi-0.97.0/docs/en/overrides/main.html`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/es/mkdocs.yml` & `fastapi-0.97.0/docs/es/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/es/docs/async.md` & `fastapi-0.97.0/docs/es/docs/async.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/es/docs/features.md` & `fastapi-0.97.0/docs/es/docs/features.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/es/docs/index.md` & `fastapi-0.97.0/docs/es/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/es/docs/python-types.md` & `fastapi-0.97.0/docs/es/docs/python-types.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/es/docs/advanced/additional-status-codes.md` & `fastapi-0.97.0/docs/es/docs/advanced/additional-status-codes.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/es/docs/advanced/index.md` & `fastapi-0.97.0/docs/es/docs/advanced/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/es/docs/advanced/path-operation-advanced-configuration.md` & `fastapi-0.97.0/docs/es/docs/advanced/path-operation-advanced-configuration.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/es/docs/advanced/response-directly.md` & `fastapi-0.97.0/docs/es/docs/advanced/response-directly.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/es/docs/tutorial/first-steps.md` & `fastapi-0.97.0/docs/es/docs/tutorial/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/es/docs/tutorial/index.md` & `fastapi-0.97.0/docs/es/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/es/docs/tutorial/path-params.md` & `fastapi-0.97.0/docs/es/docs/tutorial/path-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/es/docs/tutorial/query-params.md` & `fastapi-0.97.0/docs/es/docs/tutorial/query-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/fa/mkdocs.yml` & `fastapi-0.97.0/docs/fa/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/fa/docs/index.md` & `fastapi-0.97.0/docs/fa/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/fr/mkdocs.yml` & `fastapi-0.97.0/docs/fr/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/fr/docs/alternatives.md` & `fastapi-0.97.0/docs/fr/docs/alternatives.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/fr/docs/async.md` & `fastapi-0.97.0/docs/fr/docs/async.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/fr/docs/external-links.md` & `fastapi-0.97.0/docs/fr/docs/external-links.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/fr/docs/fastapi-people.md` & `fastapi-0.97.0/docs/fr/docs/fastapi-people.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/fr/docs/features.md` & `fastapi-0.97.0/docs/fr/docs/features.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/fr/docs/help-fastapi.md` & `fastapi-0.97.0/docs/fr/docs/help-fastapi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/fr/docs/history-design-future.md` & `fastapi-0.97.0/docs/fr/docs/history-design-future.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/fr/docs/index.md` & `fastapi-0.97.0/docs/fr/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/fr/docs/project-generation.md` & `fastapi-0.97.0/docs/fr/docs/project-generation.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/fr/docs/python-types.md` & `fastapi-0.97.0/docs/fr/docs/python-types.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/fr/docs/advanced/additional-responses.md` & `fastapi-0.97.0/docs/fr/docs/advanced/additional-responses.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/fr/docs/advanced/additional-status-codes.md` & `fastapi-0.97.0/docs/fr/docs/advanced/additional-status-codes.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/fr/docs/advanced/index.md` & `fastapi-0.97.0/docs/fr/docs/advanced/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/fr/docs/advanced/path-operation-advanced-configuration.md` & `fastapi-0.97.0/docs/fr/docs/advanced/path-operation-advanced-configuration.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/fr/docs/advanced/response-directly.md` & `fastapi-0.97.0/docs/fr/docs/advanced/response-directly.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/fr/docs/deployment/deta.md` & `fastapi-0.97.0/docs/fr/docs/deployment/deta.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/fr/docs/deployment/docker.md` & `fastapi-0.97.0/docs/fr/docs/deployment/docker.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/fr/docs/deployment/https.md` & `fastapi-0.97.0/docs/fr/docs/deployment/https.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/fr/docs/deployment/index.md` & `fastapi-0.97.0/docs/fr/docs/deployment/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/fr/docs/deployment/manually.md` & `fastapi-0.97.0/docs/fr/docs/deployment/manually.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/fr/docs/deployment/versions.md` & `fastapi-0.97.0/docs/fr/docs/deployment/versions.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/fr/docs/tutorial/background-tasks.md` & `fastapi-0.97.0/docs/fr/docs/tutorial/background-tasks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/fr/docs/tutorial/body.md` & `fastapi-0.97.0/docs/fr/docs/tutorial/body.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/fr/docs/tutorial/debugging.md` & `fastapi-0.97.0/docs/fr/docs/tutorial/debugging.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/fr/docs/tutorial/first-steps.md` & `fastapi-0.97.0/docs/fr/docs/tutorial/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/fr/docs/tutorial/path-params.md` & `fastapi-0.97.0/docs/fr/docs/tutorial/path-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/fr/docs/tutorial/query-params.md` & `fastapi-0.97.0/docs/fr/docs/tutorial/query-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/he/mkdocs.yml` & `fastapi-0.97.0/docs/he/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/he/docs/index.md` & `fastapi-0.97.0/docs/he/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/hy/mkdocs.yml` & `fastapi-0.97.0/docs/hy/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/hy/docs/index.md` & `fastapi-0.97.0/docs/hy/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/id/mkdocs.yml` & `fastapi-0.97.0/docs/id/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/id/docs/index.md` & `fastapi-0.97.0/docs/id/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/id/docs/tutorial/index.md` & `fastapi-0.97.0/docs/id/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/it/mkdocs.yml` & `fastapi-0.97.0/docs/it/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/it/docs/index.md` & `fastapi-0.97.0/docs/it/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/mkdocs.yml` & `fastapi-0.97.0/docs/ja/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/docs/alternatives.md` & `fastapi-0.97.0/docs/ja/docs/alternatives.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/docs/async.md` & `fastapi-0.97.0/docs/ja/docs/async.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/docs/benchmarks.md` & `fastapi-0.97.0/docs/ja/docs/benchmarks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/docs/contributing.md` & `fastapi-0.97.0/docs/ja/docs/contributing.md`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 ### pip
 
 上記のように環境を有効化した後:
 
 <div class="termy">
 
 ```console
-$ pip install -e ."[dev,doc,test]"
+$ pip install -r requirements.txt
 
 ---> 100%
 ```
 
 </div>
 
 これで、すべての依存関係とFastAPIを、ローカル環境にインストールします。
```

#### html2text {}

```diff
@@ -24,15 +24,15 @@
 `env/bin/
 pip`ã«`pip`ãã¤ããªãè¡¨ç¤ºãããå ´åã¯ãæ­£å¸¸ã«æ©è½ãã¦ãã¾ããð
 !!! tip "è±ç¥è­"
 ãã®ç°å¢ã§`pip`ãä½¿ã£ã¦æ°ããããã±ã¼ã¸ãã¤ã³ã¹ãã¼ã«ãããã³ã«ãä»®æ³ç°å¢ãååº¦æå¹åãã¾ãã
 ããã«ããããã®ããã±ã¼ã¸ã«ãã£ã¦ã¤ã³ã¹ãã¼ã«ãããã¿ã¼ããã«ã®ãã­ã°ã©ã 
 ãä½¿ç¨ããå ´åãã­ã¼ã«ã«ç°å¢ã®ãã®ãä½¿ç¨ããã°ã­ã¼ãã«ã«ã¤ã³ã¹ãã¼ã«ããããã®ã¯ä½¿ç¨ãããªããªãã¾ãã
 ### pip ä¸è¨ã®ããã«ç°å¢ãæå¹åããå¾:
-```console $ pip install -e ."[dev,doc,test]" ---> 100% ```
+```console $ pip install -r requirements.txt ---> 100% ```
 ããã§ããã¹ã¦ã®ä¾å­é¢ä¿ã¨FastAPIããã­ã¼ã«ã«ç°å¢ã«ã¤ã³ã¹ãã¼ã«ãã¾ãã
 #### ã­ã¼ã«ã«ç°å¢ã§FastAPIãä½¿ã
 FastAPIãã¤ã³ãã¼ããã¦ä½¿ç¨ããPythonãã¡ã¤ã«ãä½æããã­ã¼ã«ã«ç°å¢ã§å®è¡ããã¨ãã­ã¼ã«ã«ã®FastAPIã½ã¼ã¹ã³ã¼ããä½¿ç¨ããã¾ãã
 ããã¦ã`-e`
 ã§ã¤ã³ã¹ãã¼ã«ããã¦ããã­ã¼ã«ã«ã®FastAPIã½ã¼ã¹ã³ã¼ããæ´æ°ããå ´åããã®Pythonãã¡ã¤ã«ãååº¦å®è¡ããã¨ãæ´æ°ããã°ããã®æ°ãããã¼ã¸ã§ã³ã®FastAPIãä½¿ç¨ããã¾ãã
 ããã«ãããã­ã¼ã«ã«ãã¼ã¸ã§ã³ããã¤ã³ã¹ãã¼ã«ãããªãã¦ãããã¹ã¦ã®å¤æ´ããã¹ãã§ãã¾ãã
 ### ã³ã¼ãã®æ´å½¢
```

### Comparing `fastapi-0.96.1/docs/ja/docs/external-links.md` & `fastapi-0.97.0/docs/ja/docs/external-links.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/docs/fastapi-people.md` & `fastapi-0.97.0/docs/ja/docs/fastapi-people.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/docs/features.md` & `fastapi-0.97.0/docs/ja/docs/features.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/docs/help-fastapi.md` & `fastapi-0.97.0/docs/ja/docs/help-fastapi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/docs/history-design-future.md` & `fastapi-0.97.0/docs/ja/docs/history-design-future.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/docs/index.md` & `fastapi-0.97.0/docs/ja/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/docs/project-generation.md` & `fastapi-0.97.0/docs/ja/docs/project-generation.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/docs/advanced/additional-status-codes.md` & `fastapi-0.97.0/docs/ja/docs/advanced/additional-status-codes.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/docs/advanced/conditional-openapi.md` & `fastapi-0.97.0/docs/ja/docs/advanced/conditional-openapi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/docs/advanced/custom-response.md` & `fastapi-0.97.0/docs/ja/docs/advanced/custom-response.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/docs/advanced/index.md` & `fastapi-0.97.0/docs/ja/docs/advanced/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/docs/advanced/nosql-databases.md` & `fastapi-0.97.0/docs/ja/docs/advanced/nosql-databases.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/docs/advanced/path-operation-advanced-configuration.md` & `fastapi-0.97.0/docs/ja/docs/advanced/path-operation-advanced-configuration.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/docs/advanced/response-directly.md` & `fastapi-0.97.0/docs/ja/docs/advanced/response-directly.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/docs/advanced/websockets.md` & `fastapi-0.97.0/docs/ja/docs/advanced/websockets.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/docs/deployment/deta.md` & `fastapi-0.97.0/docs/ja/docs/deployment/deta.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/docs/deployment/docker.md` & `fastapi-0.97.0/docs/ja/docs/deployment/docker.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/docs/deployment/manually.md` & `fastapi-0.97.0/docs/ja/docs/deployment/manually.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/docs/deployment/versions.md` & `fastapi-0.97.0/docs/ja/docs/deployment/versions.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/docs/tutorial/body-updates.md` & `fastapi-0.97.0/docs/ja/docs/tutorial/body-updates.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/docs/tutorial/body.md` & `fastapi-0.97.0/docs/ja/docs/tutorial/body.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/docs/tutorial/cookie-params.md` & `fastapi-0.97.0/docs/ja/docs/tutorial/cookie-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/docs/tutorial/cors.md` & `fastapi-0.97.0/docs/ja/docs/tutorial/cors.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/docs/tutorial/debugging.md` & `fastapi-0.97.0/docs/ja/docs/tutorial/debugging.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/docs/tutorial/first-steps.md` & `fastapi-0.97.0/docs/ja/docs/tutorial/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/docs/tutorial/header-params.md` & `fastapi-0.97.0/docs/ja/docs/tutorial/header-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/docs/tutorial/index.md` & `fastapi-0.97.0/docs/ja/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/docs/tutorial/middleware.md` & `fastapi-0.97.0/docs/ja/docs/tutorial/middleware.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/docs/tutorial/path-params.md` & `fastapi-0.97.0/docs/ja/docs/tutorial/path-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/docs/tutorial/query-params-str-validations.md` & `fastapi-0.97.0/docs/ja/docs/tutorial/query-params-str-validations.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/docs/tutorial/query-params.md` & `fastapi-0.97.0/docs/ja/docs/tutorial/query-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/docs/tutorial/request-forms.md` & `fastapi-0.97.0/docs/ja/docs/tutorial/request-forms.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/docs/tutorial/static-files.md` & `fastapi-0.97.0/docs/ja/docs/tutorial/static-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/docs/tutorial/testing.md` & `fastapi-0.97.0/docs/ja/docs/tutorial/testing.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/docs/tutorial/security/first-steps.md` & `fastapi-0.97.0/docs/ja/docs/tutorial/security/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ja/docs/tutorial/security/oauth2-jwt.md` & `fastapi-0.97.0/docs/ja/docs/tutorial/security/oauth2-jwt.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ko/mkdocs.yml` & `fastapi-0.97.0/docs/ko/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ko/docs/index.md` & `fastapi-0.97.0/docs/ko/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ko/docs/deployment/versions.md` & `fastapi-0.97.0/docs/ko/docs/deployment/versions.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ko/docs/tutorial/cors.md` & `fastapi-0.97.0/docs/ko/docs/tutorial/cors.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ko/docs/tutorial/encoder.md` & `fastapi-0.97.0/docs/ko/docs/tutorial/encoder.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ko/docs/tutorial/first-steps.md` & `fastapi-0.97.0/docs/ko/docs/tutorial/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ko/docs/tutorial/header-params.md` & `fastapi-0.97.0/docs/ko/docs/tutorial/header-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ko/docs/tutorial/index.md` & `fastapi-0.97.0/docs/ko/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ko/docs/tutorial/path-params-numeric-validations.md` & `fastapi-0.97.0/docs/ko/docs/tutorial/path-params-numeric-validations.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ko/docs/tutorial/path-params.md` & `fastapi-0.97.0/docs/ko/docs/tutorial/path-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ko/docs/tutorial/query-params.md` & `fastapi-0.97.0/docs/ko/docs/tutorial/query-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ko/docs/tutorial/request-files.md` & `fastapi-0.97.0/docs/ko/docs/tutorial/request-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ko/docs/tutorial/request-forms-and-files.md` & `fastapi-0.97.0/docs/ko/docs/tutorial/request-forms-and-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ko/docs/tutorial/response-status-code.md` & `fastapi-0.97.0/docs/ko/docs/tutorial/response-status-code.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ko/docs/tutorial/dependencies/classes-as-dependencies.md` & `fastapi-0.97.0/docs/ko/docs/tutorial/dependencies/classes-as-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/lo/mkdocs.yml` & `fastapi-0.97.0/docs/lo/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/lo/docs/index.md` & `fastapi-0.97.0/docs/lo/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/nl/mkdocs.yml` & `fastapi-0.97.0/docs/nl/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/nl/docs/index.md` & `fastapi-0.97.0/docs/nl/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pl/mkdocs.yml` & `fastapi-0.97.0/docs/pl/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pl/docs/index.md` & `fastapi-0.97.0/docs/pl/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pl/docs/tutorial/first-steps.md` & `fastapi-0.97.0/docs/pl/docs/tutorial/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pl/docs/tutorial/index.md` & `fastapi-0.97.0/docs/pl/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/mkdocs.yml` & `fastapi-0.97.0/docs/pt/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/alternatives.md` & `fastapi-0.97.0/docs/pt/docs/alternatives.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/async.md` & `fastapi-0.97.0/docs/pt/docs/async.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/benchmarks.md` & `fastapi-0.97.0/docs/pt/docs/benchmarks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/contributing.md` & `fastapi-0.97.0/docs/pt/docs/contributing.md`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 ### pip
 
 Após ativar o ambiente como descrito acima:
 
 <div class="termy">
 
 ```console
-$ pip install -e ."[dev,doc,test]"
+$ pip install -r requirements.txt
 
 ---> 100%
 ```
 
 </div>
 
 Isso irá instalar todas as dependências e seu FastAPI local em seu ambiente local.
```

#### html2text {}

```diff
@@ -19,15 +19,15 @@
 ```console $ Get-Command pip some/directory/fastapi/env/bin/pip ```
 Se ele exibir o binÃ¡rio `pip` em `env/bin/pip` entÃ£o funcionou. ð !!! tip
 Toda vez que vocÃª instalar um novo pacote com `pip` nesse ambiente, ative o
 ambiente novamente. Isso garante que se vocÃª usar um programa instalado por
 aquele pacote, vocÃª utilizarÃ¡ aquele de seu ambiente local e nÃ£o outro que
 possa estar instalado globalmente. ### pip ApÃ³s ativar o ambiente como
 descrito acima:
-```console $ pip install -e ."[dev,doc,test]" ---> 100% ```
+```console $ pip install -r requirements.txt ---> 100% ```
 Isso irÃ¡ instalar todas as dependÃªncias e seu FastAPI local em seu ambiente
 local. #### Usando seu FastAPI local Se vocÃª cria um arquivo Python que
 importa e usa FastAPI, e roda com Python de seu ambiente local, ele irÃ¡
 utilizar o cÃ³digo fonte de seu FastAPI local. E se vocÃª atualizar o cÃ³digo
 fonte do FastAPI local, como ele Ã© instalado com `-e`, quando vocÃª rodar
 aquele arquivo Python novamente, ele irÃ¡ utilizar a nova versÃ£o do FastAPI
 que vocÃª acabou de editar. Desse modo, vocÃª nÃ£o tem que "instalar" sua
```

### Comparing `fastapi-0.96.1/docs/pt/docs/deployment.md` & `fastapi-0.97.0/docs/pt/docs/deployment.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/external-links.md` & `fastapi-0.97.0/docs/pt/docs/external-links.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/fastapi-people.md` & `fastapi-0.97.0/docs/pt/docs/fastapi-people.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/features.md` & `fastapi-0.97.0/docs/pt/docs/features.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/help-fastapi.md` & `fastapi-0.97.0/docs/pt/docs/help-fastapi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/history-design-future.md` & `fastapi-0.97.0/docs/pt/docs/history-design-future.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/index.md` & `fastapi-0.97.0/docs/pt/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/project-generation.md` & `fastapi-0.97.0/docs/pt/docs/project-generation.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/python-types.md` & `fastapi-0.97.0/docs/pt/docs/python-types.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/advanced/events.md` & `fastapi-0.97.0/docs/pt/docs/advanced/events.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/advanced/index.md` & `fastapi-0.97.0/docs/pt/docs/advanced/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/deployment/deta.md` & `fastapi-0.97.0/docs/pt/docs/deployment/deta.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/deployment/docker.md` & `fastapi-0.97.0/docs/pt/docs/deployment/docker.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/deployment/https.md` & `fastapi-0.97.0/docs/pt/docs/deployment/https.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/deployment/versions.md` & `fastapi-0.97.0/docs/pt/docs/deployment/versions.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/tutorial/background-tasks.md` & `fastapi-0.97.0/docs/pt/docs/tutorial/background-tasks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/tutorial/body-fields.md` & `fastapi-0.97.0/docs/pt/docs/tutorial/body-fields.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/tutorial/body-multiple-params.md` & `fastapi-0.97.0/docs/pt/docs/tutorial/body-multiple-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/tutorial/body-nested-models.md` & `fastapi-0.97.0/docs/pt/docs/tutorial/body-nested-models.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/tutorial/body.md` & `fastapi-0.97.0/docs/pt/docs/tutorial/body.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/tutorial/cookie-params.md` & `fastapi-0.97.0/docs/pt/docs/tutorial/cookie-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/tutorial/encoder.md` & `fastapi-0.97.0/docs/pt/docs/tutorial/encoder.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/tutorial/extra-data-types.md` & `fastapi-0.97.0/docs/pt/docs/tutorial/extra-data-types.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/tutorial/extra-models.md` & `fastapi-0.97.0/docs/pt/docs/tutorial/extra-models.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/tutorial/first-steps.md` & `fastapi-0.97.0/docs/pt/docs/tutorial/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/tutorial/handling-errors.md` & `fastapi-0.97.0/docs/pt/docs/tutorial/handling-errors.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/tutorial/header-params.md` & `fastapi-0.97.0/docs/pt/docs/tutorial/header-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/tutorial/index.md` & `fastapi-0.97.0/docs/pt/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/tutorial/path-operation-configuration.md` & `fastapi-0.97.0/docs/pt/docs/tutorial/path-operation-configuration.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/tutorial/path-params-numeric-validations.md` & `fastapi-0.97.0/docs/pt/docs/tutorial/path-params-numeric-validations.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/tutorial/path-params.md` & `fastapi-0.97.0/docs/pt/docs/tutorial/path-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/tutorial/query-params-str-validations.md` & `fastapi-0.97.0/docs/pt/docs/tutorial/query-params-str-validations.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/tutorial/query-params.md` & `fastapi-0.97.0/docs/pt/docs/tutorial/query-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/tutorial/request-forms-and-files.md` & `fastapi-0.97.0/docs/pt/docs/tutorial/request-forms-and-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/tutorial/request-forms.md` & `fastapi-0.97.0/docs/pt/docs/tutorial/request-forms.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/tutorial/response-status-code.md` & `fastapi-0.97.0/docs/pt/docs/tutorial/response-status-code.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/tutorial/static-files.md` & `fastapi-0.97.0/docs/pt/docs/tutorial/static-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/tutorial/security/first-steps.md` & `fastapi-0.97.0/docs/pt/docs/tutorial/security/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/pt/docs/tutorial/security/index.md` & `fastapi-0.97.0/docs/pt/docs/tutorial/security/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ru/mkdocs.yml` & `fastapi-0.97.0/docs/ru/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ru/docs/alternatives.md` & `fastapi-0.97.0/docs/ru/docs/alternatives.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ru/docs/async.md` & `fastapi-0.97.0/docs/ru/docs/async.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ru/docs/benchmarks.md` & `fastapi-0.97.0/docs/ru/docs/benchmarks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ru/docs/contributing.md` & `fastapi-0.97.0/docs/ru/docs/contributing.md`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 ### pip
 
 После активации виртуального окружения, как было указано ранее, введите следующую команду:
 
 <div class="termy">
 
 ```console
-$ pip install -e ."[dev,doc,test]"
+$ pip install -r requirements.txt
 
 ---> 100%
 ```
 
 </div>
 
 Это установит все необходимые зависимости в локальное окружение для Вашего локального FastAPI.
```

#### html2text {}

```diff
@@ -45,15 +45,15 @@
 Ð±Ð¸Ð±Ð»Ð¸Ð¾ÑÐµÐºÑ, ÑÑÑÐ°Ð½Ð¾Ð²Ð»ÐµÐ½Ð½ÑÑ ÑÑÐ¸Ð¼ Ð¿Ð°ÐºÐµÑÐ¾Ð¼, ÑÐ¾
 ÐÑ Ð¸ÑÐ¿Ð¾Ð»ÑÐ·ÑÐµÑÐµ Ð±Ð¸Ð±Ð»Ð¸Ð¾ÑÐµÐºÑ Ð¸Ð· ÐÐ°ÑÐµÐ³Ð¾
 Ð»Ð¾ÐºÐ°Ð»ÑÐ½Ð¾Ð³Ð¾ Ð¾ÐºÑÑÐ¶ÐµÐ½Ð¸Ñ, Ð° Ð½Ðµ Ð»ÑÐ±ÑÑ Ð´ÑÑÐ³ÑÑ,
 ÐºÐ¾ÑÐ¾ÑÐ°Ñ Ð¼Ð¾Ð¶ÐµÑ Ð±ÑÑÑ ÑÑÑÐ°Ð½Ð¾Ð²Ð»ÐµÐ½Ð° Ð³Ð»Ð¾Ð±Ð°Ð»ÑÐ½Ð¾.
 ### pip ÐÐ¾ÑÐ»Ðµ Ð°ÐºÑÐ¸Ð²Ð°ÑÐ¸Ð¸ Ð²Ð¸ÑÑÑÐ°Ð»ÑÐ½Ð¾Ð³Ð¾
 Ð¾ÐºÑÑÐ¶ÐµÐ½Ð¸Ñ, ÐºÐ°Ðº Ð±ÑÐ»Ð¾ ÑÐºÐ°Ð·Ð°Ð½Ð¾ ÑÐ°Ð½ÐµÐµ, Ð²Ð²ÐµÐ´Ð¸ÑÐµ
 ÑÐ»ÐµÐ´ÑÑÑÑÑ ÐºÐ¾Ð¼Ð°Ð½Ð´Ñ:
-```console $ pip install -e ."[dev,doc,test]" ---> 100% ```
+```console $ pip install -r requirements.txt ---> 100% ```
 Ð­ÑÐ¾ ÑÑÑÐ°Ð½Ð¾Ð²Ð¸Ñ Ð²ÑÐµ Ð½ÐµÐ¾Ð±ÑÐ¾Ð´Ð¸Ð¼ÑÐµ Ð·Ð°Ð²Ð¸ÑÐ¸Ð¼Ð¾ÑÑÐ¸
 Ð² Ð»Ð¾ÐºÐ°Ð»ÑÐ½Ð¾Ðµ Ð¾ÐºÑÑÐ¶ÐµÐ½Ð¸Ðµ Ð´Ð»Ñ ÐÐ°ÑÐµÐ³Ð¾
 Ð»Ð¾ÐºÐ°Ð»ÑÐ½Ð¾Ð³Ð¾ FastAPI. #### ÐÑÐ¿Ð¾Ð»ÑÐ·Ð¾Ð²Ð°Ð½Ð¸Ðµ
 Ð»Ð¾ÐºÐ°Ð»ÑÐ½Ð¾Ð³Ð¾ FastAPI ÐÑÐ»Ð¸ ÐÑ ÑÐ¾Ð·Ð´Ð°ÑÑÐµ Python ÑÐ°Ð¹Ð»,
 ÐºÐ¾ÑÐ¾ÑÑÐ¹ Ð¸Ð¼Ð¿Ð¾ÑÑÐ¸ÑÑÐµÑ Ð¸ Ð¸ÑÐ¿Ð¾Ð»ÑÐ·ÑÐµÑ FastAPI,Ð°
 Ð·Ð°ÑÐµÐ¼ Ð·Ð°Ð¿ÑÑÐºÐ°ÐµÑÐµ ÐµÐ³Ð¾ Ð¸Ð½ÑÐµÑÐ¿ÑÐµÑÐ°ÑÐ¾ÑÐ¾Ð¼ Python
 Ð¸Ð· ÐÐ°ÑÐµÐ³Ð¾ Ð»Ð¾ÐºÐ°Ð»ÑÐ½Ð¾Ð³Ð¾ Ð¾ÐºÑÑÐ¶ÐµÐ½Ð¸Ñ, ÑÐ¾ Ð¾Ð½ Ð±ÑÐ´ÐµÑ
```

### Comparing `fastapi-0.96.1/docs/ru/docs/external-links.md` & `fastapi-0.97.0/docs/ru/docs/external-links.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ru/docs/fastapi-people.md` & `fastapi-0.97.0/docs/ru/docs/fastapi-people.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ru/docs/features.md` & `fastapi-0.97.0/docs/ru/docs/features.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ru/docs/help-fastapi.md` & `fastapi-0.97.0/docs/ru/docs/help-fastapi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ru/docs/history-design-future.md` & `fastapi-0.97.0/docs/ru/docs/history-design-future.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ru/docs/index.md` & `fastapi-0.97.0/docs/ru/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ru/docs/project-generation.md` & `fastapi-0.97.0/docs/ru/docs/project-generation.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ru/docs/python-types.md` & `fastapi-0.97.0/docs/ru/docs/python-types.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ru/docs/deployment/concepts.md` & `fastapi-0.97.0/docs/ru/docs/deployment/concepts.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ru/docs/deployment/https.md` & `fastapi-0.97.0/docs/ru/docs/deployment/https.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ru/docs/deployment/index.md` & `fastapi-0.97.0/docs/ru/docs/deployment/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ru/docs/deployment/manually.md` & `fastapi-0.97.0/docs/ru/docs/deployment/manually.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ru/docs/deployment/versions.md` & `fastapi-0.97.0/docs/ru/docs/deployment/versions.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ru/docs/tutorial/background-tasks.md` & `fastapi-0.97.0/docs/ru/docs/tutorial/background-tasks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ru/docs/tutorial/body-fields.md` & `fastapi-0.97.0/docs/ru/docs/tutorial/body-fields.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ru/docs/tutorial/body-multiple-params.md` & `fastapi-0.97.0/docs/ru/docs/tutorial/body-multiple-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ru/docs/tutorial/body.md` & `fastapi-0.97.0/docs/ru/docs/tutorial/body.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ru/docs/tutorial/cookie-params.md` & `fastapi-0.97.0/docs/ru/docs/tutorial/cookie-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ru/docs/tutorial/debugging.md` & `fastapi-0.97.0/docs/ru/docs/tutorial/debugging.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ru/docs/tutorial/extra-data-types.md` & `fastapi-0.97.0/docs/ru/docs/tutorial/extra-data-types.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ru/docs/tutorial/first-steps.md` & `fastapi-0.97.0/docs/ru/docs/tutorial/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ru/docs/tutorial/index.md` & `fastapi-0.97.0/docs/ru/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ru/docs/tutorial/path-params-numeric-validations.md` & `fastapi-0.97.0/docs/ru/docs/tutorial/path-params-numeric-validations.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ru/docs/tutorial/path-params.md` & `fastapi-0.97.0/docs/ru/docs/tutorial/path-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ru/docs/tutorial/query-params-str-validations.md` & `fastapi-0.97.0/docs/ru/docs/tutorial/query-params-str-validations.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ru/docs/tutorial/query-params.md` & `fastapi-0.97.0/docs/ru/docs/tutorial/query-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ru/docs/tutorial/response-status-code.md` & `fastapi-0.97.0/docs/ru/docs/tutorial/response-status-code.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ru/docs/tutorial/schema-extra-example.md` & `fastapi-0.97.0/docs/ru/docs/tutorial/schema-extra-example.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ru/docs/tutorial/static-files.md` & `fastapi-0.97.0/docs/ru/docs/tutorial/static-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ru/docs/tutorial/testing.md` & `fastapi-0.97.0/docs/ru/docs/tutorial/testing.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/sq/mkdocs.yml` & `fastapi-0.97.0/docs/sq/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/sq/docs/index.md` & `fastapi-0.97.0/docs/sq/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/sv/mkdocs.yml` & `fastapi-0.97.0/docs/sv/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/sv/docs/index.md` & `fastapi-0.97.0/docs/sv/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/ta/mkdocs.yml` & `fastapi-0.97.0/docs/ta/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/tr/mkdocs.yml` & `fastapi-0.97.0/docs/tr/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/tr/docs/benchmarks.md` & `fastapi-0.97.0/docs/tr/docs/benchmarks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/tr/docs/fastapi-people.md` & `fastapi-0.97.0/docs/tr/docs/fastapi-people.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/tr/docs/features.md` & `fastapi-0.97.0/docs/tr/docs/features.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/tr/docs/index.md` & `fastapi-0.97.0/docs/tr/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/tr/docs/python-types.md` & `fastapi-0.97.0/docs/tr/docs/python-types.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/tr/docs/tutorial/first_steps.md` & `fastapi-0.97.0/docs/tr/docs/tutorial/first_steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/uk/mkdocs.yml` & `fastapi-0.97.0/docs/uk/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/uk/docs/index.md` & `fastapi-0.97.0/docs/uk/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/mkdocs.yml` & `fastapi-0.97.0/docs/zh/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/benchmarks.md` & `fastapi-0.97.0/docs/zh/docs/benchmarks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/contributing.md` & `fastapi-0.97.0/docs/zh/docs/contributing.md`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 ### pip
 
 如上所述激活环境后：
 
 <div class="termy">
 
 ```console
-$ pip install -e ."[dev,doc,test]"
+$ pip install -r requirements.txt
 
 ---> 100%
 ```
 
 </div>
 
 这将在虚拟环境中安装所有依赖和本地版本的 FastAPI。
```

#### html2text {}

```diff
@@ -17,15 +17,15 @@
 === "Windows PowerShell"
 ```console $ Get-Command pip some/directory/fastapi/env/bin/pip ```
 å¦ææ¾ç¤º `pip` ç¨åºæä»¶ä½äº `env/bin/pip` åè¯´ææ¿æ´»æåã
 ð !!! tip æ¯ä¸æ¬¡ä½ å¨è¯¥ç¯å¢ä¸ä½¿ç¨ `pip`
 å®è£äºæ°è½¯ä»¶åæ¶ï¼è¯·åæ¬¡æ¿æ´»è¯¥ç¯å¢ã
 è¿æ ·å¯ä»¥ç¡®ä¿ä½ å¨ä½¿ç¨ç±è¯¥è½¯ä»¶åå®è£çç»ç«¯ç¨åºæ¶ä½¿ç¨çæ¯å½åèæç¯å¢ä¸­çç¨åºï¼èä¸æ¯å¶ä»çå¯è½æ¯å¨å±å®è£çç¨åºã
 ### pip å¦ä¸æè¿°æ¿æ´»ç¯å¢åï¼
-```console $ pip install -e ."[dev,doc,test]" ---> 100% ```
+```console $ pip install -r requirements.txt ---> 100% ```
 è¿å°å¨èæç¯å¢ä¸­å®è£ææä¾èµåæ¬å°çæ¬ç FastAPIã ####
 ä½¿ç¨æ¬å° FastAPI å¦æä½ åå»ºä¸ä¸ªå¯¼å¥å¹¶ä½¿ç¨ FastAPI ç Python
 æä»¶ï¼ç¶åä½¿ç¨èæç¯å¢ä¸­ç Python
 è¿è¡å®ï¼å®å°ä½¿ç¨ä½ æ¬å°ç FastAPI æºç ã
 å¹¶ä¸å¦æä½ æ´æ¹è¯¥æ¬å° FastAPI çæºç ï¼ç±äºå®æ¯éè¿ `-e`
 å®è£çï¼å½ä½ åæ¬¡è¿è¡é£ä¸ª Python
 æä»¶ï¼å®å°ä½¿ç¨ä½ ååç¼è¾è¿çææ°çæ¬ç FastAPIã
```

### Comparing `fastapi-0.96.1/docs/zh/docs/fastapi-people.md` & `fastapi-0.97.0/docs/zh/docs/fastapi-people.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/features.md` & `fastapi-0.97.0/docs/zh/docs/features.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/help-fastapi.md` & `fastapi-0.97.0/docs/zh/docs/help-fastapi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/index.md` & `fastapi-0.97.0/docs/zh/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/python-types.md` & `fastapi-0.97.0/docs/zh/docs/python-types.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/advanced/additional-status-codes.md` & `fastapi-0.97.0/docs/zh/docs/advanced/additional-status-codes.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/advanced/custom-response.md` & `fastapi-0.97.0/docs/zh/docs/advanced/custom-response.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/advanced/index.md` & `fastapi-0.97.0/docs/zh/docs/advanced/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/advanced/path-operation-advanced-configuration.md` & `fastapi-0.97.0/docs/zh/docs/advanced/path-operation-advanced-configuration.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/advanced/response-change-status-code.md` & `fastapi-0.97.0/docs/zh/docs/advanced/response-change-status-code.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/advanced/response-cookies.md` & `fastapi-0.97.0/docs/zh/docs/advanced/response-cookies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/advanced/response-directly.md` & `fastapi-0.97.0/docs/zh/docs/advanced/response-directly.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/advanced/response-headers.md` & `fastapi-0.97.0/docs/zh/docs/advanced/response-headers.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/advanced/wsgi.md` & `fastapi-0.97.0/docs/zh/docs/advanced/wsgi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/bigger-applications.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/bigger-applications.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/body-fields.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/body-fields.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/body-multiple-params.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/body-multiple-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/body-nested-models.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/body-nested-models.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/body-updates.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/body-updates.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/body.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/body.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/cookie-params.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/cookie-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/cors.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/cors.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/debugging.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/debugging.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/encoder.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/encoder.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/extra-data-types.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/extra-data-types.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/extra-models.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/extra-models.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/first-steps.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/handling-errors.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/handling-errors.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/header-params.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/header-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/index.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/metadata.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/metadata.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/middleware.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/middleware.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/path-operation-configuration.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/path-operation-configuration.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/path-params-numeric-validations.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/path-params-numeric-validations.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/path-params.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/path-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/query-params-str-validations.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/query-params-str-validations.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/query-params.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/query-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/request-files.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/request-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/request-forms-and-files.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/request-forms-and-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/request-forms.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/request-forms.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/response-model.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/response-model.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/response-status-code.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/response-status-code.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/schema-extra-example.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/schema-extra-example.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/sql-databases.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/sql-databases.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/static-files.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/static-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/dependencies/classes-as-dependencies.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/dependencies/classes-as-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/dependencies/dependencies-in-path-operation-decorators.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/dependencies/dependencies-in-path-operation-decorators.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/dependencies/global-dependencies.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/dependencies/global-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/dependencies/index.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/dependencies/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/dependencies/sub-dependencies.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/dependencies/sub-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/security/first-steps.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/security/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/security/get-current-user.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/security/get-current-user.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/security/index.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/security/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/security/oauth2-jwt.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/security/oauth2-jwt.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs/zh/docs/tutorial/security/simple-oauth2.md` & `fastapi-0.97.0/docs/zh/docs/tutorial/security/simple-oauth2.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/additional_responses/tutorial002.py` & `fastapi-0.97.0/docs_src/additional_responses/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/additional_responses/tutorial003.py` & `fastapi-0.97.0/docs_src/additional_responses/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/additional_responses/tutorial004.py` & `fastapi-0.97.0/docs_src/additional_responses/tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/additional_status_codes/tutorial001.py` & `fastapi-0.97.0/docs_src/additional_status_codes/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/additional_status_codes/tutorial001_an.py` & `fastapi-0.97.0/docs_src/additional_status_codes/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/additional_status_codes/tutorial001_an_py310.py` & `fastapi-0.97.0/docs_src/additional_status_codes/tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/additional_status_codes/tutorial001_an_py39.py` & `fastapi-0.97.0/docs_src/additional_status_codes/tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/additional_status_codes/tutorial001_py310.py` & `fastapi-0.97.0/docs_src/additional_status_codes/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/app_testing/tutorial002.py` & `fastapi-0.97.0/docs_src/app_testing/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/app_testing/tutorial003.py` & `fastapi-0.97.0/docs_src/app_testing/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/app_testing/app_b/main.py` & `fastapi-0.97.0/docs_src/app_testing/app_b/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/app_testing/app_b/test_main.py` & `fastapi-0.97.0/docs_src/app_testing/app_b/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/app_testing/app_b_an/main.py` & `fastapi-0.97.0/docs_src/app_testing/app_b_an/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/app_testing/app_b_an/test_main.py` & `fastapi-0.97.0/docs_src/app_testing/app_b_an/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/app_testing/app_b_an_py310/main.py` & `fastapi-0.97.0/docs_src/app_testing/app_b_an_py310/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/app_testing/app_b_an_py310/test_main.py` & `fastapi-0.97.0/docs_src/app_testing/app_b_an_py310/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/app_testing/app_b_an_py39/main.py` & `fastapi-0.97.0/docs_src/app_testing/app_b_an_py39/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/app_testing/app_b_an_py39/test_main.py` & `fastapi-0.97.0/docs_src/app_testing/app_b_an_py39/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/app_testing/app_b_py310/main.py` & `fastapi-0.97.0/docs_src/app_testing/app_b_py310/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/app_testing/app_b_py310/test_main.py` & `fastapi-0.97.0/docs_src/app_testing/app_b_py310/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/async_sql_databases/tutorial001.py` & `fastapi-0.97.0/docs_src/async_sql_databases/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/background_tasks/tutorial001.py` & `fastapi-0.97.0/docs_src/background_tasks/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/background_tasks/tutorial002.py` & `fastapi-0.97.0/docs_src/background_tasks/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/background_tasks/tutorial002_an.py` & `fastapi-0.97.0/docs_src/background_tasks/tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/background_tasks/tutorial002_an_py310.py` & `fastapi-0.97.0/docs_src/background_tasks/tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/background_tasks/tutorial002_an_py39.py` & `fastapi-0.97.0/docs_src/background_tasks/tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/background_tasks/tutorial002_py310.py` & `fastapi-0.97.0/docs_src/background_tasks/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/bigger_applications/app/main.py` & `fastapi-0.97.0/docs_src/bigger_applications/app/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/bigger_applications/app/routers/items.py` & `fastapi-0.97.0/docs_src/bigger_applications/app/routers/items.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/bigger_applications/app_an/main.py` & `fastapi-0.97.0/docs_src/bigger_applications/app_an/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/bigger_applications/app_an/routers/items.py` & `fastapi-0.97.0/docs_src/bigger_applications/app_an/routers/items.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/bigger_applications/app_an_py39/main.py` & `fastapi-0.97.0/docs_src/bigger_applications/app_an_py39/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/bigger_applications/app_an_py39/routers/items.py` & `fastapi-0.97.0/docs_src/bigger_applications/app_an_py39/routers/items.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/body_fields/tutorial001.py` & `fastapi-0.97.0/docs_src/body_fields/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/body_fields/tutorial001_an.py` & `fastapi-0.97.0/docs_src/body_fields/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/body_fields/tutorial001_an_py310.py` & `fastapi-0.97.0/docs_src/body_fields/tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/body_fields/tutorial001_an_py39.py` & `fastapi-0.97.0/docs_src/body_fields/tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/body_fields/tutorial001_py310.py` & `fastapi-0.97.0/docs_src/body_fields/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/body_multiple_params/tutorial001.py` & `fastapi-0.97.0/docs_src/body_multiple_params/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/body_multiple_params/tutorial001_an.py` & `fastapi-0.97.0/docs_src/body_multiple_params/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/body_multiple_params/tutorial001_an_py310.py` & `fastapi-0.97.0/docs_src/body_multiple_params/tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/body_multiple_params/tutorial001_an_py39.py` & `fastapi-0.97.0/docs_src/body_multiple_params/tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/body_multiple_params/tutorial001_py310.py` & `fastapi-0.97.0/docs_src/body_multiple_params/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/body_multiple_params/tutorial003.py` & `fastapi-0.97.0/docs_src/body_multiple_params/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/body_multiple_params/tutorial003_an.py` & `fastapi-0.97.0/docs_src/body_multiple_params/tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/body_multiple_params/tutorial003_an_py310.py` & `fastapi-0.97.0/docs_src/body_multiple_params/tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/body_multiple_params/tutorial003_an_py39.py` & `fastapi-0.97.0/docs_src/body_multiple_params/tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/body_multiple_params/tutorial004.py` & `fastapi-0.97.0/docs_src/body_multiple_params/tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/body_multiple_params/tutorial004_an.py` & `fastapi-0.97.0/docs_src/body_multiple_params/tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/body_multiple_params/tutorial004_an_py310.py` & `fastapi-0.97.0/docs_src/body_multiple_params/tutorial004_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/body_multiple_params/tutorial004_an_py39.py` & `fastapi-0.97.0/docs_src/body_multiple_params/tutorial004_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/body_multiple_params/tutorial004_py310.py` & `fastapi-0.97.0/docs_src/body_multiple_params/tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/body_nested_models/tutorial005.py` & `fastapi-0.97.0/docs_src/body_nested_models/tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/body_nested_models/tutorial005_py39.py` & `fastapi-0.97.0/docs_src/body_nested_models/tutorial005_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/body_nested_models/tutorial006.py` & `fastapi-0.97.0/docs_src/body_nested_models/tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/body_nested_models/tutorial006_py39.py` & `fastapi-0.97.0/docs_src/body_nested_models/tutorial006_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/body_nested_models/tutorial007.py` & `fastapi-0.97.0/docs_src/body_nested_models/tutorial007.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/body_nested_models/tutorial007_py310.py` & `fastapi-0.97.0/docs_src/body_nested_models/tutorial007_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/body_nested_models/tutorial007_py39.py` & `fastapi-0.97.0/docs_src/body_nested_models/tutorial007_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/body_updates/tutorial001.py` & `fastapi-0.97.0/docs_src/body_updates/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/body_updates/tutorial001_py310.py` & `fastapi-0.97.0/docs_src/body_updates/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/body_updates/tutorial001_py39.py` & `fastapi-0.97.0/docs_src/body_updates/tutorial001_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/body_updates/tutorial002.py` & `fastapi-0.97.0/docs_src/body_updates/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/body_updates/tutorial002_py310.py` & `fastapi-0.97.0/docs_src/body_updates/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/body_updates/tutorial002_py39.py` & `fastapi-0.97.0/docs_src/body_updates/tutorial002_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/custom_request_and_route/tutorial001.py` & `fastapi-0.97.0/docs_src/custom_request_and_route/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/custom_request_and_route/tutorial002.py` & `fastapi-0.97.0/docs_src/custom_request_and_route/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/custom_request_and_route/tutorial003.py` & `fastapi-0.97.0/docs_src/custom_request_and_route/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/dataclasses/tutorial002.py` & `fastapi-0.97.0/docs_src/dataclasses/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/dataclasses/tutorial003.py` & `fastapi-0.97.0/docs_src/dataclasses/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/dependencies/tutorial002.py` & `fastapi-0.97.0/docs_src/dependencies/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/dependencies/tutorial002_an.py` & `fastapi-0.97.0/docs_src/dependencies/tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/dependencies/tutorial002_an_py310.py` & `fastapi-0.97.0/docs_src/dependencies/tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/dependencies/tutorial002_an_py39.py` & `fastapi-0.97.0/docs_src/dependencies/tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/dependencies/tutorial002_py310.py` & `fastapi-0.97.0/docs_src/dependencies/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/dependencies/tutorial003.py` & `fastapi-0.97.0/docs_src/dependencies/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/dependencies/tutorial003_an.py` & `fastapi-0.97.0/docs_src/dependencies/tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/dependencies/tutorial003_an_py310.py` & `fastapi-0.97.0/docs_src/dependencies/tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/dependencies/tutorial003_an_py39.py` & `fastapi-0.97.0/docs_src/dependencies/tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/dependencies/tutorial003_py310.py` & `fastapi-0.97.0/docs_src/dependencies/tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/dependencies/tutorial004.py` & `fastapi-0.97.0/docs_src/dependencies/tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/dependencies/tutorial004_an.py` & `fastapi-0.97.0/docs_src/dependencies/tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/dependencies/tutorial004_an_py310.py` & `fastapi-0.97.0/docs_src/dependencies/tutorial004_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/dependencies/tutorial004_an_py39.py` & `fastapi-0.97.0/docs_src/dependencies/tutorial004_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/dependencies/tutorial004_py310.py` & `fastapi-0.97.0/docs_src/dependencies/tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/dependencies/tutorial005_an.py` & `fastapi-0.97.0/docs_src/dependencies/tutorial005_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/dependencies/tutorial005_an_py39.py` & `fastapi-0.97.0/docs_src/dependencies/tutorial005_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/dependencies/tutorial006.py` & `fastapi-0.97.0/docs_src/dependencies/tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/dependencies/tutorial006_an.py` & `fastapi-0.97.0/docs_src/dependencies/tutorial006_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/dependencies/tutorial006_an_py39.py` & `fastapi-0.97.0/docs_src/dependencies/tutorial006_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/dependencies/tutorial008_an.py` & `fastapi-0.97.0/docs_src/dependencies/tutorial008_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/dependencies/tutorial008_an_py39.py` & `fastapi-0.97.0/docs_src/dependencies/tutorial008_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/dependencies/tutorial011_an.py` & `fastapi-0.97.0/docs_src/dependencies/tutorial011_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/dependencies/tutorial011_an_py39.py` & `fastapi-0.97.0/docs_src/dependencies/tutorial011_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/dependencies/tutorial012.py` & `fastapi-0.97.0/docs_src/dependencies/tutorial012.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/dependencies/tutorial012_an.py` & `fastapi-0.97.0/docs_src/dependencies/tutorial012_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/dependencies/tutorial012_an_py39.py` & `fastapi-0.97.0/docs_src/dependencies/tutorial012_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/dependency_testing/tutorial001.py` & `fastapi-0.97.0/docs_src/dependency_testing/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/dependency_testing/tutorial001_an.py` & `fastapi-0.97.0/docs_src/dependency_testing/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/dependency_testing/tutorial001_an_py310.py` & `fastapi-0.97.0/docs_src/dependency_testing/tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/dependency_testing/tutorial001_an_py39.py` & `fastapi-0.97.0/docs_src/dependency_testing/tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/dependency_testing/tutorial001_py310.py` & `fastapi-0.97.0/docs_src/dependency_testing/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/events/tutorial003.py` & `fastapi-0.97.0/docs_src/events/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/extending_openapi/tutorial001.py` & `fastapi-0.97.0/docs_src/extending_openapi/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/extending_openapi/tutorial002.py` & `fastapi-0.97.0/docs_src/extending_openapi/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/extra_data_types/tutorial001.py` & `fastapi-0.97.0/docs_src/extra_data_types/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/extra_data_types/tutorial001_an.py` & `fastapi-0.97.0/docs_src/extra_data_types/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/extra_data_types/tutorial001_an_py310.py` & `fastapi-0.97.0/docs_src/extra_data_types/tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/extra_data_types/tutorial001_an_py39.py` & `fastapi-0.97.0/docs_src/extra_data_types/tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/extra_data_types/tutorial001_py310.py` & `fastapi-0.97.0/docs_src/extra_data_types/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/extra_models/tutorial001.py` & `fastapi-0.97.0/docs_src/extra_models/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/extra_models/tutorial001_py310.py` & `fastapi-0.97.0/docs_src/extra_models/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/extra_models/tutorial002.py` & `fastapi-0.97.0/docs_src/extra_models/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/extra_models/tutorial002_py310.py` & `fastapi-0.97.0/docs_src/extra_models/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/extra_models/tutorial003.py` & `fastapi-0.97.0/docs_src/extra_models/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/extra_models/tutorial003_py310.py` & `fastapi-0.97.0/docs_src/extra_models/tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/generate_clients/tutorial001.py` & `fastapi-0.97.0/docs_src/generate_clients/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/generate_clients/tutorial002.py` & `fastapi-0.97.0/docs_src/generate_clients/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/generate_clients/tutorial002_py39.py` & `fastapi-0.97.0/docs_src/generate_clients/tutorial002_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/generate_clients/tutorial003.py` & `fastapi-0.97.0/docs_src/generate_clients/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/generate_clients/tutorial003_py39.py` & `fastapi-0.97.0/docs_src/generate_clients/tutorial003_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/handling_errors/tutorial003.py` & `fastapi-0.97.0/docs_src/handling_errors/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/handling_errors/tutorial004.py` & `fastapi-0.97.0/docs_src/handling_errors/tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/handling_errors/tutorial005.py` & `fastapi-0.97.0/docs_src/handling_errors/tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/handling_errors/tutorial006.py` & `fastapi-0.97.0/docs_src/handling_errors/tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/metadata/tutorial001.py` & `fastapi-0.97.0/docs_src/metadata/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/metadata/tutorial004.py` & `fastapi-0.97.0/docs_src/metadata/tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/nosql_databases/tutorial001.py` & `fastapi-0.97.0/docs_src/nosql_databases/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/openapi_callbacks/tutorial001.py` & `fastapi-0.97.0/docs_src/openapi_callbacks/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/path_operation_advanced_configuration/tutorial002.py` & `fastapi-0.97.0/docs_src/path_operation_advanced_configuration/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/path_operation_advanced_configuration/tutorial004.py` & `fastapi-0.97.0/docs_src/path_operation_advanced_configuration/tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/path_operation_advanced_configuration/tutorial006.py` & `fastapi-0.97.0/docs_src/path_operation_advanced_configuration/tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/path_operation_advanced_configuration/tutorial007.py` & `fastapi-0.97.0/docs_src/path_operation_advanced_configuration/tutorial007.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/path_operation_configuration/tutorial002.py` & `fastapi-0.97.0/docs_src/path_operation_configuration/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/path_operation_configuration/tutorial002_py310.py` & `fastapi-0.97.0/docs_src/path_operation_configuration/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/path_operation_configuration/tutorial002_py39.py` & `fastapi-0.97.0/docs_src/path_operation_configuration/tutorial002_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/path_operation_configuration/tutorial003.py` & `fastapi-0.97.0/docs_src/path_operation_configuration/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/path_operation_configuration/tutorial003_py39.py` & `fastapi-0.97.0/docs_src/path_operation_configuration/tutorial003_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/path_operation_configuration/tutorial004.py` & `fastapi-0.97.0/docs_src/path_operation_configuration/tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/path_operation_configuration/tutorial004_py310.py` & `fastapi-0.97.0/docs_src/path_operation_configuration/tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/path_operation_configuration/tutorial004_py39.py` & `fastapi-0.97.0/docs_src/path_operation_configuration/tutorial004_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/path_operation_configuration/tutorial005.py` & `fastapi-0.97.0/docs_src/path_operation_configuration/tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/path_operation_configuration/tutorial005_py310.py` & `fastapi-0.97.0/docs_src/path_operation_configuration/tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/path_operation_configuration/tutorial005_py39.py` & `fastapi-0.97.0/docs_src/path_operation_configuration/tutorial005_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/path_params/tutorial005.py` & `fastapi-0.97.0/docs_src/path_params/tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/query_params_str_validations/tutorial008_an.py` & `fastapi-0.97.0/docs_src/query_params_str_validations/tutorial008_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/query_params_str_validations/tutorial010.py` & `fastapi-0.97.0/docs_src/query_params_str_validations/tutorial010.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/query_params_str_validations/tutorial010_an.py` & `fastapi-0.97.0/docs_src/query_params_str_validations/tutorial010_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/query_params_str_validations/tutorial010_an_py310.py` & `fastapi-0.97.0/docs_src/query_params_str_validations/tutorial010_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/query_params_str_validations/tutorial010_an_py39.py` & `fastapi-0.97.0/docs_src/query_params_str_validations/tutorial010_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/query_params_str_validations/tutorial010_py310.py` & `fastapi-0.97.0/docs_src/query_params_str_validations/tutorial010_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/request_files/tutorial001_02_an.py` & `fastapi-0.97.0/docs_src/request_files/tutorial001_02_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/request_files/tutorial001_02_an_py39.py` & `fastapi-0.97.0/docs_src/request_files/tutorial001_02_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/request_files/tutorial002.py` & `fastapi-0.97.0/docs_src/request_files/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/request_files/tutorial002_an.py` & `fastapi-0.97.0/docs_src/request_files/tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/request_files/tutorial002_an_py39.py` & `fastapi-0.97.0/docs_src/request_files/tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/request_files/tutorial002_py39.py` & `fastapi-0.97.0/docs_src/request_files/tutorial002_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/request_files/tutorial003.py` & `fastapi-0.97.0/docs_src/request_files/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/request_files/tutorial003_an.py` & `fastapi-0.97.0/docs_src/request_files/tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/request_files/tutorial003_an_py39.py` & `fastapi-0.97.0/docs_src/request_files/tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/request_files/tutorial003_py39.py` & `fastapi-0.97.0/docs_src/request_files/tutorial003_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/response_model/tutorial001.py` & `fastapi-0.97.0/docs_src/response_model/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/response_model/tutorial001_01.py` & `fastapi-0.97.0/docs_src/response_model/tutorial001_01.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/response_model/tutorial001_py310.py` & `fastapi-0.97.0/docs_src/response_model/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/response_model/tutorial001_py39.py` & `fastapi-0.97.0/docs_src/response_model/tutorial001_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/response_model/tutorial004.py` & `fastapi-0.97.0/docs_src/response_model/tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/response_model/tutorial004_py310.py` & `fastapi-0.97.0/docs_src/response_model/tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/response_model/tutorial004_py39.py` & `fastapi-0.97.0/docs_src/response_model/tutorial004_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/response_model/tutorial005.py` & `fastapi-0.97.0/docs_src/response_model/tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/response_model/tutorial005_py310.py` & `fastapi-0.97.0/docs_src/response_model/tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/response_model/tutorial006.py` & `fastapi-0.97.0/docs_src/response_model/tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/response_model/tutorial006_py310.py` & `fastapi-0.97.0/docs_src/response_model/tutorial006_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/schema_extra_example/tutorial001.py` & `fastapi-0.97.0/docs_src/schema_extra_example/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/schema_extra_example/tutorial001_py310.py` & `fastapi-0.97.0/docs_src/schema_extra_example/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/schema_extra_example/tutorial003.py` & `fastapi-0.97.0/docs_src/schema_extra_example/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/schema_extra_example/tutorial003_an.py` & `fastapi-0.97.0/docs_src/schema_extra_example/tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/schema_extra_example/tutorial003_an_py310.py` & `fastapi-0.97.0/docs_src/schema_extra_example/tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/schema_extra_example/tutorial003_an_py39.py` & `fastapi-0.97.0/docs_src/schema_extra_example/tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/schema_extra_example/tutorial003_py310.py` & `fastapi-0.97.0/docs_src/schema_extra_example/tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/schema_extra_example/tutorial004.py` & `fastapi-0.97.0/docs_src/schema_extra_example/tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/schema_extra_example/tutorial004_an.py` & `fastapi-0.97.0/docs_src/schema_extra_example/tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/schema_extra_example/tutorial004_an_py310.py` & `fastapi-0.97.0/docs_src/schema_extra_example/tutorial004_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/schema_extra_example/tutorial004_an_py39.py` & `fastapi-0.97.0/docs_src/schema_extra_example/tutorial004_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/schema_extra_example/tutorial004_py310.py` & `fastapi-0.97.0/docs_src/schema_extra_example/tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/security/tutorial002.py` & `fastapi-0.97.0/docs_src/security/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/security/tutorial002_an.py` & `fastapi-0.97.0/docs_src/security/tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/security/tutorial002_an_py310.py` & `fastapi-0.97.0/docs_src/security/tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/security/tutorial002_an_py39.py` & `fastapi-0.97.0/docs_src/security/tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/security/tutorial002_py310.py` & `fastapi-0.97.0/docs_src/security/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/security/tutorial003.py` & `fastapi-0.97.0/docs_src/security/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/security/tutorial003_an.py` & `fastapi-0.97.0/docs_src/security/tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/security/tutorial003_an_py310.py` & `fastapi-0.97.0/docs_src/security/tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/security/tutorial003_an_py39.py` & `fastapi-0.97.0/docs_src/security/tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/security/tutorial003_py310.py` & `fastapi-0.97.0/docs_src/security/tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/security/tutorial004.py` & `fastapi-0.97.0/docs_src/security/tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/security/tutorial004_an.py` & `fastapi-0.97.0/docs_src/security/tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/security/tutorial004_an_py310.py` & `fastapi-0.97.0/docs_src/security/tutorial004_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/security/tutorial004_an_py39.py` & `fastapi-0.97.0/docs_src/security/tutorial004_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/security/tutorial004_py310.py` & `fastapi-0.97.0/docs_src/security/tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/security/tutorial005.py` & `fastapi-0.97.0/docs_src/security/tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/security/tutorial005_an.py` & `fastapi-0.97.0/docs_src/security/tutorial005_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/security/tutorial005_an_py310.py` & `fastapi-0.97.0/docs_src/security/tutorial005_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/security/tutorial005_an_py39.py` & `fastapi-0.97.0/docs_src/security/tutorial005_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/security/tutorial005_py310.py` & `fastapi-0.97.0/docs_src/security/tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/security/tutorial005_py39.py` & `fastapi-0.97.0/docs_src/security/tutorial005_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/security/tutorial007.py` & `fastapi-0.97.0/docs_src/security/tutorial007.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/security/tutorial007_an.py` & `fastapi-0.97.0/docs_src/security/tutorial007_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/security/tutorial007_an_py39.py` & `fastapi-0.97.0/docs_src/security/tutorial007_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/settings/app02/test_main.py` & `fastapi-0.97.0/docs_src/settings/app02/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/settings/app02_an/test_main.py` & `fastapi-0.97.0/docs_src/settings/app02_an/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/settings/app02_an_py39/test_main.py` & `fastapi-0.97.0/docs_src/settings/app02_an_py39/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/sql_databases/sql_app/alt_main.py` & `fastapi-0.97.0/docs_src/sql_databases/sql_app/alt_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/sql_databases/sql_app/crud.py` & `fastapi-0.97.0/docs_src/sql_databases/sql_app/crud.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/sql_databases/sql_app/main.py` & `fastapi-0.97.0/docs_src/sql_databases/sql_app/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/sql_databases/sql_app/models.py` & `fastapi-0.97.0/docs_src/sql_databases/sql_app/models.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/sql_databases/sql_app/tests/test_sql_app.py` & `fastapi-0.97.0/docs_src/sql_databases/sql_app/tests/test_sql_app.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/sql_databases/sql_app_py310/alt_main.py` & `fastapi-0.97.0/docs_src/sql_databases/sql_app_py310/alt_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/sql_databases/sql_app_py310/crud.py` & `fastapi-0.97.0/docs_src/sql_databases/sql_app_py310/crud.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/sql_databases/sql_app_py310/main.py` & `fastapi-0.97.0/docs_src/sql_databases/sql_app_py310/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/sql_databases/sql_app_py310/models.py` & `fastapi-0.97.0/docs_src/sql_databases/sql_app_py310/models.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/sql_databases/sql_app_py310/tests/test_sql_app.py` & `fastapi-0.97.0/docs_src/sql_databases/sql_app_py310/tests/test_sql_app.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/sql_databases/sql_app_py39/alt_main.py` & `fastapi-0.97.0/docs_src/sql_databases/sql_app_py39/alt_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/sql_databases/sql_app_py39/crud.py` & `fastapi-0.97.0/docs_src/sql_databases/sql_app_py39/crud.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/sql_databases/sql_app_py39/main.py` & `fastapi-0.97.0/docs_src/sql_databases/sql_app_py39/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/sql_databases/sql_app_py39/models.py` & `fastapi-0.97.0/docs_src/sql_databases/sql_app_py39/models.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/sql_databases/sql_app_py39/tests/test_sql_app.py` & `fastapi-0.97.0/docs_src/sql_databases/sql_app_py39/tests/test_sql_app.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/sql_databases_peewee/sql_app/crud.py` & `fastapi-0.97.0/docs_src/sql_databases_peewee/sql_app/crud.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/sql_databases_peewee/sql_app/database.py` & `fastapi-0.97.0/docs_src/sql_databases_peewee/sql_app/database.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/sql_databases_peewee/sql_app/main.py` & `fastapi-0.97.0/docs_src/sql_databases_peewee/sql_app/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/sql_databases_peewee/sql_app/schemas.py` & `fastapi-0.97.0/docs_src/sql_databases_peewee/sql_app/schemas.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/websockets/tutorial001.py` & `fastapi-0.97.0/docs_src/websockets/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/websockets/tutorial002.py` & `fastapi-0.97.0/docs_src/websockets/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/websockets/tutorial002_an.py` & `fastapi-0.97.0/docs_src/websockets/tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/websockets/tutorial002_an_py310.py` & `fastapi-0.97.0/docs_src/websockets/tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/websockets/tutorial002_an_py39.py` & `fastapi-0.97.0/docs_src/websockets/tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/websockets/tutorial002_py310.py` & `fastapi-0.97.0/docs_src/websockets/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/websockets/tutorial003.py` & `fastapi-0.97.0/docs_src/websockets/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/docs_src/websockets/tutorial003_py39.py` & `fastapi-0.97.0/docs_src/websockets/tutorial003_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/fastapi/__init__.py` & `fastapi-0.97.0/fastapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """FastAPI framework, high performance, easy to learn, fast to code, ready for production"""
 
-__version__ = "0.96.1"
+__version__ = "0.97.0"
 
 from starlette import status as status
 
 from .applications import FastAPI as FastAPI
 from .background import BackgroundTasks as BackgroundTasks
 from .datastructures import UploadFile as UploadFile
 from .exceptions import HTTPException as HTTPException
```

### Comparing `fastapi-0.96.1/fastapi/applications.py` & `fastapi-0.97.0/fastapi/applications.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,17 @@
 
 from fastapi import routing
 from fastapi.datastructures import Default, DefaultPlaceholder
 from fastapi.encoders import DictIntStrAny, SetIntStr
 from fastapi.exception_handlers import (
     http_exception_handler,
     request_validation_exception_handler,
+    websocket_request_validation_exception_handler,
 )
-from fastapi.exceptions import RequestValidationError
+from fastapi.exceptions import RequestValidationError, WebSocketRequestValidationError
 from fastapi.logger import logger
 from fastapi.middleware.asyncexitstack import AsyncExitStackMiddleware
 from fastapi.openapi.docs import (
     get_redoc_html,
     get_swagger_ui_html,
     get_swagger_ui_oauth2_redirect_html,
 )
@@ -141,14 +142,19 @@
         self.exception_handlers: Dict[
             Any, Callable[[Request, Any], Union[Response, Awaitable[Response]]]
         ] = ({} if exception_handlers is None else dict(exception_handlers))
         self.exception_handlers.setdefault(HTTPException, http_exception_handler)
         self.exception_handlers.setdefault(
             RequestValidationError, request_validation_exception_handler
         )
+        self.exception_handlers.setdefault(
+            WebSocketRequestValidationError,
+            # Starlette still has incorrect type specification for the handlers
+            websocket_request_validation_exception_handler,  # type: ignore
+        )
 
         self.user_middleware: List[Middleware] = (
             [] if middleware is None else list(middleware)
         )
         self.middleware_stack: Union[ASGIApp, None] = None
         self.setup()
 
@@ -391,23 +397,42 @@
                 generate_unique_id_function=generate_unique_id_function,
             )
             return func
 
         return decorator
 
     def add_api_websocket_route(
-        self, path: str, endpoint: Callable[..., Any], name: Optional[str] = None
+        self,
+        path: str,
+        endpoint: Callable[..., Any],
+        name: Optional[str] = None,
+        *,
+        dependencies: Optional[Sequence[Depends]] = None,
     ) -> None:
-        self.router.add_api_websocket_route(path, endpoint, name=name)
+        self.router.add_api_websocket_route(
+            path,
+            endpoint,
+            name=name,
+            dependencies=dependencies,
+        )
 
     def websocket(
-        self, path: str, name: Optional[str] = None
+        self,
+        path: str,
+        name: Optional[str] = None,
+        *,
+        dependencies: Optional[Sequence[Depends]] = None,
     ) -> Callable[[DecoratedCallable], DecoratedCallable]:
         def decorator(func: DecoratedCallable) -> DecoratedCallable:
-            self.add_api_websocket_route(path, func, name=name)
+            self.add_api_websocket_route(
+                path,
+                func,
+                name=name,
+                dependencies=dependencies,
+            )
             return func
 
         return decorator
 
     def include_router(
         self,
         router: routing.APIRouter,
```

### Comparing `fastapi-0.96.1/fastapi/concurrency.py` & `fastapi-0.97.0/fastapi/concurrency.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/fastapi/datastructures.py` & `fastapi-0.97.0/fastapi/datastructures.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/fastapi/encoders.py` & `fastapi-0.97.0/fastapi/encoders.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/fastapi/exception_handlers.py` & `fastapi-0.97.0/fastapi/exception_handlers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from fastapi.encoders import jsonable_encoder
-from fastapi.exceptions import RequestValidationError
+from fastapi.exceptions import RequestValidationError, WebSocketRequestValidationError
 from fastapi.utils import is_body_allowed_for_status_code
+from fastapi.websockets import WebSocket
 from starlette.exceptions import HTTPException
 from starlette.requests import Request
 from starlette.responses import JSONResponse, Response
-from starlette.status import HTTP_422_UNPROCESSABLE_ENTITY
+from starlette.status import HTTP_422_UNPROCESSABLE_ENTITY, WS_1008_POLICY_VIOLATION
 
 
 async def http_exception_handler(request: Request, exc: HTTPException) -> Response:
     headers = getattr(exc, "headers", None)
     if not is_body_allowed_for_status_code(exc.status_code):
         return Response(status_code=exc.status_code, headers=headers)
     return JSONResponse(
@@ -19,7 +20,15 @@
 async def request_validation_exception_handler(
     request: Request, exc: RequestValidationError
 ) -> JSONResponse:
     return JSONResponse(
         status_code=HTTP_422_UNPROCESSABLE_ENTITY,
         content={"detail": jsonable_encoder(exc.errors())},
     )
+
+
+async def websocket_request_validation_exception_handler(
+    websocket: WebSocket, exc: WebSocketRequestValidationError
+) -> None:
+    await websocket.close(
+        code=WS_1008_POLICY_VIOLATION, reason=jsonable_encoder(exc.errors())
+    )
```

### Comparing `fastapi-0.96.1/fastapi/exceptions.py` & `fastapi-0.97.0/fastapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/fastapi/param_functions.py` & `fastapi-0.97.0/fastapi/param_functions.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/fastapi/params.py` & `fastapi-0.97.0/fastapi/params.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/fastapi/responses.py` & `fastapi-0.97.0/fastapi/responses.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/fastapi/routing.py` & `fastapi-0.97.0/fastapi/routing.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,19 @@
     get_body_field,
     get_dependant,
     get_parameterless_sub_dependant,
     get_typed_return_annotation,
     solve_dependencies,
 )
 from fastapi.encoders import DictIntStrAny, SetIntStr, jsonable_encoder
-from fastapi.exceptions import RequestValidationError, WebSocketRequestValidationError
+from fastapi.exceptions import (
+    FastAPIError,
+    RequestValidationError,
+    WebSocketRequestValidationError,
+)
 from fastapi.types import DecoratedCallable
 from fastapi.utils import (
     create_cloned_field,
     create_response_field,
     generate_unique_id,
     get_value_or_default,
     is_body_allowed_for_status_code,
@@ -44,23 +48,23 @@
 from pydantic.fields import ModelField, Undefined
 from pydantic.utils import lenient_issubclass
 from starlette import routing
 from starlette.concurrency import run_in_threadpool
 from starlette.exceptions import HTTPException
 from starlette.requests import Request
 from starlette.responses import JSONResponse, Response
-from starlette.routing import BaseRoute, Match
-from starlette.routing import Mount as Mount  # noqa
 from starlette.routing import (
+    BaseRoute,
+    Match,
     compile_path,
     get_name,
     request_response,
     websocket_session,
 )
-from starlette.status import WS_1008_POLICY_VIOLATION
+from starlette.routing import Mount as Mount  # noqa
 from starlette.types import ASGIApp, Lifespan, Scope
 from starlette.websockets import WebSocket
 
 
 def _prepare_response_content(
     res: Any,
     *,
@@ -279,36 +283,43 @@
         solved_result = await solve_dependencies(
             request=websocket,
             dependant=dependant,
             dependency_overrides_provider=dependency_overrides_provider,
         )
         values, errors, _, _2, _3 = solved_result
         if errors:
-            await websocket.close(code=WS_1008_POLICY_VIOLATION)
             raise WebSocketRequestValidationError(errors)
         assert dependant.call is not None, "dependant.call must be a function"
         await dependant.call(**values)
 
     return app
 
 
 class APIWebSocketRoute(routing.WebSocketRoute):
     def __init__(
         self,
         path: str,
         endpoint: Callable[..., Any],
         *,
         name: Optional[str] = None,
+        dependencies: Optional[Sequence[params.Depends]] = None,
         dependency_overrides_provider: Optional[Any] = None,
     ) -> None:
         self.path = path
         self.endpoint = endpoint
         self.name = get_name(endpoint) if name is None else name
+        self.dependencies = list(dependencies or [])
         self.path_regex, self.path_format, self.param_convertors = compile_path(path)
         self.dependant = get_dependant(path=self.path_format, call=self.endpoint)
+        for depends in self.dependencies[::-1]:
+            self.dependant.dependencies.insert(
+                0,
+                get_parameterless_sub_dependant(depends=depends, path=self.path_format),
+            )
+
         self.app = websocket_session(
             get_websocket_app(
                 dependant=self.dependant,
                 dependency_overrides_provider=dependency_overrides_provider,
             )
         )
 
@@ -414,18 +425,15 @@
             # will be always created.
             self.secure_cloned_response_field: Optional[
                 ModelField
             ] = create_cloned_field(self.response_field)
         else:
             self.response_field = None  # type: ignore
             self.secure_cloned_response_field = None
-        if dependencies:
-            self.dependencies = list(dependencies)
-        else:
-            self.dependencies = []
+        self.dependencies = list(dependencies or [])
         self.description = description or inspect.cleandoc(self.endpoint.__doc__ or "")
         # if a "form feed" character (page break) is found in the description text,
         # truncate description text to the content preceding the first "form feed"
         self.description = self.description.split("\f")[0].strip()
         response_fields = {}
         for additional_status_code, response in self.responses.items():
             assert isinstance(response, dict), "An additional response must be a dict"
@@ -512,15 +520,15 @@
         if prefix:
             assert prefix.startswith("/"), "A path prefix must start with '/'"
             assert not prefix.endswith(
                 "/"
             ), "A path prefix must not end with '/', as the routes will start with '/'"
         self.prefix = prefix
         self.tags: List[Union[str, Enum]] = tags or []
-        self.dependencies = list(dependencies or []) or []
+        self.dependencies = list(dependencies or [])
         self.deprecated = deprecated
         self.include_in_schema = include_in_schema
         self.responses = responses or {}
         self.callbacks = callbacks or []
         self.dependency_overrides_provider = dependency_overrides_provider
         self.route_class = route_class
         self.default_response_class = default_response_class
@@ -686,29 +694,45 @@
                 generate_unique_id_function=generate_unique_id_function,
             )
             return func
 
         return decorator
 
     def add_api_websocket_route(
-        self, path: str, endpoint: Callable[..., Any], name: Optional[str] = None
+        self,
+        path: str,
+        endpoint: Callable[..., Any],
+        name: Optional[str] = None,
+        *,
+        dependencies: Optional[Sequence[params.Depends]] = None,
     ) -> None:
+        current_dependencies = self.dependencies.copy()
+        if dependencies:
+            current_dependencies.extend(dependencies)
+
         route = APIWebSocketRoute(
             self.prefix + path,
             endpoint=endpoint,
             name=name,
+            dependencies=current_dependencies,
             dependency_overrides_provider=self.dependency_overrides_provider,
         )
         self.routes.append(route)
 
     def websocket(
-        self, path: str, name: Optional[str] = None
+        self,
+        path: str,
+        name: Optional[str] = None,
+        *,
+        dependencies: Optional[Sequence[params.Depends]] = None,
     ) -> Callable[[DecoratedCallable], DecoratedCallable]:
         def decorator(func: DecoratedCallable) -> DecoratedCallable:
-            self.add_api_websocket_route(path, func, name=name)
+            self.add_api_websocket_route(
+                path, func, name=name, dependencies=dependencies
+            )
             return func
 
         return decorator
 
     def websocket_route(
         self, path: str, name: Union[str, None] = None
     ) -> Callable[[DecoratedCallable], DecoratedCallable]:
@@ -740,15 +764,15 @@
                 "/"
             ), "A path prefix must not end with '/', as the routes will start with '/'"
         else:
             for r in router.routes:
                 path = getattr(r, "path")  # noqa: B009
                 name = getattr(r, "name", "unknown")
                 if path is not None and not path:
-                    raise Exception(
+                    raise FastAPIError(
                         f"Prefix and path cannot be both empty (path operation: {name})"
                     )
         if responses is None:
             responses = {}
         for route in router.routes:
             if isinstance(route, APIRoute):
                 combined_responses = {**responses, **route.responses}
@@ -815,16 +839,24 @@
                     prefix + route.path,
                     route.endpoint,
                     methods=methods,
                     include_in_schema=route.include_in_schema,
                     name=route.name,
                 )
             elif isinstance(route, APIWebSocketRoute):
+                current_dependencies = []
+                if dependencies:
+                    current_dependencies.extend(dependencies)
+                if route.dependencies:
+                    current_dependencies.extend(route.dependencies)
                 self.add_api_websocket_route(
-                    prefix + route.path, route.endpoint, name=route.name
+                    prefix + route.path,
+                    route.endpoint,
+                    dependencies=current_dependencies,
+                    name=route.name,
                 )
             elif isinstance(route, routing.WebSocketRoute):
                 self.add_websocket_route(
                     prefix + route.path, route.endpoint, name=route.name
                 )
         for handler in router.on_startup:
             self.add_event_handler("startup", handler)
```

### Comparing `fastapi-0.96.1/fastapi/utils.py` & `fastapi-0.97.0/fastapi/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/fastapi/dependencies/models.py` & `fastapi-0.97.0/fastapi/dependencies/models.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/fastapi/dependencies/utils.py` & `fastapi-0.97.0/fastapi/dependencies/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/fastapi/middleware/asyncexitstack.py` & `fastapi-0.97.0/fastapi/middleware/asyncexitstack.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,23 +6,20 @@
 
 class AsyncExitStackMiddleware:
     def __init__(self, app: ASGIApp, context_name: str = "fastapi_astack") -> None:
         self.app = app
         self.context_name = context_name
 
     async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
-        if AsyncExitStack:
-            dependency_exception: Optional[Exception] = None
-            async with AsyncExitStack() as stack:
-                scope[self.context_name] = stack
-                try:
-                    await self.app(scope, receive, send)
-                except Exception as e:
-                    dependency_exception = e
-                    raise e
-            if dependency_exception:
-                # This exception was possibly handled by the dependency but it should
-                # still bubble up so that the ServerErrorMiddleware can return a 500
-                # or the ExceptionMiddleware can catch and handle any other exceptions
-                raise dependency_exception
-        else:
-            await self.app(scope, receive, send)  # pragma: no cover
+        dependency_exception: Optional[Exception] = None
+        async with AsyncExitStack() as stack:
+            scope[self.context_name] = stack
+            try:
+                await self.app(scope, receive, send)
+            except Exception as e:
+                dependency_exception = e
+                raise e
+        if dependency_exception:
+            # This exception was possibly handled by the dependency but it should
+            # still bubble up so that the ServerErrorMiddleware can return a 500
+            # or the ExceptionMiddleware can catch and handle any other exceptions
+            raise dependency_exception
```

### Comparing `fastapi-0.96.1/fastapi/openapi/docs.py` & `fastapi-0.97.0/fastapi/openapi/docs.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/fastapi/openapi/models.py` & `fastapi-0.97.0/fastapi/openapi/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from enum import Enum
 from typing import Any, Callable, Dict, Iterable, List, Optional, Union
 
 from fastapi.logger import logger
 from pydantic import AnyUrl, BaseModel, Field
+from typing_extensions import Literal
 
 try:
     import email_validator  # type: ignore
 
     assert email_validator  # make autoflake ignore the unused import
     from pydantic import EmailStr
 except ImportError:  # pragma: no cover
@@ -294,26 +295,26 @@
 class APIKeyIn(Enum):
     query = "query"
     header = "header"
     cookie = "cookie"
 
 
 class APIKey(SecurityBase):
-    type_ = Field(SecuritySchemeType.apiKey, alias="type")
+    type_: SecuritySchemeType = Field(default=SecuritySchemeType.apiKey, alias="type")
     in_: APIKeyIn = Field(alias="in")
     name: str
 
 
 class HTTPBase(SecurityBase):
-    type_ = Field(SecuritySchemeType.http, alias="type")
+    type_: SecuritySchemeType = Field(default=SecuritySchemeType.http, alias="type")
     scheme: str
 
 
 class HTTPBearer(HTTPBase):
-    scheme = "bearer"
+    scheme: Literal["bearer"] = "bearer"
     bearerFormat: Optional[str] = None
 
 
 class OAuthFlow(BaseModel):
     refreshUrl: Optional[str] = None
     scopes: Dict[str, str] = {}
 
@@ -345,20 +346,22 @@
     authorizationCode: Optional[OAuthFlowAuthorizationCode] = None
 
     class Config:
         extra = "allow"
 
 
 class OAuth2(SecurityBase):
-    type_ = Field(SecuritySchemeType.oauth2, alias="type")
+    type_: SecuritySchemeType = Field(default=SecuritySchemeType.oauth2, alias="type")
     flows: OAuthFlows
 
 
 class OpenIdConnect(SecurityBase):
-    type_ = Field(SecuritySchemeType.openIdConnect, alias="type")
+    type_: SecuritySchemeType = Field(
+        default=SecuritySchemeType.openIdConnect, alias="type"
+    )
     openIdConnectUrl: str
 
 
 SecurityScheme = Union[APIKey, HTTPBase, OAuth2, OpenIdConnect, HTTPBearer]
 
 
 class Components(BaseModel):
```

### Comparing `fastapi-0.96.1/fastapi/openapi/utils.py` & `fastapi-0.97.0/fastapi/openapi/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
         message = (
             f"Duplicate Operation ID {operation_id} for function "
             + f"{route.endpoint.__name__}"
         )
         file_name = getattr(route.endpoint, "__globals__", {}).get("__file__")
         if file_name:
             message += f" at {file_name}"
-        warnings.warn(message)
+        warnings.warn(message, stacklevel=1)
     operation_ids.add(operation_id)
     operation["operationId"] = operation_id
     if route.deprecated:
         operation["deprecated"] = route.deprecated
     return operation
 
 
@@ -328,18 +328,16 @@
                         or status_text
                         or "Additional Response"
                     )
                     deep_dict_update(openapi_response, process_response)
                     openapi_response["description"] = description
             http422 = str(HTTP_422_UNPROCESSABLE_ENTITY)
             if (all_route_params or route.body_field) and not any(
-                [
-                    status in operation["responses"]
-                    for status in [http422, "4XX", "default"]
-                ]
+                status in operation["responses"]
+                for status in [http422, "4XX", "default"]
             ):
                 operation["responses"][http422] = {
                     "description": "Validation Error",
                     "content": {
                         "application/json": {
                             "schema": {"$ref": REF_PREFIX + "HTTPValidationError"}
                         }
```

### Comparing `fastapi-0.96.1/fastapi/security/__init__.py` & `fastapi-0.97.0/fastapi/security/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/fastapi/security/api_key.py` & `fastapi-0.97.0/fastapi/security/api_key.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,15 +17,17 @@
         *,
         name: str,
         scheme_name: Optional[str] = None,
         description: Optional[str] = None,
         auto_error: bool = True,
     ):
         self.model: APIKey = APIKey(
-            **{"in": APIKeyIn.query}, name=name, description=description
+            **{"in": APIKeyIn.query},  # type: ignore[arg-type]
+            name=name,
+            description=description,
         )
         self.scheme_name = scheme_name or self.__class__.__name__
         self.auto_error = auto_error
 
     async def __call__(self, request: Request) -> Optional[str]:
         api_key = request.query_params.get(self.model.name)
         if not api_key:
@@ -44,15 +46,17 @@
         *,
         name: str,
         scheme_name: Optional[str] = None,
         description: Optional[str] = None,
         auto_error: bool = True,
     ):
         self.model: APIKey = APIKey(
-            **{"in": APIKeyIn.header}, name=name, description=description
+            **{"in": APIKeyIn.header},  # type: ignore[arg-type]
+            name=name,
+            description=description,
         )
         self.scheme_name = scheme_name or self.__class__.__name__
         self.auto_error = auto_error
 
     async def __call__(self, request: Request) -> Optional[str]:
         api_key = request.headers.get(self.model.name)
         if not api_key:
@@ -71,15 +75,17 @@
         *,
         name: str,
         scheme_name: Optional[str] = None,
         description: Optional[str] = None,
         auto_error: bool = True,
     ):
         self.model: APIKey = APIKey(
-            **{"in": APIKeyIn.cookie}, name=name, description=description
+            **{"in": APIKeyIn.cookie},  # type: ignore[arg-type]
+            name=name,
+            description=description,
         )
         self.scheme_name = scheme_name or self.__class__.__name__
         self.auto_error = auto_error
 
     async def __call__(self, request: Request) -> Optional[str]:
         api_key = request.cookies.get(self.model.name)
         if not api_key:
```

### Comparing `fastapi-0.96.1/fastapi/security/http.py` & `fastapi-0.97.0/fastapi/security/http.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/fastapi/security/oauth2.py` & `fastapi-0.97.0/fastapi/security/oauth2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional, Union, cast
 
 from fastapi.exceptions import HTTPException
 from fastapi.openapi.models import OAuth2 as OAuth2Model
 from fastapi.openapi.models import OAuthFlows as OAuthFlowsModel
 from fastapi.param_functions import Form
 from fastapi.security.base import SecurityBase
 from fastapi.security.utils import get_authorization_scheme_param
@@ -117,15 +117,17 @@
         self,
         *,
         flows: Union[OAuthFlowsModel, Dict[str, Dict[str, Any]]] = OAuthFlowsModel(),
         scheme_name: Optional[str] = None,
         description: Optional[str] = None,
         auto_error: bool = True,
     ):
-        self.model = OAuth2Model(flows=flows, description=description)
+        self.model = OAuth2Model(
+            flows=cast(OAuthFlowsModel, flows), description=description
+        )
         self.scheme_name = scheme_name or self.__class__.__name__
         self.auto_error = auto_error
 
     async def __call__(self, request: Request) -> Optional[str]:
         authorization = request.headers.get("Authorization")
         if not authorization:
             if self.auto_error:
@@ -144,15 +146,17 @@
         scheme_name: Optional[str] = None,
         scopes: Optional[Dict[str, str]] = None,
         description: Optional[str] = None,
         auto_error: bool = True,
     ):
         if not scopes:
             scopes = {}
-        flows = OAuthFlowsModel(password={"tokenUrl": tokenUrl, "scopes": scopes})
+        flows = OAuthFlowsModel(
+            password=cast(Any, {"tokenUrl": tokenUrl, "scopes": scopes})
+        )
         super().__init__(
             flows=flows,
             scheme_name=scheme_name,
             description=description,
             auto_error=auto_error,
         )
 
@@ -181,20 +185,23 @@
         scopes: Optional[Dict[str, str]] = None,
         description: Optional[str] = None,
         auto_error: bool = True,
     ):
         if not scopes:
             scopes = {}
         flows = OAuthFlowsModel(
-            authorizationCode={
-                "authorizationUrl": authorizationUrl,
-                "tokenUrl": tokenUrl,
-                "refreshUrl": refreshUrl,
-                "scopes": scopes,
-            }
+            authorizationCode=cast(
+                Any,
+                {
+                    "authorizationUrl": authorizationUrl,
+                    "tokenUrl": tokenUrl,
+                    "refreshUrl": refreshUrl,
+                    "scopes": scopes,
+                },
+            )
         )
         super().__init__(
             flows=flows,
             scheme_name=scheme_name,
             description=description,
             auto_error=auto_error,
         )
```

### Comparing `fastapi-0.96.1/fastapi/security/open_id_connect_url.py` & `fastapi-0.97.0/fastapi/security/open_id_connect_url.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/scripts/docs.py` & `fastapi-0.97.0/scripts/docs.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/scripts/gitter_releases_bot.py` & `fastapi-0.97.0/scripts/gitter_releases_bot.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/main.py` & `fastapi-0.97.0/tests/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_additional_properties.py` & `fastapi-0.97.0/tests/test_additional_properties.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_additional_response_extra.py` & `fastapi-0.97.0/tests/test_additional_response_extra.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_additional_responses_bad.py` & `fastapi-0.97.0/tests/test_additional_responses_bad.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_additional_responses_custom_model_in_callback.py` & `fastapi-0.97.0/tests/test_additional_responses_custom_model_in_callback.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_additional_responses_custom_validationerror.py` & `fastapi-0.97.0/tests/test_additional_responses_custom_validationerror.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_additional_responses_default_validationerror.py` & `fastapi-0.97.0/tests/test_additional_responses_default_validationerror.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_additional_responses_response_class.py` & `fastapi-0.97.0/tests/test_additional_responses_response_class.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_additional_responses_router.py` & `fastapi-0.97.0/tests/test_additional_responses_router.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_ambiguous_params.py` & `fastapi-0.97.0/tests/test_ambiguous_params.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_annotated.py` & `fastapi-0.97.0/tests/test_annotated.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_application.py` & `fastapi-0.97.0/tests/test_application.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_custom_middleware_exception.py` & `fastapi-0.97.0/tests/test_custom_middleware_exception.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_custom_route_class.py` & `fastapi-0.97.0/tests/test_custom_route_class.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_custom_schema_fields.py` & `fastapi-0.97.0/tests/test_custom_schema_fields.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_custom_swagger_ui_redirect.py` & `fastapi-0.97.0/tests/test_custom_swagger_ui_redirect.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_datastructures.py` & `fastapi-0.97.0/tests/test_datastructures.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_datetime_custom_encoder.py` & `fastapi-0.97.0/tests/test_datetime_custom_encoder.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_default_response_class.py` & `fastapi-0.97.0/tests/test_default_response_class.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_default_response_class_router.py` & `fastapi-0.97.0/tests/test_default_response_class_router.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_dependency_cache.py` & `fastapi-0.97.0/tests/test_dependency_cache.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_dependency_class.py` & `fastapi-0.97.0/tests/test_dependency_class.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_dependency_contextmanager.py` & `fastapi-0.97.0/tests/test_dependency_contextmanager.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_dependency_contextvars.py` & `fastapi-0.97.0/tests/test_dependency_contextvars.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_dependency_duplicates.py` & `fastapi-0.97.0/tests/test_dependency_duplicates.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_dependency_normal_exceptions.py` & `fastapi-0.97.0/tests/test_dependency_normal_exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_dependency_overrides.py` & `fastapi-0.97.0/tests/test_dependency_overrides.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_dependency_security_overrides.py` & `fastapi-0.97.0/tests/test_dependency_security_overrides.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_deprecated_openapi_prefix.py` & `fastapi-0.97.0/tests/test_deprecated_openapi_prefix.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_duplicate_models_openapi.py` & `fastapi-0.97.0/tests/test_duplicate_models_openapi.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_empty_router.py` & `fastapi-0.97.0/tests/test_empty_router.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pytest
 from fastapi import APIRouter, FastAPI
+from fastapi.exceptions import FastAPIError
 from fastapi.testclient import TestClient
 
 app = FastAPI()
 
 router = APIRouter()
 
 
@@ -27,9 +28,9 @@
         response = client.get("/prefix/")
         assert response.status_code == 200, response.text
         assert response.json() == ["OK"]
 
 
 def test_include_empty():
     # if both include and router.path are empty - it should raise exception
-    with pytest.raises(Exception):
+    with pytest.raises(FastAPIError):
         app.include_router(router)
```

### Comparing `fastapi-0.96.1/tests/test_enforce_once_required_parameter.py` & `fastapi-0.97.0/tests/test_enforce_once_required_parameter.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_exception_handlers.py` & `fastapi-0.97.0/tests/test_exception_handlers.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_extra_routes.py` & `fastapi-0.97.0/tests/test_extra_routes.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_filter_pydantic_sub_model.py` & `fastapi-0.97.0/tests/test_filter_pydantic_sub_model.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_forms_from_non_typing_sequences.py` & `fastapi-0.97.0/tests/test_forms_from_non_typing_sequences.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_generate_unique_id_function.py` & `fastapi-0.97.0/tests/test_generate_unique_id_function.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_get_request_body.py` & `fastapi-0.97.0/tests/test_get_request_body.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_http_connection_injection.py` & `fastapi-0.97.0/tests/test_http_connection_injection.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_include_router_defaults_overrides.py` & `fastapi-0.97.0/tests/test_include_router_defaults_overrides.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_infer_param_optionality.py` & `fastapi-0.97.0/tests/test_infer_param_optionality.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_inherited_custom_class.py` & `fastapi-0.97.0/tests/test_inherited_custom_class.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_invalid_path_param.py` & `fastapi-0.97.0/tests/test_invalid_path_param.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_invalid_sequence_param.py` & `fastapi-0.97.0/tests/test_invalid_sequence_param.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_jsonable_encoder.py` & `fastapi-0.97.0/tests/test_jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_local_docs.py` & `fastapi-0.97.0/tests/test_local_docs.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_multi_body_errors.py` & `fastapi-0.97.0/tests/test_multi_body_errors.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_multi_query_errors.py` & `fastapi-0.97.0/tests/test_multi_query_errors.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_multipart_installation.py` & `fastapi-0.97.0/tests/test_multipart_installation.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_no_swagger_ui_redirect.py` & `fastapi-0.97.0/tests/test_no_swagger_ui_redirect.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_openapi_query_parameter_extension.py` & `fastapi-0.97.0/tests/test_openapi_query_parameter_extension.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_openapi_route_extensions.py` & `fastapi-0.97.0/tests/test_openapi_route_extensions.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_openapi_servers.py` & `fastapi-0.97.0/tests/test_openapi_servers.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_operations_signatures.py` & `fastapi-0.97.0/tests/test_operations_signatures.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_orjson_response_class.py` & `fastapi-0.97.0/tests/test_orjson_response_class.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_param_class.py` & `fastapi-0.97.0/tests/test_param_class.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_param_in_path_and_dependency.py` & `fastapi-0.97.0/tests/test_param_in_path_and_dependency.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_param_include_in_schema.py` & `fastapi-0.97.0/tests/test_param_include_in_schema.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_params_repr.py` & `fastapi-0.97.0/tests/test_params_repr.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_path.py` & `fastapi-0.97.0/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_put_no_body.py` & `fastapi-0.97.0/tests/test_put_no_body.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_query.py` & `fastapi-0.97.0/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_read_with_orm_mode.py` & `fastapi-0.97.0/tests/test_read_with_orm_mode.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_repeated_cookie_headers.py` & `fastapi-0.97.0/tests/test_repeated_cookie_headers.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_repeated_dependency_schema.py` & `fastapi-0.97.0/tests/test_repeated_dependency_schema.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_repeated_parameter_alias.py` & `fastapi-0.97.0/tests/test_repeated_parameter_alias.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_reponse_set_reponse_code_empty.py` & `fastapi-0.97.0/tests/test_reponse_set_reponse_code_empty.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_request_body_parameters_media_type.py` & `fastapi-0.97.0/tests/test_request_body_parameters_media_type.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_required_noneable.py` & `fastapi-0.97.0/tests/test_required_noneable.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_response_by_alias.py` & `fastapi-0.97.0/tests/test_response_by_alias.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_response_change_status_code.py` & `fastapi-0.97.0/tests/test_response_change_status_code.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_response_class_no_mediatype.py` & `fastapi-0.97.0/tests/test_response_class_no_mediatype.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_response_code_no_body.py` & `fastapi-0.97.0/tests/test_response_code_no_body.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_response_model_as_return_annotation.py` & `fastapi-0.97.0/tests/test_response_model_as_return_annotation.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_response_model_include_exclude.py` & `fastapi-0.97.0/tests/test_response_model_include_exclude.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_response_model_invalid.py` & `fastapi-0.97.0/tests/test_response_model_invalid.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_response_model_sub_types.py` & `fastapi-0.97.0/tests/test_response_model_sub_types.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_route_scope.py` & `fastapi-0.97.0/tests/test_route_scope.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_router_events.py` & `fastapi-0.97.0/tests/test_router_events.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_schema_extra_examples.py` & `fastapi-0.97.0/tests/test_schema_extra_examples.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_security_api_key_cookie.py` & `fastapi-0.97.0/tests/test_security_api_key_cookie.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_security_api_key_cookie_description.py` & `fastapi-0.97.0/tests/test_security_api_key_cookie_description.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_security_api_key_cookie_optional.py` & `fastapi-0.97.0/tests/test_security_api_key_cookie_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_security_api_key_header.py` & `fastapi-0.97.0/tests/test_security_api_key_header.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_security_api_key_header_description.py` & `fastapi-0.97.0/tests/test_security_api_key_header_description.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_security_api_key_header_optional.py` & `fastapi-0.97.0/tests/test_security_api_key_header_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_security_api_key_query.py` & `fastapi-0.97.0/tests/test_security_api_key_query.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_security_api_key_query_description.py` & `fastapi-0.97.0/tests/test_security_api_key_query_description.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_security_api_key_query_optional.py` & `fastapi-0.97.0/tests/test_security_api_key_query_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_security_http_base.py` & `fastapi-0.97.0/tests/test_security_http_base.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_security_http_base_description.py` & `fastapi-0.97.0/tests/test_security_http_base_description.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_security_http_base_optional.py` & `fastapi-0.97.0/tests/test_security_http_base_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_security_http_basic_optional.py` & `fastapi-0.97.0/tests/test_security_http_basic_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_security_http_basic_realm.py` & `fastapi-0.97.0/tests/test_security_http_basic_realm.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_security_http_basic_realm_description.py` & `fastapi-0.97.0/tests/test_security_http_basic_realm_description.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_security_http_bearer.py` & `fastapi-0.97.0/tests/test_security_http_bearer.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_security_http_bearer_description.py` & `fastapi-0.97.0/tests/test_security_http_bearer_description.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_security_http_bearer_optional.py` & `fastapi-0.97.0/tests/test_security_http_bearer_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_security_http_digest.py` & `fastapi-0.97.0/tests/test_security_http_digest.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_security_http_digest_description.py` & `fastapi-0.97.0/tests/test_security_http_digest_description.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_security_http_digest_optional.py` & `fastapi-0.97.0/tests/test_security_http_digest_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_security_oauth2.py` & `fastapi-0.97.0/tests/test_security_oauth2.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_security_oauth2_authorization_code_bearer.py` & `fastapi-0.97.0/tests/test_security_oauth2_authorization_code_bearer.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_security_oauth2_authorization_code_bearer_description.py` & `fastapi-0.97.0/tests/test_security_oauth2_authorization_code_bearer_description.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_security_oauth2_optional.py` & `fastapi-0.97.0/tests/test_security_oauth2_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_security_oauth2_optional_description.py` & `fastapi-0.97.0/tests/test_security_oauth2_optional_description.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_security_oauth2_password_bearer_optional.py` & `fastapi-0.97.0/tests/test_security_oauth2_password_bearer_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_security_oauth2_password_bearer_optional_description.py` & `fastapi-0.97.0/tests/test_security_oauth2_password_bearer_optional_description.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_security_openid_connect.py` & `fastapi-0.97.0/tests/test_security_openid_connect.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_security_openid_connect_description.py` & `fastapi-0.97.0/tests/test_security_openid_connect_description.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_security_openid_connect_optional.py` & `fastapi-0.97.0/tests/test_security_openid_connect_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_serialize_response.py` & `fastapi-0.97.0/tests/test_serialize_response.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_serialize_response_dataclass.py` & `fastapi-0.97.0/tests/test_serialize_response_dataclass.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_serialize_response_model.py` & `fastapi-0.97.0/tests/test_serialize_response_model.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_skip_defaults.py` & `fastapi-0.97.0/tests/test_skip_defaults.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_starlette_exception.py` & `fastapi-0.97.0/tests/test_starlette_exception.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_starlette_urlconvertors.py` & `fastapi-0.97.0/tests/test_starlette_urlconvertors.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_sub_callbacks.py` & `fastapi-0.97.0/tests/test_sub_callbacks.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_swagger_ui_init_oauth.py` & `fastapi-0.97.0/tests/test_swagger_ui_init_oauth.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tuples.py` & `fastapi-0.97.0/tests/test_tuples.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_typing_python39.py` & `fastapi-0.97.0/tests/test_typing_python39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_union_body.py` & `fastapi-0.97.0/tests/test_union_body.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_union_inherited_body.py` & `fastapi-0.97.0/tests/test_union_inherited_body.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_validate_response.py` & `fastapi-0.97.0/tests/test_validate_response.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_validate_response_dataclass.py` & `fastapi-0.97.0/tests/test_validate_response_dataclass.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_validate_response_recursive.py` & `fastapi-0.97.0/tests/test_validate_response_recursive.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_modules_same_name_body/test_main.py` & `fastapi-0.97.0/tests/test_modules_same_name_body/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_additional_responses/test_tutorial001.py` & `fastapi-0.97.0/tests/test_tutorial/test_additional_responses/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_additional_responses/test_tutorial002.py` & `fastapi-0.97.0/tests/test_tutorial/test_additional_responses/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_additional_responses/test_tutorial003.py` & `fastapi-0.97.0/tests/test_tutorial/test_additional_responses/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_additional_responses/test_tutorial004.py` & `fastapi-0.97.0/tests/test_tutorial/test_additional_responses/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_additional_status_codes/test_tutorial001.py` & `fastapi-0.97.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an.py` & `fastapi-0.97.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_advanced_middleware/test_tutorial002.py` & `fastapi-0.97.0/tests/test_tutorial/test_advanced_middleware/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_advanced_middleware/test_tutorial003.py` & `fastapi-0.97.0/tests/test_tutorial/test_advanced_middleware/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_async_sql_databases/test_tutorial001.py` & `fastapi-0.97.0/tests/test_tutorial/test_async_sql_databases/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_background_tasks/test_tutorial001.py` & `fastapi-0.97.0/tests/test_tutorial/test_background_tasks/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_background_tasks/test_tutorial002.py` & `fastapi-0.97.0/tests/test_tutorial/test_background_tasks/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_background_tasks/test_tutorial002_an.py` & `fastapi-0.97.0/tests/test_tutorial/test_background_tasks/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_background_tasks/test_tutorial002_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_background_tasks/test_tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_behind_a_proxy/test_tutorial001.py` & `fastapi-0.97.0/tests/test_tutorial/test_behind_a_proxy/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_behind_a_proxy/test_tutorial002.py` & `fastapi-0.97.0/tests/test_tutorial/test_behind_a_proxy/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_behind_a_proxy/test_tutorial003.py` & `fastapi-0.97.0/tests/test_tutorial/test_behind_a_proxy/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_behind_a_proxy/test_tutorial004.py` & `fastapi-0.97.0/tests/test_tutorial/test_behind_a_proxy/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_bigger_applications/test_main.py` & `fastapi-0.97.0/tests/test_tutorial/test_bigger_applications/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_bigger_applications/test_main_an.py` & `fastapi-0.97.0/tests/test_tutorial/test_bigger_applications/test_main_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_bigger_applications/test_main_an_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_bigger_applications/test_main_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_body/test_tutorial001.py` & `fastapi-0.97.0/tests/test_tutorial/test_body/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_body/test_tutorial001_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_body/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_body_fields/test_tutorial001.py` & `fastapi-0.97.0/tests/test_tutorial/test_body_fields/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_body_fields/test_tutorial001_an.py` & `fastapi-0.97.0/tests/test_tutorial/test_body_fields/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_body_fields/test_tutorial001_an_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_body_fields/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_body_fields/test_tutorial001_an_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_body_fields/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_body_fields/test_tutorial001_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_body_fields/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_body_multiple_params/test_tutorial001.py` & `fastapi-0.97.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an.py` & `fastapi-0.97.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_body_multiple_params/test_tutorial003.py` & `fastapi-0.97.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an.py` & `fastapi-0.97.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_body_nested_models/test_tutorial009.py` & `fastapi-0.97.0/tests/test_tutorial/test_body_nested_models/test_tutorial009.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_body_nested_models/test_tutorial009_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_body_nested_models/test_tutorial009_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_body_updates/test_tutorial001.py` & `fastapi-0.97.0/tests/test_tutorial/test_body_updates/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_body_updates/test_tutorial001_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_body_updates/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_body_updates/test_tutorial001_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_body_updates/test_tutorial001_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_conditional_openapi/test_tutorial001.py` & `fastapi-0.97.0/tests/test_tutorial/test_conditional_openapi/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_cookie_params/test_tutorial001.py` & `fastapi-0.97.0/tests/test_tutorial/test_cookie_params/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_cookie_params/test_tutorial001_an.py` & `fastapi-0.97.0/tests/test_tutorial/test_cookie_params/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_cookie_params/test_tutorial001_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_cookie_params/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_cors/test_tutorial001.py` & `fastapi-0.97.0/tests/test_tutorial/test_cors/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_custom_request_and_route/test_tutorial001.py` & `fastapi-0.97.0/tests/test_tutorial/test_custom_request_and_route/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_custom_request_and_route/test_tutorial002.py` & `fastapi-0.97.0/tests/test_tutorial/test_custom_request_and_route/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_custom_request_and_route/test_tutorial003.py` & `fastapi-0.97.0/tests/test_tutorial/test_custom_request_and_route/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_custom_response/test_tutorial001.py` & `fastapi-0.97.0/tests/test_tutorial/test_custom_response/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_custom_response/test_tutorial001b.py` & `fastapi-0.97.0/tests/test_tutorial/test_custom_response/test_tutorial001b.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_custom_response/test_tutorial004.py` & `fastapi-0.97.0/tests/test_tutorial/test_custom_response/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_custom_response/test_tutorial005.py` & `fastapi-0.97.0/tests/test_tutorial/test_custom_response/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_custom_response/test_tutorial006.py` & `fastapi-0.97.0/tests/test_tutorial/test_custom_response/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_custom_response/test_tutorial006b.py` & `fastapi-0.97.0/tests/test_tutorial/test_custom_response/test_tutorial006b.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_custom_response/test_tutorial006c.py` & `fastapi-0.97.0/tests/test_tutorial/test_custom_response/test_tutorial006c.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_dataclasses/test_tutorial001.py` & `fastapi-0.97.0/tests/test_tutorial/test_dataclasses/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_dataclasses/test_tutorial002.py` & `fastapi-0.97.0/tests/test_tutorial/test_dataclasses/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_dataclasses/test_tutorial003.py` & `fastapi-0.97.0/tests/test_tutorial/test_dataclasses/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_dependencies/test_tutorial001.py` & `fastapi-0.97.0/tests/test_tutorial/test_dependencies/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_dependencies/test_tutorial001_an.py` & `fastapi-0.97.0/tests/test_tutorial/test_dependencies/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_dependencies/test_tutorial001_an_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_dependencies/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_dependencies/test_tutorial001_an_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_dependencies/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_dependencies/test_tutorial001_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_dependencies/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_dependencies/test_tutorial004.py` & `fastapi-0.97.0/tests/test_tutorial/test_dependencies/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_dependencies/test_tutorial004_an.py` & `fastapi-0.97.0/tests/test_tutorial/test_dependencies/test_tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_dependencies/test_tutorial004_an_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_dependencies/test_tutorial004_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_dependencies/test_tutorial004_an_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_dependencies/test_tutorial004_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_dependencies/test_tutorial004_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_dependencies/test_tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_dependencies/test_tutorial006.py` & `fastapi-0.97.0/tests/test_tutorial/test_dependencies/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_dependencies/test_tutorial006_an.py` & `fastapi-0.97.0/tests/test_tutorial/test_dependencies/test_tutorial006_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_dependencies/test_tutorial006_an_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_dependencies/test_tutorial006_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_dependencies/test_tutorial012.py` & `fastapi-0.97.0/tests/test_tutorial/test_dependencies/test_tutorial012.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_dependencies/test_tutorial012_an.py` & `fastapi-0.97.0/tests/test_tutorial/test_dependencies/test_tutorial012_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_dependencies/test_tutorial012_an_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_dependencies/test_tutorial012_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_events/test_tutorial001.py` & `fastapi-0.97.0/tests/test_tutorial/test_events/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_events/test_tutorial002.py` & `fastapi-0.97.0/tests/test_tutorial/test_events/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_events/test_tutorial003.py` & `fastapi-0.97.0/tests/test_tutorial/test_events/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_extending_openapi/test_tutorial001.py` & `fastapi-0.97.0/tests/test_tutorial/test_extending_openapi/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_extending_openapi/test_tutorial002.py` & `fastapi-0.97.0/tests/test_tutorial/test_extending_openapi/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_extending_openapi/test_tutorial003.py` & `fastapi-0.97.0/tests/test_tutorial/test_extending_openapi/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_extending_openapi/test_tutorial004.py` & `fastapi-0.97.0/tests/test_tutorial/test_extending_openapi/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_extending_openapi/test_tutorial005.py` & `fastapi-0.97.0/tests/test_tutorial/test_extending_openapi/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_extra_data_types/test_tutorial001.py` & `fastapi-0.97.0/tests/test_tutorial/test_extra_data_types/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_extra_data_types/test_tutorial001_an.py` & `fastapi-0.97.0/tests/test_tutorial/test_extra_data_types/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_extra_data_types/test_tutorial001_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_extra_data_types/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_extra_models/test_tutorial003.py` & `fastapi-0.97.0/tests/test_tutorial/test_extra_models/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_extra_models/test_tutorial003_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_extra_models/test_tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_extra_models/test_tutorial004.py` & `fastapi-0.97.0/tests/test_tutorial/test_extra_models/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_extra_models/test_tutorial004_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_extra_models/test_tutorial004_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_extra_models/test_tutorial005.py` & `fastapi-0.97.0/tests/test_tutorial/test_extra_models/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_extra_models/test_tutorial005_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_extra_models/test_tutorial005_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_first_steps/test_tutorial001.py` & `fastapi-0.97.0/tests/test_tutorial/test_first_steps/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_generate_clients/test_tutorial003.py` & `fastapi-0.97.0/tests/test_tutorial/test_generate_clients/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_handling_errors/test_tutorial001.py` & `fastapi-0.97.0/tests/test_tutorial/test_handling_errors/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_handling_errors/test_tutorial002.py` & `fastapi-0.97.0/tests/test_tutorial/test_handling_errors/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_handling_errors/test_tutorial003.py` & `fastapi-0.97.0/tests/test_tutorial/test_handling_errors/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_handling_errors/test_tutorial004.py` & `fastapi-0.97.0/tests/test_tutorial/test_handling_errors/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_handling_errors/test_tutorial005.py` & `fastapi-0.97.0/tests/test_tutorial/test_handling_errors/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_handling_errors/test_tutorial006.py` & `fastapi-0.97.0/tests/test_tutorial/test_handling_errors/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_header_params/test_tutorial001.py` & `fastapi-0.97.0/tests/test_tutorial/test_header_params/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_header_params/test_tutorial001_an.py` & `fastapi-0.97.0/tests/test_tutorial/test_header_params/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_header_params/test_tutorial001_an_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_header_params/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_header_params/test_tutorial001_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_header_params/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_header_params/test_tutorial002.py` & `fastapi-0.97.0/tests/test_tutorial/test_header_params/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_header_params/test_tutorial002_an.py` & `fastapi-0.97.0/tests/test_tutorial/test_header_params/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_header_params/test_tutorial002_an_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_header_params/test_tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_header_params/test_tutorial002_an_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_header_params/test_tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_header_params/test_tutorial002_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_header_params/test_tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_header_params/test_tutorial003.py` & `fastapi-0.97.0/tests/test_tutorial/test_header_params/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_header_params/test_tutorial003_an.py` & `fastapi-0.97.0/tests/test_tutorial/test_header_params/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_header_params/test_tutorial003_an_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_header_params/test_tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_header_params/test_tutorial003_an_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_header_params/test_tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_header_params/test_tutorial003_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_header_params/test_tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_metadata/test_tutorial001.py` & `fastapi-0.97.0/tests/test_tutorial/test_metadata/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_metadata/test_tutorial004.py` & `fastapi-0.97.0/tests/test_tutorial/test_metadata/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_openapi_callbacks/test_tutorial001.py` & `fastapi-0.97.0/tests/test_tutorial/test_openapi_callbacks/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial001.py` & `fastapi-0.97.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial002.py` & `fastapi-0.97.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial003.py` & `fastapi-0.97.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial004.py` & `fastapi-0.97.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial005.py` & `fastapi-0.97.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial006.py` & `fastapi-0.97.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial007.py` & `fastapi-0.97.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial007.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_path_operation_configurations/test_tutorial002b.py` & `fastapi-0.97.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial002b.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_path_operation_configurations/test_tutorial005.py` & `fastapi-0.97.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_path_operation_configurations/test_tutorial006.py` & `fastapi-0.97.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_path_params/test_tutorial004.py` & `fastapi-0.97.0/tests/test_tutorial/test_path_params/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_path_params/test_tutorial005.py` & `fastapi-0.97.0/tests/test_tutorial/test_path_params/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_query_params/test_tutorial005.py` & `fastapi-0.97.0/tests/test_tutorial/test_query_params/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_query_params/test_tutorial006.py` & `fastapi-0.97.0/tests/test_tutorial/test_query_params/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_query_params/test_tutorial006_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_query_params/test_tutorial006_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010.py` & `fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an.py` & `fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011.py` & `fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an.py` & `fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012.py` & `fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial012.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an.py` & `fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial013.py` & `fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial013.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an.py` & `fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014.py` & `fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an.py` & `fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_request_files/test_tutorial001.py` & `fastapi-0.97.0/tests/test_tutorial/test_request_files/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_request_files/test_tutorial001_02.py` & `fastapi-0.97.0/tests/test_tutorial/test_request_files/test_tutorial001_02.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_request_files/test_tutorial001_02_an.py` & `fastapi-0.97.0/tests/test_tutorial/test_request_files/test_tutorial001_02_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_request_files/test_tutorial001_02_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_request_files/test_tutorial001_02_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_request_files/test_tutorial001_03.py` & `fastapi-0.97.0/tests/test_tutorial/test_request_files/test_tutorial001_03.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_request_files/test_tutorial001_03_an.py` & `fastapi-0.97.0/tests/test_tutorial/test_request_files/test_tutorial001_03_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_request_files/test_tutorial001_03_an_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_request_files/test_tutorial001_03_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_request_files/test_tutorial001_an.py` & `fastapi-0.97.0/tests/test_tutorial/test_request_files/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_request_files/test_tutorial001_an_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_request_files/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_request_files/test_tutorial002.py` & `fastapi-0.97.0/tests/test_tutorial/test_request_files/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_request_files/test_tutorial002_an.py` & `fastapi-0.97.0/tests/test_tutorial/test_request_files/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_request_files/test_tutorial002_an_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_request_files/test_tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_request_files/test_tutorial002_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_request_files/test_tutorial002_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_request_files/test_tutorial003.py` & `fastapi-0.97.0/tests/test_tutorial/test_request_files/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_request_files/test_tutorial003_an.py` & `fastapi-0.97.0/tests/test_tutorial/test_request_files/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_request_files/test_tutorial003_an_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_request_files/test_tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_request_files/test_tutorial003_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_request_files/test_tutorial003_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_request_forms/test_tutorial001.py` & `fastapi-0.97.0/tests/test_tutorial/test_request_forms/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_request_forms/test_tutorial001_an.py` & `fastapi-0.97.0/tests/test_tutorial/test_request_forms/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_request_forms/test_tutorial001_an_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_request_forms/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_request_forms_and_files/test_tutorial001.py` & `fastapi-0.97.0/tests/test_tutorial/test_request_forms_and_files/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an.py` & `fastapi-0.97.0/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_response_change_status_code/test_tutorial001.py` & `fastapi-0.97.0/tests/test_tutorial/test_response_change_status_code/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_response_model/test_tutorial003.py` & `fastapi-0.97.0/tests/test_tutorial/test_response_model/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_response_model/test_tutorial003_01.py` & `fastapi-0.97.0/tests/test_tutorial/test_response_model/test_tutorial003_01.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_response_model/test_tutorial003_01_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_response_model/test_tutorial003_01_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_response_model/test_tutorial003_02.py` & `fastapi-0.97.0/tests/test_tutorial/test_response_model/test_tutorial003_02.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_response_model/test_tutorial003_03.py` & `fastapi-0.97.0/tests/test_tutorial/test_response_model/test_tutorial003_03.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_response_model/test_tutorial003_05.py` & `fastapi-0.97.0/tests/test_tutorial/test_response_model/test_tutorial003_05.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_response_model/test_tutorial003_05_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_response_model/test_tutorial003_05_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_response_model/test_tutorial003_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_response_model/test_tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_response_model/test_tutorial004.py` & `fastapi-0.97.0/tests/test_tutorial/test_response_model/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_response_model/test_tutorial004_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_response_model/test_tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_response_model/test_tutorial004_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_response_model/test_tutorial004_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_response_model/test_tutorial005.py` & `fastapi-0.97.0/tests/test_tutorial/test_response_model/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_response_model/test_tutorial005_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_response_model/test_tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_response_model/test_tutorial006.py` & `fastapi-0.97.0/tests/test_tutorial/test_response_model/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_response_model/test_tutorial006_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_response_model/test_tutorial006_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_schema_extra_example/test_tutorial004.py` & `fastapi-0.97.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an.py` & `fastapi-0.97.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_security/test_tutorial001.py` & `fastapi-0.97.0/tests/test_tutorial/test_security/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_security/test_tutorial001_an.py` & `fastapi-0.97.0/tests/test_tutorial/test_security/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_security/test_tutorial001_an_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_security/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_security/test_tutorial003.py` & `fastapi-0.97.0/tests/test_tutorial/test_security/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_security/test_tutorial003_an.py` & `fastapi-0.97.0/tests/test_tutorial/test_security/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_security/test_tutorial003_an_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_security/test_tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_security/test_tutorial003_an_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_security/test_tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_security/test_tutorial003_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_security/test_tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_security/test_tutorial005.py` & `fastapi-0.97.0/tests/test_tutorial/test_security/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_security/test_tutorial005_an.py` & `fastapi-0.97.0/tests/test_tutorial/test_security/test_tutorial005_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_security/test_tutorial005_an_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_security/test_tutorial005_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_security/test_tutorial005_an_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_security/test_tutorial005_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_security/test_tutorial005_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_security/test_tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_security/test_tutorial005_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_security/test_tutorial005_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_security/test_tutorial006.py` & `fastapi-0.97.0/tests/test_tutorial/test_security/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_security/test_tutorial006_an.py` & `fastapi-0.97.0/tests/test_tutorial/test_security/test_tutorial006_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_security/test_tutorial006_an_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_security/test_tutorial006_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_sql_databases/test_sql_databases.py` & `fastapi-0.97.0/tests/test_tutorial/test_sql_databases/test_sql_databases.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware.py` & `fastapi-0.97.0/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_sql_databases/test_sql_databases_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_sql_databases/test_sql_databases_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_sql_databases/test_sql_databases_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_sql_databases/test_sql_databases_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_sql_databases/test_testing_databases.py` & `fastapi-0.97.0/tests/test_tutorial/test_sql_databases/test_testing_databases.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_sql_databases/test_testing_databases_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_sql_databases/test_testing_databases_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_sql_databases/test_testing_databases_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_sql_databases/test_testing_databases_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_sql_databases_peewee/test_sql_databases_peewee.py` & `fastapi-0.97.0/tests/test_tutorial/test_sql_databases_peewee/test_sql_databases_peewee.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_sub_applications/test_tutorial001.py` & `fastapi-0.97.0/tests/test_tutorial/test_sub_applications/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_templates/test_tutorial001.py` & `fastapi-0.97.0/tests/test_tutorial/test_templates/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_testing/test_main.py` & `fastapi-0.97.0/tests/test_tutorial/test_testing/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_testing/test_tutorial001.py` & `fastapi-0.97.0/tests/test_tutorial/test_testing/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_testing_dependencies/test_tutorial001.py` & `fastapi-0.97.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an.py` & `fastapi-0.97.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_websockets/test_tutorial001.py` & `fastapi-0.97.0/tests/test_tutorial/test_websockets/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_websockets/test_tutorial002.py` & `fastapi-0.97.0/tests/test_tutorial/test_websockets/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_websockets/test_tutorial002_an.py` & `fastapi-0.97.0/tests/test_tutorial/test_websockets/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_websockets/test_tutorial002_an_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_websockets/test_tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_websockets/test_tutorial002_an_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_websockets/test_tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_websockets/test_tutorial002_py310.py` & `fastapi-0.97.0/tests/test_tutorial/test_websockets/test_tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_websockets/test_tutorial003.py` & `fastapi-0.97.0/tests/test_tutorial/test_websockets/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/tests/test_tutorial/test_websockets/test_tutorial003_py39.py` & `fastapi-0.97.0/tests/test_tutorial/test_websockets/test_tutorial003_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/LICENSE` & `fastapi-0.97.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/README.md` & `fastapi-0.97.0/README.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.96.1/PKG-INFO` & `fastapi-0.97.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6661 7374  : 2.1.Name: fast
 00000020: 6170 690a 5665 7273 696f 6e3a 2030 2e39  api.Version: 0.9
-00000030: 362e 310a 5375 6d6d 6172 793a 2046 6173  6.1.Summary: Fas
+00000030: 372e 300a 5375 6d6d 6172 793a 2046 6173  7.0.Summary: Fas
 00000040: 7441 5049 2066 7261 6d65 776f 726b 2c20  tAPI framework, 
 00000050: 6869 6768 2070 6572 666f 726d 616e 6365  high performance
 00000060: 2c20 6561 7379 2074 6f20 6c65 6172 6e2c  , easy to learn,
 00000070: 2066 6173 7420 746f 2063 6f64 652c 2072   fast to code, r
 00000080: 6561 6479 2066 6f72 2070 726f 6475 6374  eady for product
 00000090: 696f 6e0a 5072 6f6a 6563 742d 5552 4c3a  ion.Project-URL:
 000000a0: 2048 6f6d 6570 6167 652c 2068 7474 7073   Homepage, https
@@ -136,1425 +136,1310 @@
 00000870: 2e31 2e30 2c21 3d34 2e32 2e30 2c21 3d34  .1.0,!=4.2.0,!=4
 00000880: 2e33 2e30 2c21 3d35 2e30 2e30 2c21 3d35  .3.0,!=5.0.0,!=5
 00000890: 2e31 2e30 2c3e 3d34 2e30 2e31 3b20 6578  .1.0,>=4.0.1; ex
 000008a0: 7472 6120 3d3d 2027 616c 6c27 0a52 6571  tra == 'all'.Req
 000008b0: 7569 7265 732d 4469 7374 3a20 7576 6963  uires-Dist: uvic
 000008c0: 6f72 6e5b 7374 616e 6461 7264 5d3e 3d30  orn[standard]>=0
 000008d0: 2e31 322e 303b 2065 7874 7261 203d 3d20  .12.0; extra == 
-000008e0: 2761 6c6c 270a 5072 6f76 6964 6573 2d45  'all'.Provides-E
-000008f0: 7874 7261 3a20 6465 760a 5265 7175 6972  xtra: dev.Requir
-00000900: 6573 2d44 6973 743a 2070 7265 2d63 6f6d  es-Dist: pre-com
-00000910: 6d69 743c 332e 302e 302c 3e3d 322e 3137  mit<3.0.0,>=2.17
-00000920: 2e30 3b20 6578 7472 6120 3d3d 2027 6465  .0; extra == 'de
-00000930: 7627 0a52 6571 7569 7265 732d 4469 7374  v'.Requires-Dist
-00000940: 3a20 7275 6666 3d3d 302e 302e 3133 383b  : ruff==0.0.138;
-00000950: 2065 7874 7261 203d 3d20 2764 6576 270a   extra == 'dev'.
-00000960: 5265 7175 6972 6573 2d44 6973 743a 2075  Requires-Dist: u
-00000970: 7669 636f 726e 5b73 7461 6e64 6172 645d  vicorn[standard]
-00000980: 3c30 2e32 312e 302c 3e3d 302e 3132 2e30  <0.21.0,>=0.12.0
-00000990: 3b20 6578 7472 6120 3d3d 2027 6465 7627  ; extra == 'dev'
-000009a0: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-000009b0: 2064 6f63 0a52 6571 7569 7265 732d 4469   doc.Requires-Di
-000009c0: 7374 3a20 6d64 782d 696e 636c 7564 653c  st: mdx-include<
-000009d0: 322e 302e 302c 3e3d 312e 342e 313b 2065  2.0.0,>=1.4.1; e
-000009e0: 7874 7261 203d 3d20 2764 6f63 270a 5265  xtra == 'doc'.Re
-000009f0: 7175 6972 6573 2d44 6973 743a 206d 6b64  quires-Dist: mkd
-00000a00: 6f63 732d 6d61 726b 646f 776e 6578 7472  ocs-markdownextr
-00000a10: 6164 6174 612d 706c 7567 696e 3c30 2e33  adata-plugin<0.3
-00000a20: 2e30 2c3e 3d30 2e31 2e37 3b20 6578 7472  .0,>=0.1.7; extr
-00000a30: 6120 3d3d 2027 646f 6327 0a52 6571 7569  a == 'doc'.Requi
-00000a40: 7265 732d 4469 7374 3a20 6d6b 646f 6373  res-Dist: mkdocs
-00000a50: 2d6d 6174 6572 6961 6c3c 392e 302e 302c  -material<9.0.0,
-00000a60: 3e3d 382e 312e 343b 2065 7874 7261 203d  >=8.1.4; extra =
-00000a70: 3d20 2764 6f63 270a 5265 7175 6972 6573  = 'doc'.Requires
-00000a80: 2d44 6973 743a 206d 6b64 6f63 733c 322e  -Dist: mkdocs<2.
-00000a90: 302e 302c 3e3d 312e 312e 323b 2065 7874  0.0,>=1.1.2; ext
-00000aa0: 7261 203d 3d20 2764 6f63 270a 5265 7175  ra == 'doc'.Requ
-00000ab0: 6972 6573 2d44 6973 743a 2070 7979 616d  ires-Dist: pyyam
-00000ac0: 6c3c 372e 302e 302c 3e3d 352e 332e 313b  l<7.0.0,>=5.3.1;
-00000ad0: 2065 7874 7261 203d 3d20 2764 6f63 270a   extra == 'doc'.
-00000ae0: 5265 7175 6972 6573 2d44 6973 743a 2074  Requires-Dist: t
-00000af0: 7970 6572 2d63 6c69 3c30 2e30 2e31 342c  yper-cli<0.0.14,
-00000b00: 3e3d 302e 302e 3133 3b20 6578 7472 6120  >=0.0.13; extra 
-00000b10: 3d3d 2027 646f 6327 0a52 6571 7569 7265  == 'doc'.Require
-00000b20: 732d 4469 7374 3a20 7479 7065 725b 616c  s-Dist: typer[al
-00000b30: 6c5d 3c30 2e38 2e30 2c3e 3d30 2e36 2e31  l]<0.8.0,>=0.6.1
-00000b40: 3b20 6578 7472 6120 3d3d 2027 646f 6327  ; extra == 'doc'
-00000b50: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-00000b60: 2074 6573 740a 5265 7175 6972 6573 2d44   test.Requires-D
-00000b70: 6973 743a 2061 6e79 696f 5b74 7269 6f5d  ist: anyio[trio]
-00000b80: 3c34 2e30 2e30 2c3e 3d33 2e32 2e31 3b20  <4.0.0,>=3.2.1; 
-00000b90: 6578 7472 6120 3d3d 2027 7465 7374 270a  extra == 'test'.
-00000ba0: 5265 7175 6972 6573 2d44 6973 743a 2062  Requires-Dist: b
-00000bb0: 6c61 636b 3d3d 3233 2e31 2e30 3b20 6578  lack==23.1.0; ex
-00000bc0: 7472 6120 3d3d 2027 7465 7374 270a 5265  tra == 'test'.Re
-00000bd0: 7175 6972 6573 2d44 6973 743a 2063 6f76  quires-Dist: cov
-00000be0: 6572 6167 655b 746f 6d6c 5d3c 382e 302c  erage[toml]<8.0,
-00000bf0: 3e3d 362e 352e 303b 2065 7874 7261 203d  >=6.5.0; extra =
-00000c00: 3d20 2774 6573 7427 0a52 6571 7569 7265  = 'test'.Require
-00000c10: 732d 4469 7374 3a20 6461 7461 6261 7365  s-Dist: database
-00000c20: 735b 7371 6c69 7465 5d3c 302e 372e 302c  s[sqlite]<0.7.0,
-00000c30: 3e3d 302e 332e 323b 2065 7874 7261 203d  >=0.3.2; extra =
-00000c40: 3d20 2774 6573 7427 0a52 6571 7569 7265  = 'test'.Require
-00000c50: 732d 4469 7374 3a20 656d 6169 6c2d 7661  s-Dist: email-va
-00000c60: 6c69 6461 746f 723c 322e 302e 302c 3e3d  lidator<2.0.0,>=
-00000c70: 312e 312e 313b 2065 7874 7261 203d 3d20  1.1.1; extra == 
-00000c80: 2774 6573 7427 0a52 6571 7569 7265 732d  'test'.Requires-
-00000c90: 4469 7374 3a20 666c 6173 6b3c 332e 302e  Dist: flask<3.0.
-00000ca0: 302c 3e3d 312e 312e 323b 2065 7874 7261  0,>=1.1.2; extra
-00000cb0: 203d 3d20 2774 6573 7427 0a52 6571 7569   == 'test'.Requi
-00000cc0: 7265 732d 4469 7374 3a20 6874 7470 783c  res-Dist: httpx<
-00000cd0: 302e 3234 2e30 2c3e 3d30 2e32 332e 303b  0.24.0,>=0.23.0;
-00000ce0: 2065 7874 7261 203d 3d20 2774 6573 7427   extra == 'test'
-00000cf0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000d00: 6973 6f72 743c 362e 302e 302c 3e3d 352e  isort<6.0.0,>=5.
-00000d10: 302e 363b 2065 7874 7261 203d 3d20 2774  0.6; extra == 't
-00000d20: 6573 7427 0a52 6571 7569 7265 732d 4469  est'.Requires-Di
-00000d30: 7374 3a20 6d79 7079 3d3d 302e 3938 323b  st: mypy==0.982;
-00000d40: 2065 7874 7261 203d 3d20 2774 6573 7427   extra == 'test'
-00000d50: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000d60: 6f72 6a73 6f6e 3c34 2e30 2e30 2c3e 3d33  orjson<4.0.0,>=3
-00000d70: 2e32 2e31 3b20 6578 7472 6120 3d3d 2027  .2.1; extra == '
-00000d80: 7465 7374 270a 5265 7175 6972 6573 2d44  test'.Requires-D
-00000d90: 6973 743a 2070 6173 736c 6962 5b62 6372  ist: passlib[bcr
-00000da0: 7970 745d 3c32 2e30 2e30 2c3e 3d31 2e37  ypt]<2.0.0,>=1.7
-00000db0: 2e32 3b20 6578 7472 6120 3d3d 2027 7465  .2; extra == 'te
-00000dc0: 7374 270a 5265 7175 6972 6573 2d44 6973  st'.Requires-Dis
-00000dd0: 743a 2070 6565 7765 653c 342e 302e 302c  t: peewee<4.0.0,
-00000de0: 3e3d 332e 3133 2e33 3b20 6578 7472 6120  >=3.13.3; extra 
-00000df0: 3d3d 2027 7465 7374 270a 5265 7175 6972  == 'test'.Requir
-00000e00: 6573 2d44 6973 743a 2070 7974 6573 743c  es-Dist: pytest<
-00000e10: 382e 302e 302c 3e3d 372e 312e 333b 2065  8.0.0,>=7.1.3; e
-00000e20: 7874 7261 203d 3d20 2774 6573 7427 0a52  xtra == 'test'.R
-00000e30: 6571 7569 7265 732d 4469 7374 3a20 7079  equires-Dist: py
-00000e40: 7468 6f6e 2d6a 6f73 655b 6372 7970 746f  thon-jose[crypto
-00000e50: 6772 6170 6879 5d3c 342e 302e 302c 3e3d  graphy]<4.0.0,>=
-00000e60: 332e 332e 303b 2065 7874 7261 203d 3d20  3.3.0; extra == 
-00000e70: 2774 6573 7427 0a52 6571 7569 7265 732d  'test'.Requires-
-00000e80: 4469 7374 3a20 7079 7468 6f6e 2d6d 756c  Dist: python-mul
-00000e90: 7469 7061 7274 3c30 2e30 2e37 2c3e 3d30  tipart<0.0.7,>=0
-00000ea0: 2e30 2e35 3b20 6578 7472 6120 3d3d 2027  .0.5; extra == '
-00000eb0: 7465 7374 270a 5265 7175 6972 6573 2d44  test'.Requires-D
-00000ec0: 6973 743a 2070 7979 616d 6c3c 372e 302e  ist: pyyaml<7.0.
-00000ed0: 302c 3e3d 352e 332e 313b 2065 7874 7261  0,>=5.3.1; extra
-00000ee0: 203d 3d20 2774 6573 7427 0a52 6571 7569   == 'test'.Requi
-00000ef0: 7265 732d 4469 7374 3a20 7275 6666 3d3d  res-Dist: ruff==
-00000f00: 302e 302e 3133 383b 2065 7874 7261 203d  0.0.138; extra =
-00000f10: 3d20 2774 6573 7427 0a52 6571 7569 7265  = 'test'.Require
-00000f20: 732d 4469 7374 3a20 7371 6c61 6c63 6865  s-Dist: sqlalche
-00000f30: 6d79 3c31 2e34 2e34 332c 3e3d 312e 332e  my<1.4.43,>=1.3.
-00000f40: 3138 3b20 6578 7472 6120 3d3d 2027 7465  18; extra == 'te
-00000f50: 7374 270a 5265 7175 6972 6573 2d44 6973  st'.Requires-Dis
-00000f60: 743a 2074 7970 6573 2d6f 726a 736f 6e3d  t: types-orjson=
-00000f70: 3d33 2e36 2e32 3b20 6578 7472 6120 3d3d  =3.6.2; extra ==
-00000f80: 2027 7465 7374 270a 5265 7175 6972 6573   'test'.Requires
-00000f90: 2d44 6973 743a 2074 7970 6573 2d75 6a73  -Dist: types-ujs
-00000fa0: 6f6e 3d3d 352e 372e 302e 313b 2065 7874  on==5.7.0.1; ext
-00000fb0: 7261 203d 3d20 2774 6573 7427 0a52 6571  ra == 'test'.Req
-00000fc0: 7569 7265 732d 4469 7374 3a20 756a 736f  uires-Dist: ujso
-00000fd0: 6e21 3d34 2e30 2e32 2c21 3d34 2e31 2e30  n!=4.0.2,!=4.1.0
-00000fe0: 2c21 3d34 2e32 2e30 2c21 3d34 2e33 2e30  ,!=4.2.0,!=4.3.0
-00000ff0: 2c21 3d35 2e30 2e30 2c21 3d35 2e31 2e30  ,!=5.0.0,!=5.1.0
-00001000: 2c3c 362e 302e 302c 3e3d 342e 302e 313b  ,<6.0.0,>=4.0.1;
-00001010: 2065 7874 7261 203d 3d20 2774 6573 7427   extra == 'test'
-00001020: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
-00001030: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
-00001040: 6d61 726b 646f 776e 0a0a 3c70 2061 6c69  markdown..<p ali
-00001050: 676e 3d22 6365 6e74 6572 223e 0a20 203c  gn="center">.  <
-00001060: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00001070: 6661 7374 6170 692e 7469 616e 676f 6c6f  fastapi.tiangolo
-00001080: 2e63 6f6d 223e 3c69 6d67 2073 7263 3d22  .com"><img src="
-00001090: 6874 7470 733a 2f2f 6661 7374 6170 692e  https://fastapi.
-000010a0: 7469 616e 676f 6c6f 2e63 6f6d 2f69 6d67  tiangolo.com/img
-000010b0: 2f6c 6f67 6f2d 6d61 7267 696e 2f6c 6f67  /logo-margin/log
-000010c0: 6f2d 7465 616c 2e70 6e67 2220 616c 743d  o-teal.png" alt=
-000010d0: 2246 6173 7441 5049 223e 3c2f 613e 0a3c  "FastAPI"></a>.<
-000010e0: 2f70 3e0a 3c70 2061 6c69 676e 3d22 6365  /p>.<p align="ce
-000010f0: 6e74 6572 223e 0a20 2020 203c 656d 3e46  nter">.    <em>F
-00001100: 6173 7441 5049 2066 7261 6d65 776f 726b  astAPI framework
-00001110: 2c20 6869 6768 2070 6572 666f 726d 616e  , high performan
-00001120: 6365 2c20 6561 7379 2074 6f20 6c65 6172  ce, easy to lear
-00001130: 6e2c 2066 6173 7420 746f 2063 6f64 652c  n, fast to code,
-00001140: 2072 6561 6479 2066 6f72 2070 726f 6475   ready for produ
-00001150: 6374 696f 6e3c 2f65 6d3e 0a3c 2f70 3e0a  ction</em>.</p>.
-00001160: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
-00001170: 223e 0a3c 6120 6872 6566 3d22 6874 7470  ">.<a href="http
-00001180: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f74  s://github.com/t
-00001190: 6961 6e67 6f6c 6f2f 6661 7374 6170 692f  iangolo/fastapi/
-000011a0: 6163 7469 6f6e 733f 7175 6572 793d 776f  actions?query=wo
-000011b0: 726b 666c 6f77 2533 4154 6573 742b 6576  rkflow%3ATest+ev
-000011c0: 656e 7425 3341 7075 7368 2b62 7261 6e63  ent%3Apush+branc
-000011d0: 6825 3341 6d61 7374 6572 2220 7461 7267  h%3Amaster" targ
-000011e0: 6574 3d22 5f62 6c61 6e6b 223e 0a20 2020  et="_blank">.   
-000011f0: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
-00001200: 3a2f 2f67 6974 6875 622e 636f 6d2f 7469  ://github.com/ti
-00001210: 616e 676f 6c6f 2f66 6173 7461 7069 2f77  angolo/fastapi/w
-00001220: 6f72 6b66 6c6f 7773 2f54 6573 742f 6261  orkflows/Test/ba
-00001230: 6467 652e 7376 673f 6576 656e 743d 7075  dge.svg?event=pu
-00001240: 7368 2662 7261 6e63 683d 6d61 7374 6572  sh&branch=master
-00001250: 2220 616c 743d 2254 6573 7422 3e0a 3c2f  " alt="Test">.</
-00001260: 613e 0a3c 6120 6872 6566 3d22 6874 7470  a>.<a href="http
-00001270: 733a 2f2f 636f 7665 7261 6765 2d62 6164  s://coverage-bad
-00001280: 6765 2e73 616d 7565 6c63 6f6c 7669 6e2e  ge.samuelcolvin.
-00001290: 776f 726b 6572 732e 6465 762f 7265 6469  workers.dev/redi
-000012a0: 7265 6374 2f74 6961 6e67 6f6c 6f2f 6661  rect/tiangolo/fa
-000012b0: 7374 6170 6922 2074 6172 6765 743d 225f  stapi" target="_
-000012c0: 626c 616e 6b22 3e0a 2020 2020 3c69 6d67  blank">.    <img
-000012d0: 2073 7263 3d22 6874 7470 733a 2f2f 636f   src="https://co
-000012e0: 7665 7261 6765 2d62 6164 6765 2e73 616d  verage-badge.sam
-000012f0: 7565 6c63 6f6c 7669 6e2e 776f 726b 6572  uelcolvin.worker
-00001300: 732e 6465 762f 7469 616e 676f 6c6f 2f66  s.dev/tiangolo/f
-00001310: 6173 7461 7069 2e73 7667 2220 616c 743d  astapi.svg" alt=
-00001320: 2243 6f76 6572 6167 6522 3e0a 3c2f 613e  "Coverage">.</a>
-00001330: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
-00001340: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
-00001350: 6374 2f66 6173 7461 7069 2220 7461 7267  ct/fastapi" targ
-00001360: 6574 3d22 5f62 6c61 6e6b 223e 0a20 2020  et="_blank">.   
-00001370: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
-00001380: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00001390: 6f2f 7079 7069 2f76 2f66 6173 7461 7069  o/pypi/v/fastapi
-000013a0: 3f63 6f6c 6f72 3d25 3233 3334 4430 3538  ?color=%2334D058
-000013b0: 266c 6162 656c 3d70 7970 6925 3230 7061  &label=pypi%20pa
-000013c0: 636b 6167 6522 2061 6c74 3d22 5061 636b  ckage" alt="Pack
-000013d0: 6167 6520 7665 7273 696f 6e22 3e0a 3c2f  age version">.</
-000013e0: 613e 0a3c 6120 6872 6566 3d22 6874 7470  a>.<a href="http
-000013f0: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
-00001400: 6a65 6374 2f66 6173 7461 7069 2220 7461  ject/fastapi" ta
-00001410: 7267 6574 3d22 5f62 6c61 6e6b 223e 0a20  rget="_blank">. 
-00001420: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
-00001430: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00001440: 2e69 6f2f 7079 7069 2f70 7976 6572 7369  .io/pypi/pyversi
-00001450: 6f6e 732f 6661 7374 6170 692e 7376 673f  ons/fastapi.svg?
-00001460: 636f 6c6f 723d 2532 3333 3444 3035 3822  color=%2334D058"
-00001470: 2061 6c74 3d22 5375 7070 6f72 7465 6420   alt="Supported 
-00001480: 5079 7468 6f6e 2076 6572 7369 6f6e 7322  Python versions"
-00001490: 3e0a 3c2f 613e 0a3c 2f70 3e0a 0a2d 2d2d  >.</a>.</p>..---
-000014a0: 0a0a 2a2a 446f 6375 6d65 6e74 6174 696f  ..**Documentatio
-000014b0: 6e2a 2a3a 203c 6120 6872 6566 3d22 6874  n**: <a href="ht
-000014c0: 7470 733a 2f2f 6661 7374 6170 692e 7469  tps://fastapi.ti
-000014d0: 616e 676f 6c6f 2e63 6f6d 2220 7461 7267  angolo.com" targ
-000014e0: 6574 3d22 5f62 6c61 6e6b 223e 6874 7470  et="_blank">http
-000014f0: 733a 2f2f 6661 7374 6170 692e 7469 616e  s://fastapi.tian
-00001500: 676f 6c6f 2e63 6f6d 3c2f 613e 0a0a 2a2a  golo.com</a>..**
-00001510: 536f 7572 6365 2043 6f64 652a 2a3a 203c  Source Code**: <
-00001520: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00001530: 6769 7468 7562 2e63 6f6d 2f74 6961 6e67  github.com/tiang
-00001540: 6f6c 6f2f 6661 7374 6170 6922 2074 6172  olo/fastapi" tar
-00001550: 6765 743d 225f 626c 616e 6b22 3e68 7474  get="_blank">htt
-00001560: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001570: 7469 616e 676f 6c6f 2f66 6173 7461 7069  tiangolo/fastapi
-00001580: 3c2f 613e 0a0a 2d2d 2d0a 0a46 6173 7441  </a>..---..FastA
-00001590: 5049 2069 7320 6120 6d6f 6465 726e 2c20  PI is a modern, 
-000015a0: 6661 7374 2028 6869 6768 2d70 6572 666f  fast (high-perfo
-000015b0: 726d 616e 6365 292c 2077 6562 2066 7261  rmance), web fra
-000015c0: 6d65 776f 726b 2066 6f72 2062 7569 6c64  mework for build
-000015d0: 696e 6720 4150 4973 2077 6974 6820 5079  ing APIs with Py
-000015e0: 7468 6f6e 2033 2e37 2b20 6261 7365 6420  thon 3.7+ based 
-000015f0: 6f6e 2073 7461 6e64 6172 6420 5079 7468  on standard Pyth
-00001600: 6f6e 2074 7970 6520 6869 6e74 732e 0a0a  on type hints...
-00001610: 5468 6520 6b65 7920 6665 6174 7572 6573  The key features
-00001620: 2061 7265 3a0a 0a2a 202a 2a46 6173 742a   are:..* **Fast*
-00001630: 2a3a 2056 6572 7920 6869 6768 2070 6572  *: Very high per
-00001640: 666f 726d 616e 6365 2c20 6f6e 2070 6172  formance, on par
-00001650: 2077 6974 6820 2a2a 4e6f 6465 4a53 2a2a   with **NodeJS**
-00001660: 2061 6e64 202a 2a47 6f2a 2a20 2874 6861   and **Go** (tha
-00001670: 6e6b 7320 746f 2053 7461 726c 6574 7465  nks to Starlette
-00001680: 2061 6e64 2050 7964 616e 7469 6329 2e20   and Pydantic). 
-00001690: 5b4f 6e65 206f 6620 7468 6520 6661 7374  [One of the fast
-000016a0: 6573 7420 5079 7468 6f6e 2066 7261 6d65  est Python frame
-000016b0: 776f 726b 7320 6176 6169 6c61 626c 655d  works available]
-000016c0: 2823 7065 7266 6f72 6d61 6e63 6529 2e0a  (#performance)..
-000016d0: 2a20 2a2a 4661 7374 2074 6f20 636f 6465  * **Fast to code
-000016e0: 2a2a 3a20 496e 6372 6561 7365 2074 6865  **: Increase the
-000016f0: 2073 7065 6564 2074 6f20 6465 7665 6c6f   speed to develo
-00001700: 7020 6665 6174 7572 6573 2062 7920 6162  p features by ab
-00001710: 6f75 7420 3230 3025 2074 6f20 3330 3025  out 200% to 300%
-00001720: 2e20 2a0a 2a20 2a2a 4665 7765 7220 6275  . *.* **Fewer bu
-00001730: 6773 2a2a 3a20 5265 6475 6365 2061 626f  gs**: Reduce abo
-00001740: 7574 2034 3025 206f 6620 6875 6d61 6e20  ut 40% of human 
-00001750: 2864 6576 656c 6f70 6572 2920 696e 6475  (developer) indu
-00001760: 6365 6420 6572 726f 7273 2e20 2a0a 2a20  ced errors. *.* 
-00001770: 2a2a 496e 7475 6974 6976 652a 2a3a 2047  **Intuitive**: G
-00001780: 7265 6174 2065 6469 746f 7220 7375 7070  reat editor supp
-00001790: 6f72 742e 203c 6162 6272 2074 6974 6c65  ort. <abbr title
-000017a0: 3d22 616c 736f 206b 6e6f 776e 2061 7320  ="also known as 
-000017b0: 6175 746f 2d63 6f6d 706c 6574 652c 2061  auto-complete, a
-000017c0: 7574 6f63 6f6d 706c 6574 696f 6e2c 2049  utocompletion, I
-000017d0: 6e74 656c 6c69 5365 6e73 6522 3e43 6f6d  ntelliSense">Com
-000017e0: 706c 6574 696f 6e3c 2f61 6262 723e 2065  pletion</abbr> e
-000017f0: 7665 7279 7768 6572 652e 204c 6573 7320  verywhere. Less 
-00001800: 7469 6d65 2064 6562 7567 6769 6e67 2e0a  time debugging..
-00001810: 2a20 2a2a 4561 7379 2a2a 3a20 4465 7369  * **Easy**: Desi
-00001820: 676e 6564 2074 6f20 6265 2065 6173 7920  gned to be easy 
-00001830: 746f 2075 7365 2061 6e64 206c 6561 726e  to use and learn
-00001840: 2e20 4c65 7373 2074 696d 6520 7265 6164  . Less time read
-00001850: 696e 6720 646f 6373 2e0a 2a20 2a2a 5368  ing docs..* **Sh
-00001860: 6f72 742a 2a3a 204d 696e 696d 697a 6520  ort**: Minimize 
-00001870: 636f 6465 2064 7570 6c69 6361 7469 6f6e  code duplication
-00001880: 2e20 4d75 6c74 6970 6c65 2066 6561 7475  . Multiple featu
-00001890: 7265 7320 6672 6f6d 2065 6163 6820 7061  res from each pa
-000018a0: 7261 6d65 7465 7220 6465 636c 6172 6174  rameter declarat
-000018b0: 696f 6e2e 2046 6577 6572 2062 7567 732e  ion. Fewer bugs.
-000018c0: 0a2a 202a 2a52 6f62 7573 742a 2a3a 2047  .* **Robust**: G
-000018d0: 6574 2070 726f 6475 6374 696f 6e2d 7265  et production-re
-000018e0: 6164 7920 636f 6465 2e20 5769 7468 2061  ady code. With a
-000018f0: 7574 6f6d 6174 6963 2069 6e74 6572 6163  utomatic interac
-00001900: 7469 7665 2064 6f63 756d 656e 7461 7469  tive documentati
-00001910: 6f6e 2e0a 2a20 2a2a 5374 616e 6461 7264  on..* **Standard
-00001920: 732d 6261 7365 642a 2a3a 2042 6173 6564  s-based**: Based
-00001930: 206f 6e20 2861 6e64 2066 756c 6c79 2063   on (and fully c
-00001940: 6f6d 7061 7469 626c 6520 7769 7468 2920  ompatible with) 
-00001950: 7468 6520 6f70 656e 2073 7461 6e64 6172  the open standar
-00001960: 6473 2066 6f72 2041 5049 733a 203c 6120  ds for APIs: <a 
-00001970: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
-00001980: 7468 7562 2e63 6f6d 2f4f 4149 2f4f 7065  thub.com/OAI/Ope
-00001990: 6e41 5049 2d53 7065 6369 6669 6361 7469  nAPI-Specificati
-000019a0: 6f6e 2220 636c 6173 733d 2265 7874 6572  on" class="exter
-000019b0: 6e61 6c2d 6c69 6e6b 2220 7461 7267 6574  nal-link" target
-000019c0: 3d22 5f62 6c61 6e6b 223e 4f70 656e 4150  ="_blank">OpenAP
-000019d0: 493c 2f61 3e20 2870 7265 7669 6f75 736c  I</a> (previousl
-000019e0: 7920 6b6e 6f77 6e20 6173 2053 7761 6767  y known as Swagg
-000019f0: 6572 2920 616e 6420 3c61 2068 7265 663d  er) and <a href=
-00001a00: 2268 7474 7073 3a2f 2f6a 736f 6e2d 7363  "https://json-sc
-00001a10: 6865 6d61 2e6f 7267 2f22 2063 6c61 7373  hema.org/" class
-00001a20: 3d22 6578 7465 726e 616c 2d6c 696e 6b22  ="external-link"
-00001a30: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
-00001a40: 3e4a 534f 4e20 5363 6865 6d61 3c2f 613e  >JSON Schema</a>
-00001a50: 2e0a 0a3c 736d 616c 6c3e 2a20 6573 7469  ...<small>* esti
-00001a60: 6d61 7469 6f6e 2062 6173 6564 206f 6e20  mation based on 
-00001a70: 7465 7374 7320 6f6e 2061 6e20 696e 7465  tests on an inte
-00001a80: 726e 616c 2064 6576 656c 6f70 6d65 6e74  rnal development
-00001a90: 2074 6561 6d2c 2062 7569 6c64 696e 6720   team, building 
-00001aa0: 7072 6f64 7563 7469 6f6e 2061 7070 6c69  production appli
-00001ab0: 6361 7469 6f6e 732e 3c2f 736d 616c 6c3e  cations.</small>
-00001ac0: 0a0a 2323 2053 706f 6e73 6f72 730a 0a3c  ..## Sponsors..<
-00001ad0: 212d 2d20 7370 6f6e 736f 7273 202d 2d3e  !-- sponsors -->
-00001ae0: 0a0a 3c61 2068 7265 663d 2268 7474 7073  ..<a href="https
-00001af0: 3a2f 2f63 7279 7074 6170 692e 696f 2f22  ://cryptapi.io/"
-00001b00: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
-00001b10: 2074 6974 6c65 3d22 4372 7970 7441 5049   title="CryptAPI
-00001b20: 3a20 596f 7572 2065 6173 7920 746f 2075  : Your easy to u
-00001b30: 7365 2c20 7365 6375 7265 2061 6e64 2070  se, secure and p
-00001b40: 7269 7661 6379 206f 7269 656e 7465 6420  rivacy oriented 
-00001b50: 7061 796d 656e 7420 6761 7465 7761 792e  payment gateway.
-00001b60: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
-00001b70: 733a 2f2f 6661 7374 6170 692e 7469 616e  s://fastapi.tian
-00001b80: 676f 6c6f 2e63 6f6d 2f69 6d67 2f73 706f  golo.com/img/spo
-00001b90: 6e73 6f72 732f 6372 7970 7461 7069 2e73  nsors/cryptapi.s
-00001ba0: 7667 223e 3c2f 613e 0a3c 6120 6872 6566  vg"></a>.<a href
-00001bb0: 3d22 6874 7470 733a 2f2f 706c 6174 666f  ="https://platfo
-00001bc0: 726d 2e73 682f 7472 792d 6974 2d6e 6f77  rm.sh/try-it-now
-00001bd0: 2f3f 7574 6d5f 736f 7572 6365 3d66 6173  /?utm_source=fas
-00001be0: 7461 7069 2d73 6967 6e75 7026 7574 6d5f  tapi-signup&utm_
-00001bf0: 6d65 6469 756d 3d62 616e 6e65 7226 7574  medium=banner&ut
-00001c00: 6d5f 6361 6d70 6169 676e 3d46 6173 7441  m_campaign=FastA
-00001c10: 5049 2d73 6967 6e75 702d 4a75 6e65 2d32  PI-signup-June-2
-00001c20: 3032 3322 2074 6172 6765 743d 225f 626c  023" target="_bl
-00001c30: 616e 6b22 2074 6974 6c65 3d22 4275 696c  ank" title="Buil
-00001c40: 642c 2072 756e 2061 6e64 2073 6361 6c65  d, run and scale
-00001c50: 2079 6f75 7220 6170 7073 206f 6e20 6120   your apps on a 
-00001c60: 6d6f 6465 726e 2c20 7265 6c69 6162 6c65  modern, reliable
-00001c70: 2c20 616e 6420 7365 6375 7265 2050 6161  , and secure Paa
-00001c80: 532e 223e 3c69 6d67 2073 7263 3d22 6874  S."><img src="ht
-00001c90: 7470 733a 2f2f 6661 7374 6170 692e 7469  tps://fastapi.ti
-00001ca0: 616e 676f 6c6f 2e63 6f6d 2f69 6d67 2f73  angolo.com/img/s
-00001cb0: 706f 6e73 6f72 732f 706c 6174 666f 726d  ponsors/platform
-00001cc0: 2d73 682e 706e 6722 3e3c 2f61 3e0a 3c61  -sh.png"></a>.<a
-00001cd0: 2068 7265 663d 2268 7474 7073 3a2f 2f77   href="https://w
-00001ce0: 7777 2e64 6574 612e 7368 2f3f 7265 663d  ww.deta.sh/?ref=
-00001cf0: 6661 7374 6170 6922 2074 6172 6765 743d  fastapi" target=
-00001d00: 225f 626c 616e 6b22 2074 6974 6c65 3d22  "_blank" title="
-00001d10: 5468 6520 6c61 756e 6368 7061 6420 666f  The launchpad fo
-00001d20: 7220 616c 6c20 796f 7572 2028 7465 616d  r all your (team
-00001d30: 2773 2920 6964 6561 7322 3e3c 696d 6720  's) ideas"><img 
-00001d40: 7372 633d 2268 7474 7073 3a2f 2f66 6173  src="https://fas
-00001d50: 7461 7069 2e74 6961 6e67 6f6c 6f2e 636f  tapi.tiangolo.co
-00001d60: 6d2f 696d 672f 7370 6f6e 736f 7273 2f64  m/img/sponsors/d
-00001d70: 6574 612e 7376 6722 3e3c 2f61 3e0a 3c61  eta.svg"></a>.<a
-00001d80: 2068 7265 663d 2268 7474 7073 3a2f 2f74   href="https://t
-00001d90: 7261 696e 696e 672e 7461 6c6b 7079 7468  raining.talkpyth
-00001da0: 6f6e 2e66 6d2f 6661 7374 6170 692d 636f  on.fm/fastapi-co
-00001db0: 7572 7365 7322 2074 6172 6765 743d 225f  urses" target="_
-00001dc0: 626c 616e 6b22 2074 6974 6c65 3d22 4661  blank" title="Fa
-00001dd0: 7374 4150 4920 7669 6465 6f20 636f 7572  stAPI video cour
-00001de0: 7365 7320 6f6e 2064 656d 616e 6420 6672  ses on demand fr
-00001df0: 6f6d 2070 656f 706c 6520 796f 7520 7472  om people you tr
-00001e00: 7573 7422 3e3c 696d 6720 7372 633d 2268  ust"><img src="h
-00001e10: 7474 7073 3a2f 2f66 6173 7461 7069 2e74  ttps://fastapi.t
-00001e20: 6961 6e67 6f6c 6f2e 636f 6d2f 696d 672f  iangolo.com/img/
-00001e30: 7370 6f6e 736f 7273 2f74 616c 6b70 7974  sponsors/talkpyt
-00001e40: 686f 6e2e 706e 6722 3e3c 2f61 3e0a 3c61  hon.png"></a>.<a
-00001e50: 2068 7265 663d 2268 7474 7073 3a2f 2f74   href="https://t
-00001e60: 6573 7464 7269 7665 6e2e 696f 2f63 6f75  estdriven.io/cou
-00001e70: 7273 6573 2f74 6464 2d66 6173 7461 7069  rses/tdd-fastapi
-00001e80: 2f22 2074 6172 6765 743d 225f 626c 616e  /" target="_blan
-00001e90: 6b22 2074 6974 6c65 3d22 4c65 6172 6e20  k" title="Learn 
-00001ea0: 746f 2062 7569 6c64 2068 6967 682d 7175  to build high-qu
-00001eb0: 616c 6974 7920 7765 6220 6170 7073 2077  ality web apps w
-00001ec0: 6974 6820 6265 7374 2070 7261 6374 6963  ith best practic
-00001ed0: 6573 223e 3c69 6d67 2073 7263 3d22 6874  es"><img src="ht
-00001ee0: 7470 733a 2f2f 6661 7374 6170 692e 7469  tps://fastapi.ti
-00001ef0: 616e 676f 6c6f 2e63 6f6d 2f69 6d67 2f73  angolo.com/img/s
-00001f00: 706f 6e73 6f72 732f 7465 7374 6472 6976  ponsors/testdriv
-00001f10: 656e 2e73 7667 223e 3c2f 613e 0a3c 6120  en.svg"></a>.<a 
-00001f20: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
-00001f30: 7468 7562 2e63 6f6d 2f64 6565 7073 6574  thub.com/deepset
-00001f40: 2d61 692f 6861 7973 7461 636b 2f22 2074  -ai/haystack/" t
-00001f50: 6172 6765 743d 225f 626c 616e 6b22 2074  arget="_blank" t
-00001f60: 6974 6c65 3d22 4275 696c 6420 706f 7765  itle="Build powe
-00001f70: 7266 756c 2073 6561 7263 6820 6672 6f6d  rful search from
-00001f80: 2063 6f6d 706f 7361 626c 652c 206f 7065   composable, ope
-00001f90: 6e20 736f 7572 6365 2062 7569 6c64 696e  n source buildin
-00001fa0: 6720 626c 6f63 6b73 223e 3c69 6d67 2073  g blocks"><img s
-00001fb0: 7263 3d22 6874 7470 733a 2f2f 6661 7374  rc="https://fast
-00001fc0: 6170 692e 7469 616e 676f 6c6f 2e63 6f6d  api.tiangolo.com
-00001fd0: 2f69 6d67 2f73 706f 6e73 6f72 732f 6861  /img/sponsors/ha
-00001fe0: 7973 7461 636b 2d66 6173 7461 7069 2e73  ystack-fastapi.s
-00001ff0: 7667 223e 3c2f 613e 0a3c 6120 6872 6566  vg"></a>.<a href
-00002000: 3d22 6874 7470 733a 2f2f 6361 7265 6572  ="https://career
-00002010: 732e 706f 7765 6e73 2e63 6f6d 2f22 2074  s.powens.com/" t
-00002020: 6172 6765 743d 225f 626c 616e 6b22 2074  arget="_blank" t
-00002030: 6974 6c65 3d22 506f 7765 6e73 2069 7320  itle="Powens is 
-00002040: 6869 7269 6e67 2122 3e3c 696d 6720 7372  hiring!"><img sr
-00002050: 633d 2268 7474 7073 3a2f 2f66 6173 7461  c="https://fasta
-00002060: 7069 2e74 6961 6e67 6f6c 6f2e 636f 6d2f  pi.tiangolo.com/
-00002070: 696d 672f 7370 6f6e 736f 7273 2f70 6f77  img/sponsors/pow
-00002080: 656e 732e 706e 6722 3e3c 2f61 3e0a 3c61  ens.png"></a>.<a
-00002090: 2068 7265 663d 2268 7474 7073 3a2f 2f77   href="https://w
-000020a0: 7777 2e73 7669 782e 636f 6d2f 2220 7461  ww.svix.com/" ta
-000020b0: 7267 6574 3d22 5f62 6c61 6e6b 2220 7469  rget="_blank" ti
-000020c0: 746c 653d 2253 7669 7820 2d20 5765 6268  tle="Svix - Webh
-000020d0: 6f6f 6b73 2061 7320 6120 7365 7276 6963  ooks as a servic
-000020e0: 6522 3e3c 696d 6720 7372 633d 2268 7474  e"><img src="htt
-000020f0: 7073 3a2f 2f66 6173 7461 7069 2e74 6961  ps://fastapi.tia
-00002100: 6e67 6f6c 6f2e 636f 6d2f 696d 672f 7370  ngolo.com/img/sp
-00002110: 6f6e 736f 7273 2f73 7669 782e 7376 6722  onsors/svix.svg"
-00002120: 3e3c 2f61 3e0a 3c61 2068 7265 663d 2268  ></a>.<a href="h
-00002130: 7474 7073 3a2f 2f64 6174 6162 656e 746f  ttps://databento
-00002140: 2e63 6f6d 2f22 2074 6172 6765 743d 225f  .com/" target="_
-00002150: 626c 616e 6b22 2074 6974 6c65 3d22 5061  blank" title="Pa
-00002160: 7920 6173 2079 6f75 2067 6f20 666f 7220  y as you go for 
-00002170: 6d61 726b 6574 2064 6174 6122 3e3c 696d  market data"><im
-00002180: 6720 7372 633d 2268 7474 7073 3a2f 2f66  g src="https://f
-00002190: 6173 7461 7069 2e74 6961 6e67 6f6c 6f2e  astapi.tiangolo.
-000021a0: 636f 6d2f 696d 672f 7370 6f6e 736f 7273  com/img/sponsors
-000021b0: 2f64 6174 6162 656e 746f 2e73 7667 223e  /databento.svg">
-000021c0: 3c2f 613e 0a0a 3c21 2d2d 202f 7370 6f6e  </a>..<!-- /spon
-000021d0: 736f 7273 202d 2d3e 0a0a 3c61 2068 7265  sors -->..<a hre
-000021e0: 663d 2268 7474 7073 3a2f 2f66 6173 7461  f="https://fasta
-000021f0: 7069 2e74 6961 6e67 6f6c 6f2e 636f 6d2f  pi.tiangolo.com/
-00002200: 6661 7374 6170 692d 7065 6f70 6c65 2f23  fastapi-people/#
-00002210: 7370 6f6e 736f 7273 2220 636c 6173 733d  sponsors" class=
-00002220: 2265 7874 6572 6e61 6c2d 6c69 6e6b 2220  "external-link" 
-00002230: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
-00002240: 4f74 6865 7220 7370 6f6e 736f 7273 3c2f  Other sponsors</
-00002250: 613e 0a0a 2323 204f 7069 6e69 6f6e 730a  a>..## Opinions.
-00002260: 0a22 5f5b 2e2e 2e5d 2049 276d 2075 7369  ."_[...] I'm usi
-00002270: 6e67 202a 2a46 6173 7441 5049 2a2a 2061  ng **FastAPI** a
-00002280: 2074 6f6e 2074 6865 7365 2064 6179 732e   ton these days.
-00002290: 205b 2e2e 2e5d 2049 276d 2061 6374 7561   [...] I'm actua
-000022a0: 6c6c 7920 706c 616e 6e69 6e67 2074 6f20  lly planning to 
-000022b0: 7573 6520 6974 2066 6f72 2061 6c6c 206f  use it for all o
-000022c0: 6620 6d79 2074 6561 6d27 7320 2a2a 4d4c  f my team's **ML
-000022d0: 2073 6572 7669 6365 7320 6174 204d 6963   services at Mic
-000022e0: 726f 736f 6674 2a2a 2e20 536f 6d65 206f  rosoft**. Some o
-000022f0: 6620 7468 656d 2061 7265 2067 6574 7469  f them are getti
-00002300: 6e67 2069 6e74 6567 7261 7465 6420 696e  ng integrated in
-00002310: 746f 2074 6865 2063 6f72 6520 2a2a 5769  to the core **Wi
-00002320: 6e64 6f77 732a 2a20 7072 6f64 7563 7420  ndows** product 
-00002330: 616e 6420 736f 6d65 202a 2a4f 6666 6963  and some **Offic
-00002340: 652a 2a20 7072 6f64 7563 7473 2e5f 220a  e** products._".
-00002350: 0a3c 6469 7620 7374 796c 653d 2274 6578  .<div style="tex
-00002360: 742d 616c 6967 6e3a 2072 6967 6874 3b20  t-align: right; 
-00002370: 6d61 7267 696e 2d72 6967 6874 3a20 3130  margin-right: 10
-00002380: 253b 223e 4b61 6269 7220 4b68 616e 202d  %;">Kabir Khan -
-00002390: 203c 7374 726f 6e67 3e4d 6963 726f 736f   <strong>Microso
-000023a0: 6674 3c2f 7374 726f 6e67 3e20 3c61 2068  ft</strong> <a h
-000023b0: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
-000023c0: 6875 622e 636f 6d2f 7469 616e 676f 6c6f  hub.com/tiangolo
-000023d0: 2f66 6173 7461 7069 2f70 756c 6c2f 3236  /fastapi/pull/26
-000023e0: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
-000023f0: 223e 3c73 6d61 6c6c 3e28 7265 6629 3c2f  "><small>(ref)</
-00002400: 736d 616c 6c3e 3c2f 613e 3c2f 6469 763e  small></a></div>
-00002410: 0a0a 2d2d 2d0a 0a22 5f57 6520 6164 6f70  ..---.."_We adop
-00002420: 7465 6420 7468 6520 2a2a 4661 7374 4150  ted the **FastAP
-00002430: 492a 2a20 6c69 6272 6172 7920 746f 2073  I** library to s
-00002440: 7061 776e 2061 202a 2a52 4553 542a 2a20  pawn a **REST** 
-00002450: 7365 7276 6572 2074 6861 7420 6361 6e20  server that can 
-00002460: 6265 2071 7565 7269 6564 2074 6f20 6f62  be queried to ob
-00002470: 7461 696e 202a 2a70 7265 6469 6374 696f  tain **predictio
-00002480: 6e73 2a2a 2e20 5b66 6f72 204c 7564 7769  ns**. [for Ludwi
-00002490: 675d 5f22 0a0a 3c64 6976 2073 7479 6c65  g]_"..<div style
-000024a0: 3d22 7465 7874 2d61 6c69 676e 3a20 7269  ="text-align: ri
-000024b0: 6768 743b 206d 6172 6769 6e2d 7269 6768  ght; margin-righ
-000024c0: 743a 2031 3025 3b22 3e50 6965 726f 204d  t: 10%;">Piero M
-000024d0: 6f6c 696e 6f2c 2059 6172 6f73 6c61 7620  olino, Yaroslav 
-000024e0: 4475 6469 6e2c 2061 6e64 2053 6169 2053  Dudin, and Sai S
-000024f0: 756d 616e 7468 204d 6972 7961 6c61 202d  umanth Miryala -
-00002500: 203c 7374 726f 6e67 3e55 6265 723c 2f73   <strong>Uber</s
-00002510: 7472 6f6e 673e 203c 6120 6872 6566 3d22  trong> <a href="
-00002520: 6874 7470 733a 2f2f 656e 672e 7562 6572  https://eng.uber
-00002530: 2e63 6f6d 2f6c 7564 7769 672d 7630 2d32  .com/ludwig-v0-2
-00002540: 2f22 2074 6172 6765 743d 225f 626c 616e  /" target="_blan
-00002550: 6b22 3e3c 736d 616c 6c3e 2872 6566 293c  k"><small>(ref)<
-00002560: 2f73 6d61 6c6c 3e3c 2f61 3e3c 2f64 6976  /small></a></div
-00002570: 3e0a 0a2d 2d2d 0a0a 225f 2a2a 4e65 7466  >..---.."_**Netf
-00002580: 6c69 782a 2a20 6973 2070 6c65 6173 6564  lix** is pleased
-00002590: 2074 6f20 616e 6e6f 756e 6365 2074 6865   to announce the
-000025a0: 206f 7065 6e2d 736f 7572 6365 2072 656c   open-source rel
-000025b0: 6561 7365 206f 6620 6f75 7220 2a2a 6372  ease of our **cr
-000025c0: 6973 6973 206d 616e 6167 656d 656e 742a  isis management*
-000025d0: 2a20 6f72 6368 6573 7472 6174 696f 6e20  * orchestration 
-000025e0: 6672 616d 6577 6f72 6b3a 202a 2a44 6973  framework: **Dis
-000025f0: 7061 7463 682a 2a21 205b 6275 696c 7420  patch**! [built 
-00002600: 7769 7468 202a 2a46 6173 7441 5049 2a2a  with **FastAPI**
-00002610: 5d5f 220a 0a3c 6469 7620 7374 796c 653d  ]_"..<div style=
-00002620: 2274 6578 742d 616c 6967 6e3a 2072 6967  "text-align: rig
-00002630: 6874 3b20 6d61 7267 696e 2d72 6967 6874  ht; margin-right
-00002640: 3a20 3130 253b 223e 4b65 7669 6e20 476c  : 10%;">Kevin Gl
-00002650: 6973 736f 6e2c 204d 6172 6320 5669 6c61  isson, Marc Vila
-00002660: 6e6f 7661 2c20 466f 7265 7374 204d 6f6e  nova, Forest Mon
-00002670: 7365 6e20 2d20 3c73 7472 6f6e 673e 4e65  sen - <strong>Ne
-00002680: 7466 6c69 783c 2f73 7472 6f6e 673e 203c  tflix</strong> <
-00002690: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-000026a0: 6e65 7466 6c69 7874 6563 6862 6c6f 672e  netflixtechblog.
-000026b0: 636f 6d2f 696e 7472 6f64 7563 696e 672d  com/introducing-
-000026c0: 6469 7370 6174 6368 2d64 6134 6238 6132  dispatch-da4b8a2
-000026d0: 6138 3037 3222 2074 6172 6765 743d 225f  a8072" target="_
-000026e0: 626c 616e 6b22 3e3c 736d 616c 6c3e 2872  blank"><small>(r
-000026f0: 6566 293c 2f73 6d61 6c6c 3e3c 2f61 3e3c  ef)</small></a><
-00002700: 2f64 6976 3e0a 0a2d 2d2d 0a0a 225f 49e2  /div>..---.."_I.
-00002710: 8099 6d20 6f76 6572 2074 6865 206d 6f6f  ..m over the moo
-00002720: 6e20 6578 6369 7465 6420 6162 6f75 7420  n excited about 
-00002730: 2a2a 4661 7374 4150 492a 2a2e 2049 74e2  **FastAPI**. It.
-00002740: 8099 7320 736f 2066 756e 215f 220a 0a3c  ..s so fun!_"..<
-00002750: 6469 7620 7374 796c 653d 2274 6578 742d  div style="text-
-00002760: 616c 6967 6e3a 2072 6967 6874 3b20 6d61  align: right; ma
-00002770: 7267 696e 2d72 6967 6874 3a20 3130 253b  rgin-right: 10%;
-00002780: 223e 4272 6961 6e20 4f6b 6b65 6e20 2d20  ">Brian Okken - 
-00002790: 3c73 7472 6f6e 673e 3c61 2068 7265 663d  <strong><a href=
-000027a0: 2268 7474 7073 3a2f 2f70 7974 686f 6e62  "https://pythonb
-000027b0: 7974 6573 2e66 6d2f 6570 6973 6f64 6573  ytes.fm/episodes
-000027c0: 2f73 686f 772f 3132 332f 7469 6d65 2d74  /show/123/time-t
-000027d0: 6f2d 7269 6768 742d 7468 652d 7079 2d77  o-right-the-py-w
-000027e0: 726f 6e67 733f 7469 6d65 5f69 6e5f 7365  rongs?time_in_se
-000027f0: 633d 3835 3522 2074 6172 6765 743d 225f  c=855" target="_
-00002800: 626c 616e 6b22 3e50 7974 686f 6e20 4279  blank">Python By
-00002810: 7465 733c 2f61 3e20 706f 6463 6173 7420  tes</a> podcast 
-00002820: 686f 7374 3c2f 7374 726f 6e67 3e20 3c61  host</strong> <a
-00002830: 2068 7265 663d 2268 7474 7073 3a2f 2f74   href="https://t
-00002840: 7769 7474 6572 2e63 6f6d 2f62 7269 616e  witter.com/brian
-00002850: 6f6b 6b65 6e2f 7374 6174 7573 2f31 3131  okken/status/111
-00002860: 3232 3230 3037 3939 3732 3732 3838 3332  2220079972728832
-00002870: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
-00002880: 223e 3c73 6d61 6c6c 3e28 7265 6629 3c2f  "><small>(ref)</
-00002890: 736d 616c 6c3e 3c2f 613e 3c2f 6469 763e  small></a></div>
-000028a0: 0a0a 2d2d 2d0a 0a22 5f48 6f6e 6573 746c  ..---.."_Honestl
-000028b0: 792c 2077 6861 7420 796f 7527 7665 2062  y, what you've b
-000028c0: 7569 6c74 206c 6f6f 6b73 2073 7570 6572  uilt looks super
-000028d0: 2073 6f6c 6964 2061 6e64 2070 6f6c 6973   solid and polis
-000028e0: 6865 642e 2049 6e20 6d61 6e79 2077 6179  hed. In many way
-000028f0: 732c 2069 7427 7320 7768 6174 2049 2077  s, it's what I w
-00002900: 616e 7465 6420 2a2a 4875 672a 2a20 746f  anted **Hug** to
-00002910: 2062 6520 2d20 6974 2773 2072 6561 6c6c   be - it's reall
-00002920: 7920 696e 7370 6972 696e 6720 746f 2073  y inspiring to s
-00002930: 6565 2073 6f6d 656f 6e65 2062 7569 6c64  ee someone build
-00002940: 2074 6861 742e 5f22 0a0a 3c64 6976 2073   that._"..<div s
-00002950: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
-00002960: 3a20 7269 6768 743b 206d 6172 6769 6e2d  : right; margin-
-00002970: 7269 6768 743a 2031 3025 3b22 3e54 696d  right: 10%;">Tim
-00002980: 6f74 6879 2043 726f 736c 6579 202d 203c  othy Crosley - <
-00002990: 7374 726f 6e67 3e3c 6120 6872 6566 3d22  strong><a href="
-000029a0: 6874 7470 733a 2f2f 7777 772e 6875 672e  https://www.hug.
-000029b0: 7265 7374 2f22 2074 6172 6765 743d 225f  rest/" target="_
-000029c0: 626c 616e 6b22 3e48 7567 3c2f 613e 2063  blank">Hug</a> c
-000029d0: 7265 6174 6f72 3c2f 7374 726f 6e67 3e20  reator</strong> 
-000029e0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-000029f0: 2f6e 6577 732e 7963 6f6d 6269 6e61 746f  /news.ycombinato
-00002a00: 722e 636f 6d2f 6974 656d 3f69 643d 3139  r.com/item?id=19
-00002a10: 3435 3534 3635 2220 7461 7267 6574 3d22  455465" target="
-00002a20: 5f62 6c61 6e6b 223e 3c73 6d61 6c6c 3e28  _blank"><small>(
-00002a30: 7265 6629 3c2f 736d 616c 6c3e 3c2f 613e  ref)</small></a>
-00002a40: 3c2f 6469 763e 0a0a 2d2d 2d0a 0a22 5f49  </div>..---.."_I
-00002a50: 6620 796f 7527 7265 206c 6f6f 6b69 6e67  f you're looking
-00002a60: 2074 6f20 6c65 6172 6e20 6f6e 6520 2a2a   to learn one **
-00002a70: 6d6f 6465 726e 2066 7261 6d65 776f 726b  modern framework
-00002a80: 2a2a 2066 6f72 2062 7569 6c64 696e 6720  ** for building 
-00002a90: 5245 5354 2041 5049 732c 2063 6865 636b  REST APIs, check
-00002aa0: 206f 7574 202a 2a46 6173 7441 5049 2a2a   out **FastAPI**
-00002ab0: 205b 2e2e 2e5d 2049 7427 7320 6661 7374   [...] It's fast
-00002ac0: 2c20 6561 7379 2074 6f20 7573 6520 616e  , easy to use an
-00002ad0: 6420 6561 7379 2074 6f20 6c65 6172 6e20  d easy to learn 
-00002ae0: 5b2e 2e2e 5d5f 220a 0a22 5f57 6527 7665  [...]_".."_We've
-00002af0: 2073 7769 7463 6865 6420 6f76 6572 2074   switched over t
-00002b00: 6f20 2a2a 4661 7374 4150 492a 2a20 666f  o **FastAPI** fo
-00002b10: 7220 6f75 7220 2a2a 4150 4973 2a2a 205b  r our **APIs** [
-00002b20: 2e2e 2e5d 2049 2074 6869 6e6b 2079 6f75  ...] I think you
-00002b30: 276c 6c20 6c69 6b65 2069 7420 5b2e 2e2e  'll like it [...
-00002b40: 5d5f 220a 0a3c 6469 7620 7374 796c 653d  ]_"..<div style=
-00002b50: 2274 6578 742d 616c 6967 6e3a 2072 6967  "text-align: rig
-00002b60: 6874 3b20 6d61 7267 696e 2d72 6967 6874  ht; margin-right
-00002b70: 3a20 3130 253b 223e 496e 6573 204d 6f6e  : 10%;">Ines Mon
-00002b80: 7461 6e69 202d 204d 6174 7468 6577 2048  tani - Matthew H
-00002b90: 6f6e 6e69 6261 6c20 2d20 3c73 7472 6f6e  onnibal - <stron
-00002ba0: 673e 3c61 2068 7265 663d 2268 7474 7073  g><a href="https
-00002bb0: 3a2f 2f65 7870 6c6f 7369 6f6e 2e61 6922  ://explosion.ai"
-00002bc0: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
-00002bd0: 3e45 7870 6c6f 7369 6f6e 2041 493c 2f61  >Explosion AI</a
-00002be0: 3e20 666f 756e 6465 7273 202d 203c 6120  > founders - <a 
-00002bf0: 6872 6566 3d22 6874 7470 733a 2f2f 7370  href="https://sp
-00002c00: 6163 792e 696f 2220 7461 7267 6574 3d22  acy.io" target="
-00002c10: 5f62 6c61 6e6b 223e 7370 6143 793c 2f61  _blank">spaCy</a
-00002c20: 3e20 6372 6561 746f 7273 3c2f 7374 726f  > creators</stro
-00002c30: 6e67 3e20 3c61 2068 7265 663d 2268 7474  ng> <a href="htt
-00002c40: 7073 3a2f 2f74 7769 7474 6572 2e63 6f6d  ps://twitter.com
-00002c50: 2f5f 696e 6573 6d6f 6e74 616e 692f 7374  /_inesmontani/st
-00002c60: 6174 7573 2f31 3134 3431 3733 3232 3533  atus/11441732253
-00002c70: 3232 3134 3337 3434 2220 7461 7267 6574  22143744" target
-00002c80: 3d22 5f62 6c61 6e6b 223e 3c73 6d61 6c6c  ="_blank"><small
-00002c90: 3e28 7265 6629 3c2f 736d 616c 6c3e 3c2f  >(ref)</small></
-00002ca0: 613e 202d 203c 6120 6872 6566 3d22 6874  a> - <a href="ht
-00002cb0: 7470 733a 2f2f 7477 6974 7465 722e 636f  tps://twitter.co
-00002cc0: 6d2f 686f 6e6e 6962 616c 2f73 7461 7475  m/honnibal/statu
-00002cd0: 732f 3131 3434 3033 3134 3231 3835 3936  s/11440314218596
-00002ce0: 3535 3638 3022 2074 6172 6765 743d 225f  55680" target="_
-00002cf0: 626c 616e 6b22 3e3c 736d 616c 6c3e 2872  blank"><small>(r
-00002d00: 6566 293c 2f73 6d61 6c6c 3e3c 2f61 3e3c  ef)</small></a><
-00002d10: 2f64 6976 3e0a 0a2d 2d2d 0a0a 225f 4966  /div>..---.."_If
-00002d20: 2061 6e79 6f6e 6520 6973 206c 6f6f 6b69   anyone is looki
-00002d30: 6e67 2074 6f20 6275 696c 6420 6120 7072  ng to build a pr
-00002d40: 6f64 7563 7469 6f6e 2050 7974 686f 6e20  oduction Python 
-00002d50: 4150 492c 2049 2077 6f75 6c64 2068 6967  API, I would hig
-00002d60: 686c 7920 7265 636f 6d6d 656e 6420 2a2a  hly recommend **
-00002d70: 4661 7374 4150 492a 2a2e 2049 7420 6973  FastAPI**. It is
-00002d80: 202a 2a62 6561 7574 6966 756c 6c79 2064   **beautifully d
-00002d90: 6573 6967 6e65 642a 2a2c 202a 2a73 696d  esigned**, **sim
-00002da0: 706c 6520 746f 2075 7365 2a2a 2061 6e64  ple to use** and
-00002db0: 202a 2a68 6967 686c 7920 7363 616c 6162   **highly scalab
-00002dc0: 6c65 2a2a 2c20 6974 2068 6173 2062 6563  le**, it has bec
-00002dd0: 6f6d 6520 6120 2a2a 6b65 7920 636f 6d70  ome a **key comp
-00002de0: 6f6e 656e 742a 2a20 696e 206f 7572 2041  onent** in our A
-00002df0: 5049 2066 6972 7374 2064 6576 656c 6f70  PI first develop
-00002e00: 6d65 6e74 2073 7472 6174 6567 7920 616e  ment strategy an
-00002e10: 6420 6973 2064 7269 7669 6e67 206d 616e  d is driving man
-00002e20: 7920 6175 746f 6d61 7469 6f6e 7320 616e  y automations an
-00002e30: 6420 7365 7276 6963 6573 2073 7563 6820  d services such 
-00002e40: 6173 206f 7572 2056 6972 7475 616c 2054  as our Virtual T
-00002e50: 4143 2045 6e67 696e 6565 722e 5f22 0a0a  AC Engineer._"..
-00002e60: 3c64 6976 2073 7479 6c65 3d22 7465 7874  <div style="text
-00002e70: 2d61 6c69 676e 3a20 7269 6768 743b 206d  -align: right; m
-00002e80: 6172 6769 6e2d 7269 6768 743a 2031 3025  argin-right: 10%
-00002e90: 3b22 3e44 656f 6e20 5069 6c6c 7362 7572  ;">Deon Pillsbur
-00002ea0: 7920 2d20 3c73 7472 6f6e 673e 4369 7363  y - <strong>Cisc
-00002eb0: 6f3c 2f73 7472 6f6e 673e 203c 6120 6872  o</strong> <a hr
-00002ec0: 6566 3d22 6874 7470 733a 2f2f 7777 772e  ef="https://www.
-00002ed0: 6c69 6e6b 6564 696e 2e63 6f6d 2f70 6f73  linkedin.com/pos
-00002ee0: 7473 2f64 656f 6e70 696c 6c73 6275 7279  ts/deonpillsbury
-00002ef0: 5f63 6973 636f 2d63 782d 7079 7468 6f6e  _cisco-cx-python
-00002f00: 2d61 6374 6976 6974 792d 3639 3633 3234  -activity-696324
-00002f10: 3236 3238 3533 3634 3837 3933 362d 7472  2628536487936-tr
-00002f20: 4170 2f22 2074 6172 6765 743d 225f 626c  Ap/" target="_bl
-00002f30: 616e 6b22 3e3c 736d 616c 6c3e 2872 6566  ank"><small>(ref
-00002f40: 293c 2f73 6d61 6c6c 3e3c 2f61 3e3c 2f64  )</small></a></d
-00002f50: 6976 3e0a 0a2d 2d2d 0a0a 2323 202a 2a54  iv>..---..## **T
-00002f60: 7970 6572 2a2a 2c20 7468 6520 4661 7374  yper**, the Fast
-00002f70: 4150 4920 6f66 2043 4c49 730a 0a3c 6120  API of CLIs..<a 
-00002f80: 6872 6566 3d22 6874 7470 733a 2f2f 7479  href="https://ty
-00002f90: 7065 722e 7469 616e 676f 6c6f 2e63 6f6d  per.tiangolo.com
-00002fa0: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
-00002fb0: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
-00002fc0: 733a 2f2f 7479 7065 722e 7469 616e 676f  s://typer.tiango
-00002fd0: 6c6f 2e63 6f6d 2f69 6d67 2f6c 6f67 6f2d  lo.com/img/logo-
-00002fe0: 6d61 7267 696e 2f6c 6f67 6f2d 6d61 7267  margin/logo-marg
-00002ff0: 696e 2d76 6563 746f 722e 7376 6722 2073  in-vector.svg" s
-00003000: 7479 6c65 3d22 7769 6474 683a 2032 3025  tyle="width: 20%
-00003010: 3b22 3e3c 2f61 3e0a 0a49 6620 796f 7520  ;"></a>..If you 
-00003020: 6172 6520 6275 696c 6469 6e67 2061 203c  are building a <
-00003030: 6162 6272 2074 6974 6c65 3d22 436f 6d6d  abbr title="Comm
-00003040: 616e 6420 4c69 6e65 2049 6e74 6572 6661  and Line Interfa
-00003050: 6365 223e 434c 493c 2f61 6262 723e 2061  ce">CLI</abbr> a
-00003060: 7070 2074 6f20 6265 2075 7365 6420 696e  pp to be used in
-00003070: 2074 6865 2074 6572 6d69 6e61 6c20 696e   the terminal in
-00003080: 7374 6561 6420 6f66 2061 2077 6562 2041  stead of a web A
-00003090: 5049 2c20 6368 6563 6b20 6f75 7420 3c61  PI, check out <a
-000030a0: 2068 7265 663d 2268 7474 7073 3a2f 2f74   href="https://t
-000030b0: 7970 6572 2e74 6961 6e67 6f6c 6f2e 636f  yper.tiangolo.co
-000030c0: 6d2f 2220 636c 6173 733d 2265 7874 6572  m/" class="exter
-000030d0: 6e61 6c2d 6c69 6e6b 2220 7461 7267 6574  nal-link" target
-000030e0: 3d22 5f62 6c61 6e6b 223e 2a2a 5479 7065  ="_blank">**Type
-000030f0: 722a 2a3c 2f61 3e2e 0a0a 2a2a 5479 7065  r**</a>...**Type
-00003100: 722a 2a20 6973 2046 6173 7441 5049 2773  r** is FastAPI's
-00003110: 206c 6974 746c 6520 7369 626c 696e 672e   little sibling.
-00003120: 2041 6e64 2069 7427 7320 696e 7465 6e64   And it's intend
-00003130: 6564 2074 6f20 6265 2074 6865 202a 2a46  ed to be the **F
-00003140: 6173 7441 5049 206f 6620 434c 4973 2a2a  astAPI of CLIs**
-00003150: 2e20 e28c a8ef b88f 20f0 9f9a 800a 0a23  . ...... ......#
-00003160: 2320 5265 7175 6972 656d 656e 7473 0a0a  # Requirements..
-00003170: 5079 7468 6f6e 2033 2e37 2b0a 0a46 6173  Python 3.7+..Fas
-00003180: 7441 5049 2073 7461 6e64 7320 6f6e 2074  tAPI stands on t
-00003190: 6865 2073 686f 756c 6465 7273 206f 6620  he shoulders of 
-000031a0: 6769 616e 7473 3a0a 0a2a 203c 6120 6872  giants:..* <a hr
-000031b0: 6566 3d22 6874 7470 733a 2f2f 7777 772e  ef="https://www.
-000031c0: 7374 6172 6c65 7474 652e 696f 2f22 2063  starlette.io/" c
-000031d0: 6c61 7373 3d22 6578 7465 726e 616c 2d6c  lass="external-l
-000031e0: 696e 6b22 2074 6172 6765 743d 225f 626c  ink" target="_bl
-000031f0: 616e 6b22 3e53 7461 726c 6574 7465 3c2f  ank">Starlette</
-00003200: 613e 2066 6f72 2074 6865 2077 6562 2070  a> for the web p
-00003210: 6172 7473 2e0a 2a20 3c61 2068 7265 663d  arts..* <a href=
-00003220: 2268 7474 7073 3a2f 2f70 7964 616e 7469  "https://pydanti
-00003230: 632d 646f 6373 2e68 656c 706d 616e 7561  c-docs.helpmanua
-00003240: 6c2e 696f 2f22 2063 6c61 7373 3d22 6578  l.io/" class="ex
-00003250: 7465 726e 616c 2d6c 696e 6b22 2074 6172  ternal-link" tar
-00003260: 6765 743d 225f 626c 616e 6b22 3e50 7964  get="_blank">Pyd
-00003270: 616e 7469 633c 2f61 3e20 666f 7220 7468  antic</a> for th
-00003280: 6520 6461 7461 2070 6172 7473 2e0a 0a23  e data parts...#
-00003290: 2320 496e 7374 616c 6c61 7469 6f6e 0a0a  # Installation..
-000032a0: 3c64 6976 2063 6c61 7373 3d22 7465 726d  <div class="term
-000032b0: 7922 3e0a 0a60 6060 636f 6e73 6f6c 650a  y">..```console.
-000032c0: 2420 7069 7020 696e 7374 616c 6c20 6661  $ pip install fa
-000032d0: 7374 6170 690a 0a2d 2d2d 3e20 3130 3025  stapi..---> 100%
-000032e0: 0a60 6060 0a0a 3c2f 6469 763e 0a0a 596f  .```..</div>..Yo
-000032f0: 7520 7769 6c6c 2061 6c73 6f20 6e65 6564  u will also need
-00003300: 2061 6e20 4153 4749 2073 6572 7665 722c   an ASGI server,
-00003310: 2066 6f72 2070 726f 6475 6374 696f 6e20   for production 
-00003320: 7375 6368 2061 7320 3c61 2068 7265 663d  such as <a href=
-00003330: 2268 7474 7073 3a2f 2f77 7777 2e75 7669  "https://www.uvi
-00003340: 636f 726e 2e6f 7267 2220 636c 6173 733d  corn.org" class=
-00003350: 2265 7874 6572 6e61 6c2d 6c69 6e6b 2220  "external-link" 
-00003360: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
-00003370: 5576 6963 6f72 6e3c 2f61 3e20 6f72 203c  Uvicorn</a> or <
-00003380: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00003390: 6769 7468 7562 2e63 6f6d 2f70 676a 6f6e  github.com/pgjon
-000033a0: 6573 2f68 7970 6572 636f 726e 2220 636c  es/hypercorn" cl
-000033b0: 6173 733d 2265 7874 6572 6e61 6c2d 6c69  ass="external-li
-000033c0: 6e6b 2220 7461 7267 6574 3d22 5f62 6c61  nk" target="_bla
-000033d0: 6e6b 223e 4879 7065 7263 6f72 6e3c 2f61  nk">Hypercorn</a
-000033e0: 3e2e 0a0a 3c64 6976 2063 6c61 7373 3d22  >...<div class="
-000033f0: 7465 726d 7922 3e0a 0a60 6060 636f 6e73  termy">..```cons
-00003400: 6f6c 650a 2420 7069 7020 696e 7374 616c  ole.$ pip instal
-00003410: 6c20 2275 7669 636f 726e 5b73 7461 6e64  l "uvicorn[stand
-00003420: 6172 645d 220a 0a2d 2d2d 3e20 3130 3025  ard]"..---> 100%
-00003430: 0a60 6060 0a0a 3c2f 6469 763e 0a0a 2323  .```..</div>..##
-00003440: 2045 7861 6d70 6c65 0a0a 2323 2320 4372   Example..### Cr
-00003450: 6561 7465 2069 740a 0a2a 2043 7265 6174  eate it..* Creat
-00003460: 6520 6120 6669 6c65 2060 6d61 696e 2e70  e a file `main.p
-00003470: 7960 2077 6974 683a 0a0a 6060 6050 7974  y` with:..```Pyt
-00003480: 686f 6e0a 6672 6f6d 2074 7970 696e 6720  hon.from typing 
-00003490: 696d 706f 7274 2055 6e69 6f6e 0a0a 6672  import Union..fr
-000034a0: 6f6d 2066 6173 7461 7069 2069 6d70 6f72  om fastapi impor
-000034b0: 7420 4661 7374 4150 490a 0a61 7070 203d  t FastAPI..app =
-000034c0: 2046 6173 7441 5049 2829 0a0a 0a40 6170   FastAPI()...@ap
-000034d0: 702e 6765 7428 222f 2229 0a64 6566 2072  p.get("/").def r
-000034e0: 6561 645f 726f 6f74 2829 3a0a 2020 2020  ead_root():.    
-000034f0: 7265 7475 726e 207b 2248 656c 6c6f 223a  return {"Hello":
-00003500: 2022 576f 726c 6422 7d0a 0a0a 4061 7070   "World"}...@app
-00003510: 2e67 6574 2822 2f69 7465 6d73 2f7b 6974  .get("/items/{it
-00003520: 656d 5f69 647d 2229 0a64 6566 2072 6561  em_id}").def rea
-00003530: 645f 6974 656d 2869 7465 6d5f 6964 3a20  d_item(item_id: 
-00003540: 696e 742c 2071 3a20 556e 696f 6e5b 7374  int, q: Union[st
-00003550: 722c 204e 6f6e 655d 203d 204e 6f6e 6529  r, None] = None)
-00003560: 3a0a 2020 2020 7265 7475 726e 207b 2269  :.    return {"i
-00003570: 7465 6d5f 6964 223a 2069 7465 6d5f 6964  tem_id": item_id
-00003580: 2c20 2271 223a 2071 7d0a 6060 600a 0a3c  , "q": q}.```..<
-00003590: 6465 7461 696c 7320 6d61 726b 646f 776e  details markdown
-000035a0: 3d22 3122 3e0a 3c73 756d 6d61 7279 3e4f  ="1">.<summary>O
-000035b0: 7220 7573 6520 3c63 6f64 653e 6173 796e  r use <code>asyn
-000035c0: 6320 6465 663c 2f63 6f64 653e 2e2e 2e3c  c def</code>...<
-000035d0: 2f73 756d 6d61 7279 3e0a 0a49 6620 796f  /summary>..If yo
-000035e0: 7572 2063 6f64 6520 7573 6573 2060 6173  ur code uses `as
-000035f0: 796e 6360 202f 2060 6177 6169 7460 2c20  ync` / `await`, 
-00003600: 7573 6520 6061 7379 6e63 2064 6566 603a  use `async def`:
-00003610: 0a0a 6060 6050 7974 686f 6e20 686c 5f6c  ..```Python hl_l
-00003620: 696e 6573 3d22 3920 2031 3422 0a66 726f  ines="9  14".fro
-00003630: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
-00003640: 556e 696f 6e0a 0a66 726f 6d20 6661 7374  Union..from fast
-00003650: 6170 6920 696d 706f 7274 2046 6173 7441  api import FastA
-00003660: 5049 0a0a 6170 7020 3d20 4661 7374 4150  PI..app = FastAP
-00003670: 4928 290a 0a0a 4061 7070 2e67 6574 2822  I()...@app.get("
-00003680: 2f22 290a 6173 796e 6320 6465 6620 7265  /").async def re
-00003690: 6164 5f72 6f6f 7428 293a 0a20 2020 2072  ad_root():.    r
-000036a0: 6574 7572 6e20 7b22 4865 6c6c 6f22 3a20  eturn {"Hello": 
-000036b0: 2257 6f72 6c64 227d 0a0a 0a40 6170 702e  "World"}...@app.
-000036c0: 6765 7428 222f 6974 656d 732f 7b69 7465  get("/items/{ite
-000036d0: 6d5f 6964 7d22 290a 6173 796e 6320 6465  m_id}").async de
-000036e0: 6620 7265 6164 5f69 7465 6d28 6974 656d  f read_item(item
-000036f0: 5f69 643a 2069 6e74 2c20 713a 2055 6e69  _id: int, q: Uni
-00003700: 6f6e 5b73 7472 2c20 4e6f 6e65 5d20 3d20  on[str, None] = 
-00003710: 4e6f 6e65 293a 0a20 2020 2072 6574 7572  None):.    retur
-00003720: 6e20 7b22 6974 656d 5f69 6422 3a20 6974  n {"item_id": it
-00003730: 656d 5f69 642c 2022 7122 3a20 717d 0a60  em_id, "q": q}.`
-00003740: 6060 0a0a 2a2a 4e6f 7465 2a2a 3a0a 0a49  ``..**Note**:..I
-00003750: 6620 796f 7520 646f 6e27 7420 6b6e 6f77  f you don't know
-00003760: 2c20 6368 6563 6b20 7468 6520 5f22 496e  , check the _"In
-00003770: 2061 2068 7572 7279 3f22 5f20 7365 6374   a hurry?"_ sect
-00003780: 696f 6e20 6162 6f75 7420 3c61 2068 7265  ion about <a hre
-00003790: 663d 2268 7474 7073 3a2f 2f66 6173 7461  f="https://fasta
-000037a0: 7069 2e74 6961 6e67 6f6c 6f2e 636f 6d2f  pi.tiangolo.com/
-000037b0: 6173 796e 632f 2369 6e2d 612d 6875 7272  async/#in-a-hurr
-000037c0: 7922 2074 6172 6765 743d 225f 626c 616e  y" target="_blan
-000037d0: 6b22 3e60 6173 796e 6360 2061 6e64 2060  k">`async` and `
-000037e0: 6177 6169 7460 2069 6e20 7468 6520 646f  await` in the do
-000037f0: 6373 3c2f 613e 2e0a 0a3c 2f64 6574 6169  cs</a>...</detai
-00003800: 6c73 3e0a 0a23 2323 2052 756e 2069 740a  ls>..### Run it.
-00003810: 0a52 756e 2074 6865 2073 6572 7665 7220  .Run the server 
-00003820: 7769 7468 3a0a 0a3c 6469 7620 636c 6173  with:..<div clas
-00003830: 733d 2274 6572 6d79 223e 0a0a 6060 6063  s="termy">..```c
-00003840: 6f6e 736f 6c65 0a24 2075 7669 636f 726e  onsole.$ uvicorn
-00003850: 206d 6169 6e3a 6170 7020 2d2d 7265 6c6f   main:app --relo
-00003860: 6164 0a0a 494e 464f 3a20 2020 2020 5576  ad..INFO:     Uv
-00003870: 6963 6f72 6e20 7275 6e6e 696e 6720 6f6e  icorn running on
-00003880: 2068 7474 703a 2f2f 3132 372e 302e 302e   http://127.0.0.
-00003890: 313a 3830 3030 2028 5072 6573 7320 4354  1:8000 (Press CT
-000038a0: 524c 2b43 2074 6f20 7175 6974 290a 494e  RL+C to quit).IN
-000038b0: 464f 3a20 2020 2020 5374 6172 7465 6420  FO:     Started 
-000038c0: 7265 6c6f 6164 6572 2070 726f 6365 7373  reloader process
-000038d0: 205b 3238 3732 305d 0a49 4e46 4f3a 2020   [28720].INFO:  
-000038e0: 2020 2053 7461 7274 6564 2073 6572 7665     Started serve
-000038f0: 7220 7072 6f63 6573 7320 5b32 3837 3232  r process [28722
-00003900: 5d0a 494e 464f 3a20 2020 2020 5761 6974  ].INFO:     Wait
-00003910: 696e 6720 666f 7220 6170 706c 6963 6174  ing for applicat
-00003920: 696f 6e20 7374 6172 7475 702e 0a49 4e46  ion startup..INF
-00003930: 4f3a 2020 2020 2041 7070 6c69 6361 7469  O:     Applicati
-00003940: 6f6e 2073 7461 7274 7570 2063 6f6d 706c  on startup compl
-00003950: 6574 652e 0a60 6060 0a0a 3c2f 6469 763e  ete..```..</div>
-00003960: 0a0a 3c64 6574 6169 6c73 206d 6172 6b64  ..<details markd
-00003970: 6f77 6e3d 2231 223e 0a3c 7375 6d6d 6172  own="1">.<summar
-00003980: 793e 4162 6f75 7420 7468 6520 636f 6d6d  y>About the comm
-00003990: 616e 6420 3c63 6f64 653e 7576 6963 6f72  and <code>uvicor
-000039a0: 6e20 6d61 696e 3a61 7070 202d 2d72 656c  n main:app --rel
-000039b0: 6f61 643c 2f63 6f64 653e 2e2e 2e3c 2f73  oad</code>...</s
-000039c0: 756d 6d61 7279 3e0a 0a54 6865 2063 6f6d  ummary>..The com
-000039d0: 6d61 6e64 2060 7576 6963 6f72 6e20 6d61  mand `uvicorn ma
-000039e0: 696e 3a61 7070 6020 7265 6665 7273 2074  in:app` refers t
-000039f0: 6f3a 0a0a 2a20 606d 6169 6e60 3a20 7468  o:..* `main`: th
-00003a00: 6520 6669 6c65 2060 6d61 696e 2e70 7960  e file `main.py`
-00003a10: 2028 7468 6520 5079 7468 6f6e 2022 6d6f   (the Python "mo
-00003a20: 6475 6c65 2229 2e0a 2a20 6061 7070 603a  dule")..* `app`:
-00003a30: 2074 6865 206f 626a 6563 7420 6372 6561   the object crea
-00003a40: 7465 6420 696e 7369 6465 206f 6620 606d  ted inside of `m
-00003a50: 6169 6e2e 7079 6020 7769 7468 2074 6865  ain.py` with the
-00003a60: 206c 696e 6520 6061 7070 203d 2046 6173   line `app = Fas
-00003a70: 7441 5049 2829 602e 0a2a 2060 2d2d 7265  tAPI()`..* `--re
-00003a80: 6c6f 6164 603a 206d 616b 6520 7468 6520  load`: make the 
-00003a90: 7365 7276 6572 2072 6573 7461 7274 2061  server restart a
-00003aa0: 6674 6572 2063 6f64 6520 6368 616e 6765  fter code change
-00003ab0: 732e 204f 6e6c 7920 646f 2074 6869 7320  s. Only do this 
-00003ac0: 666f 7220 6465 7665 6c6f 706d 656e 742e  for development.
-00003ad0: 0a0a 3c2f 6465 7461 696c 733e 0a0a 2323  ..</details>..##
-00003ae0: 2320 4368 6563 6b20 6974 0a0a 4f70 656e  # Check it..Open
-00003af0: 2079 6f75 7220 6272 6f77 7365 7220 6174   your browser at
-00003b00: 203c 6120 6872 6566 3d22 6874 7470 3a2f   <a href="http:/
-00003b10: 2f31 3237 2e30 2e30 2e31 3a38 3030 302f  /127.0.0.1:8000/
-00003b20: 6974 656d 732f 353f 713d 736f 6d65 7175  items/5?q=somequ
-00003b30: 6572 7922 2063 6c61 7373 3d22 6578 7465  ery" class="exte
-00003b40: 726e 616c 2d6c 696e 6b22 2074 6172 6765  rnal-link" targe
-00003b50: 743d 225f 626c 616e 6b22 3e68 7474 703a  t="_blank">http:
-00003b60: 2f2f 3132 372e 302e 302e 313a 3830 3030  //127.0.0.1:8000
-00003b70: 2f69 7465 6d73 2f35 3f71 3d73 6f6d 6571  /items/5?q=someq
-00003b80: 7565 7279 3c2f 613e 2e0a 0a59 6f75 2077  uery</a>...You w
-00003b90: 696c 6c20 7365 6520 7468 6520 4a53 4f4e  ill see the JSON
-00003ba0: 2072 6573 706f 6e73 6520 6173 3a0a 0a60   response as:..`
-00003bb0: 6060 4a53 4f4e 0a7b 2269 7465 6d5f 6964  ``JSON.{"item_id
-00003bc0: 223a 2035 2c20 2271 223a 2022 736f 6d65  ": 5, "q": "some
-00003bd0: 7175 6572 7922 7d0a 6060 600a 0a59 6f75  query"}.```..You
-00003be0: 2061 6c72 6561 6479 2063 7265 6174 6564   already created
-00003bf0: 2061 6e20 4150 4920 7468 6174 3a0a 0a2a   an API that:..*
-00003c00: 2052 6563 6569 7665 7320 4854 5450 2072   Receives HTTP r
-00003c10: 6571 7565 7374 7320 696e 2074 6865 205f  equests in the _
-00003c20: 7061 7468 735f 2060 2f60 2061 6e64 2060  paths_ `/` and `
-00003c30: 2f69 7465 6d73 2f7b 6974 656d 5f69 647d  /items/{item_id}
-00003c40: 602e 0a2a 2042 6f74 6820 5f70 6174 6873  `..* Both _paths
-00003c50: 5f20 7461 6b65 2060 4745 5460 203c 656d  _ take `GET` <em
-00003c60: 3e6f 7065 7261 7469 6f6e 733c 2f65 6d3e  >operations</em>
-00003c70: 2028 616c 736f 206b 6e6f 776e 2061 7320   (also known as 
-00003c80: 4854 5450 205f 6d65 7468 6f64 735f 292e  HTTP _methods_).
-00003c90: 0a2a 2054 6865 205f 7061 7468 5f20 602f  .* The _path_ `/
-00003ca0: 6974 656d 732f 7b69 7465 6d5f 6964 7d60  items/{item_id}`
-00003cb0: 2068 6173 2061 205f 7061 7468 2070 6172   has a _path par
-00003cc0: 616d 6574 6572 5f20 6069 7465 6d5f 6964  ameter_ `item_id
-00003cd0: 6020 7468 6174 2073 686f 756c 6420 6265  ` that should be
-00003ce0: 2061 6e20 6069 6e74 602e 0a2a 2054 6865   an `int`..* The
-00003cf0: 205f 7061 7468 5f20 602f 6974 656d 732f   _path_ `/items/
-00003d00: 7b69 7465 6d5f 6964 7d60 2068 6173 2061  {item_id}` has a
-00003d10: 6e20 6f70 7469 6f6e 616c 2060 7374 7260  n optional `str`
-00003d20: 205f 7175 6572 7920 7061 7261 6d65 7465   _query paramete
-00003d30: 725f 2060 7160 2e0a 0a23 2323 2049 6e74  r_ `q`...### Int
-00003d40: 6572 6163 7469 7665 2041 5049 2064 6f63  eractive API doc
-00003d50: 730a 0a4e 6f77 2067 6f20 746f 203c 6120  s..Now go to <a 
-00003d60: 6872 6566 3d22 6874 7470 3a2f 2f31 3237  href="http://127
-00003d70: 2e30 2e30 2e31 3a38 3030 302f 646f 6373  .0.0.1:8000/docs
-00003d80: 2220 636c 6173 733d 2265 7874 6572 6e61  " class="externa
-00003d90: 6c2d 6c69 6e6b 2220 7461 7267 6574 3d22  l-link" target="
-00003da0: 5f62 6c61 6e6b 223e 6874 7470 3a2f 2f31  _blank">http://1
-00003db0: 3237 2e30 2e30 2e31 3a38 3030 302f 646f  27.0.0.1:8000/do
-00003dc0: 6373 3c2f 613e 2e0a 0a59 6f75 2077 696c  cs</a>...You wil
-00003dd0: 6c20 7365 6520 7468 6520 6175 746f 6d61  l see the automa
-00003de0: 7469 6320 696e 7465 7261 6374 6976 6520  tic interactive 
-00003df0: 4150 4920 646f 6375 6d65 6e74 6174 696f  API documentatio
-00003e00: 6e20 2870 726f 7669 6465 6420 6279 203c  n (provided by <
-00003e10: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00003e20: 6769 7468 7562 2e63 6f6d 2f73 7761 6767  github.com/swagg
-00003e30: 6572 2d61 7069 2f73 7761 6767 6572 2d75  er-api/swagger-u
-00003e40: 6922 2063 6c61 7373 3d22 6578 7465 726e  i" class="extern
-00003e50: 616c 2d6c 696e 6b22 2074 6172 6765 743d  al-link" target=
-00003e60: 225f 626c 616e 6b22 3e53 7761 6767 6572  "_blank">Swagger
-00003e70: 2055 493c 2f61 3e29 3a0a 0a21 5b53 7761   UI</a>):..![Swa
-00003e80: 6767 6572 2055 495d 2868 7474 7073 3a2f  gger UI](https:/
-00003e90: 2f66 6173 7461 7069 2e74 6961 6e67 6f6c  /fastapi.tiangol
-00003ea0: 6f2e 636f 6d2f 696d 672f 696e 6465 782f  o.com/img/index/
-00003eb0: 696e 6465 782d 3031 2d73 7761 6767 6572  index-01-swagger
-00003ec0: 2d75 692d 7369 6d70 6c65 2e70 6e67 290a  -ui-simple.png).
-00003ed0: 0a23 2323 2041 6c74 6572 6e61 7469 7665  .### Alternative
-00003ee0: 2041 5049 2064 6f63 730a 0a41 6e64 206e   API docs..And n
-00003ef0: 6f77 2c20 676f 2074 6f20 3c61 2068 7265  ow, go to <a hre
-00003f00: 663d 2268 7474 703a 2f2f 3132 372e 302e  f="http://127.0.
-00003f10: 302e 313a 3830 3030 2f72 6564 6f63 2220  0.1:8000/redoc" 
-00003f20: 636c 6173 733d 2265 7874 6572 6e61 6c2d  class="external-
-00003f30: 6c69 6e6b 2220 7461 7267 6574 3d22 5f62  link" target="_b
-00003f40: 6c61 6e6b 223e 6874 7470 3a2f 2f31 3237  lank">http://127
-00003f50: 2e30 2e30 2e31 3a38 3030 302f 7265 646f  .0.0.1:8000/redo
-00003f60: 633c 2f61 3e2e 0a0a 596f 7520 7769 6c6c  c</a>...You will
-00003f70: 2073 6565 2074 6865 2061 6c74 6572 6e61   see the alterna
-00003f80: 7469 7665 2061 7574 6f6d 6174 6963 2064  tive automatic d
-00003f90: 6f63 756d 656e 7461 7469 6f6e 2028 7072  ocumentation (pr
-00003fa0: 6f76 6964 6564 2062 7920 3c61 2068 7265  ovided by <a hre
-00003fb0: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
-00003fc0: 622e 636f 6d2f 5265 6269 6c6c 792f 5265  b.com/Rebilly/Re
-00003fd0: 446f 6322 2063 6c61 7373 3d22 6578 7465  Doc" class="exte
-00003fe0: 726e 616c 2d6c 696e 6b22 2074 6172 6765  rnal-link" targe
-00003ff0: 743d 225f 626c 616e 6b22 3e52 6544 6f63  t="_blank">ReDoc
-00004000: 3c2f 613e 293a 0a0a 215b 5265 446f 635d  </a>):..![ReDoc]
-00004010: 2868 7474 7073 3a2f 2f66 6173 7461 7069  (https://fastapi
-00004020: 2e74 6961 6e67 6f6c 6f2e 636f 6d2f 696d  .tiangolo.com/im
-00004030: 672f 696e 6465 782f 696e 6465 782d 3032  g/index/index-02
-00004040: 2d72 6564 6f63 2d73 696d 706c 652e 706e  -redoc-simple.pn
-00004050: 6729 0a0a 2323 2045 7861 6d70 6c65 2075  g)..## Example u
-00004060: 7067 7261 6465 0a0a 4e6f 7720 6d6f 6469  pgrade..Now modi
-00004070: 6679 2074 6865 2066 696c 6520 606d 6169  fy the file `mai
-00004080: 6e2e 7079 6020 746f 2072 6563 6569 7665  n.py` to receive
-00004090: 2061 2062 6f64 7920 6672 6f6d 2061 2060   a body from a `
-000040a0: 5055 5460 2072 6571 7565 7374 2e0a 0a44  PUT` request...D
-000040b0: 6563 6c61 7265 2074 6865 2062 6f64 7920  eclare the body 
-000040c0: 7573 696e 6720 7374 616e 6461 7264 2050  using standard P
-000040d0: 7974 686f 6e20 7479 7065 732c 2074 6861  ython types, tha
-000040e0: 6e6b 7320 746f 2050 7964 616e 7469 632e  nks to Pydantic.
-000040f0: 0a0a 6060 6050 7974 686f 6e20 686c 5f6c  ..```Python hl_l
-00004100: 696e 6573 3d22 3420 2039 2d31 3220 2032  ines="4  9-12  2
-00004110: 352d 3237 220a 6672 6f6d 2074 7970 696e  5-27".from typin
-00004120: 6720 696d 706f 7274 2055 6e69 6f6e 0a0a  g import Union..
-00004130: 6672 6f6d 2066 6173 7461 7069 2069 6d70  from fastapi imp
-00004140: 6f72 7420 4661 7374 4150 490a 6672 6f6d  ort FastAPI.from
-00004150: 2070 7964 616e 7469 6320 696d 706f 7274   pydantic import
-00004160: 2042 6173 654d 6f64 656c 0a0a 6170 7020   BaseModel..app 
-00004170: 3d20 4661 7374 4150 4928 290a 0a0a 636c  = FastAPI()...cl
-00004180: 6173 7320 4974 656d 2842 6173 654d 6f64  ass Item(BaseMod
-00004190: 656c 293a 0a20 2020 206e 616d 653a 2073  el):.    name: s
-000041a0: 7472 0a20 2020 2070 7269 6365 3a20 666c  tr.    price: fl
-000041b0: 6f61 740a 2020 2020 6973 5f6f 6666 6572  oat.    is_offer
-000041c0: 3a20 556e 696f 6e5b 626f 6f6c 2c20 4e6f  : Union[bool, No
-000041d0: 6e65 5d20 3d20 4e6f 6e65 0a0a 0a40 6170  ne] = None...@ap
-000041e0: 702e 6765 7428 222f 2229 0a64 6566 2072  p.get("/").def r
-000041f0: 6561 645f 726f 6f74 2829 3a0a 2020 2020  ead_root():.    
-00004200: 7265 7475 726e 207b 2248 656c 6c6f 223a  return {"Hello":
-00004210: 2022 576f 726c 6422 7d0a 0a0a 4061 7070   "World"}...@app
-00004220: 2e67 6574 2822 2f69 7465 6d73 2f7b 6974  .get("/items/{it
-00004230: 656d 5f69 647d 2229 0a64 6566 2072 6561  em_id}").def rea
-00004240: 645f 6974 656d 2869 7465 6d5f 6964 3a20  d_item(item_id: 
-00004250: 696e 742c 2071 3a20 556e 696f 6e5b 7374  int, q: Union[st
-00004260: 722c 204e 6f6e 655d 203d 204e 6f6e 6529  r, None] = None)
-00004270: 3a0a 2020 2020 7265 7475 726e 207b 2269  :.    return {"i
-00004280: 7465 6d5f 6964 223a 2069 7465 6d5f 6964  tem_id": item_id
-00004290: 2c20 2271 223a 2071 7d0a 0a0a 4061 7070  , "q": q}...@app
-000042a0: 2e70 7574 2822 2f69 7465 6d73 2f7b 6974  .put("/items/{it
-000042b0: 656d 5f69 647d 2229 0a64 6566 2075 7064  em_id}").def upd
-000042c0: 6174 655f 6974 656d 2869 7465 6d5f 6964  ate_item(item_id
-000042d0: 3a20 696e 742c 2069 7465 6d3a 2049 7465  : int, item: Ite
-000042e0: 6d29 3a0a 2020 2020 7265 7475 726e 207b  m):.    return {
-000042f0: 2269 7465 6d5f 6e61 6d65 223a 2069 7465  "item_name": ite
-00004300: 6d2e 6e61 6d65 2c20 2269 7465 6d5f 6964  m.name, "item_id
-00004310: 223a 2069 7465 6d5f 6964 7d0a 6060 600a  ": item_id}.```.
-00004320: 0a54 6865 2073 6572 7665 7220 7368 6f75  .The server shou
-00004330: 6c64 2072 656c 6f61 6420 6175 746f 6d61  ld reload automa
-00004340: 7469 6361 6c6c 7920 2862 6563 6175 7365  tically (because
-00004350: 2079 6f75 2061 6464 6564 2060 2d2d 7265   you added `--re
-00004360: 6c6f 6164 6020 746f 2074 6865 2060 7576  load` to the `uv
-00004370: 6963 6f72 6e60 2063 6f6d 6d61 6e64 2061  icorn` command a
-00004380: 626f 7665 292e 0a0a 2323 2320 496e 7465  bove)...### Inte
-00004390: 7261 6374 6976 6520 4150 4920 646f 6373  ractive API docs
-000043a0: 2075 7067 7261 6465 0a0a 4e6f 7720 676f   upgrade..Now go
-000043b0: 2074 6f20 3c61 2068 7265 663d 2268 7474   to <a href="htt
-000043c0: 703a 2f2f 3132 372e 302e 302e 313a 3830  p://127.0.0.1:80
-000043d0: 3030 2f64 6f63 7322 2063 6c61 7373 3d22  00/docs" class="
-000043e0: 6578 7465 726e 616c 2d6c 696e 6b22 2074  external-link" t
-000043f0: 6172 6765 743d 225f 626c 616e 6b22 3e68  arget="_blank">h
-00004400: 7474 703a 2f2f 3132 372e 302e 302e 313a  ttp://127.0.0.1:
-00004410: 3830 3030 2f64 6f63 733c 2f61 3e2e 0a0a  8000/docs</a>...
-00004420: 2a20 5468 6520 696e 7465 7261 6374 6976  * The interactiv
-00004430: 6520 4150 4920 646f 6375 6d65 6e74 6174  e API documentat
-00004440: 696f 6e20 7769 6c6c 2062 6520 6175 746f  ion will be auto
-00004450: 6d61 7469 6361 6c6c 7920 7570 6461 7465  matically update
-00004460: 642c 2069 6e63 6c75 6469 6e67 2074 6865  d, including the
-00004470: 206e 6577 2062 6f64 793a 0a0a 215b 5377   new body:..![Sw
-00004480: 6167 6765 7220 5549 5d28 6874 7470 733a  agger UI](https:
-00004490: 2f2f 6661 7374 6170 692e 7469 616e 676f  //fastapi.tiango
-000044a0: 6c6f 2e63 6f6d 2f69 6d67 2f69 6e64 6578  lo.com/img/index
-000044b0: 2f69 6e64 6578 2d30 332d 7377 6167 6765  /index-03-swagge
-000044c0: 722d 3032 2e70 6e67 290a 0a2a 2043 6c69  r-02.png)..* Cli
-000044d0: 636b 206f 6e20 7468 6520 6275 7474 6f6e  ck on the button
-000044e0: 2022 5472 7920 6974 206f 7574 222c 2069   "Try it out", i
-000044f0: 7420 616c 6c6f 7773 2079 6f75 2074 6f20  t allows you to 
-00004500: 6669 6c6c 2074 6865 2070 6172 616d 6574  fill the paramet
-00004510: 6572 7320 616e 6420 6469 7265 6374 6c79  ers and directly
-00004520: 2069 6e74 6572 6163 7420 7769 7468 2074   interact with t
-00004530: 6865 2041 5049 3a0a 0a21 5b53 7761 6767  he API:..![Swagg
-00004540: 6572 2055 4920 696e 7465 7261 6374 696f  er UI interactio
-00004550: 6e5d 2868 7474 7073 3a2f 2f66 6173 7461  n](https://fasta
-00004560: 7069 2e74 6961 6e67 6f6c 6f2e 636f 6d2f  pi.tiangolo.com/
-00004570: 696d 672f 696e 6465 782f 696e 6465 782d  img/index/index-
-00004580: 3034 2d73 7761 6767 6572 2d30 332e 706e  04-swagger-03.pn
-00004590: 6729 0a0a 2a20 5468 656e 2063 6c69 636b  g)..* Then click
-000045a0: 206f 6e20 7468 6520 2245 7865 6375 7465   on the "Execute
-000045b0: 2220 6275 7474 6f6e 2c20 7468 6520 7573  " button, the us
-000045c0: 6572 2069 6e74 6572 6661 6365 2077 696c  er interface wil
-000045d0: 6c20 636f 6d6d 756e 6963 6174 6520 7769  l communicate wi
-000045e0: 7468 2079 6f75 7220 4150 492c 2073 656e  th your API, sen
-000045f0: 6420 7468 6520 7061 7261 6d65 7465 7273  d the parameters
-00004600: 2c20 6765 7420 7468 6520 7265 7375 6c74  , get the result
-00004610: 7320 616e 6420 7368 6f77 2074 6865 6d20  s and show them 
-00004620: 6f6e 2074 6865 2073 6372 6565 6e3a 0a0a  on the screen:..
-00004630: 215b 5377 6167 6765 7220 5549 2069 6e74  ![Swagger UI int
-00004640: 6572 6163 7469 6f6e 5d28 6874 7470 733a  eraction](https:
-00004650: 2f2f 6661 7374 6170 692e 7469 616e 676f  //fastapi.tiango
-00004660: 6c6f 2e63 6f6d 2f69 6d67 2f69 6e64 6578  lo.com/img/index
-00004670: 2f69 6e64 6578 2d30 352d 7377 6167 6765  /index-05-swagge
-00004680: 722d 3034 2e70 6e67 290a 0a23 2323 2041  r-04.png)..### A
-00004690: 6c74 6572 6e61 7469 7665 2041 5049 2064  lternative API d
-000046a0: 6f63 7320 7570 6772 6164 650a 0a41 6e64  ocs upgrade..And
-000046b0: 206e 6f77 2c20 676f 2074 6f20 3c61 2068   now, go to <a h
-000046c0: 7265 663d 2268 7474 703a 2f2f 3132 372e  ref="http://127.
-000046d0: 302e 302e 313a 3830 3030 2f72 6564 6f63  0.0.1:8000/redoc
-000046e0: 2220 636c 6173 733d 2265 7874 6572 6e61  " class="externa
-000046f0: 6c2d 6c69 6e6b 2220 7461 7267 6574 3d22  l-link" target="
-00004700: 5f62 6c61 6e6b 223e 6874 7470 3a2f 2f31  _blank">http://1
-00004710: 3237 2e30 2e30 2e31 3a38 3030 302f 7265  27.0.0.1:8000/re
-00004720: 646f 633c 2f61 3e2e 0a0a 2a20 5468 6520  doc</a>...* The 
-00004730: 616c 7465 726e 6174 6976 6520 646f 6375  alternative docu
-00004740: 6d65 6e74 6174 696f 6e20 7769 6c6c 2061  mentation will a
-00004750: 6c73 6f20 7265 666c 6563 7420 7468 6520  lso reflect the 
-00004760: 6e65 7720 7175 6572 7920 7061 7261 6d65  new query parame
-00004770: 7465 7220 616e 6420 626f 6479 3a0a 0a21  ter and body:..!
-00004780: 5b52 6544 6f63 5d28 6874 7470 733a 2f2f  [ReDoc](https://
-00004790: 6661 7374 6170 692e 7469 616e 676f 6c6f  fastapi.tiangolo
-000047a0: 2e63 6f6d 2f69 6d67 2f69 6e64 6578 2f69  .com/img/index/i
-000047b0: 6e64 6578 2d30 362d 7265 646f 632d 3032  ndex-06-redoc-02
-000047c0: 2e70 6e67 290a 0a23 2323 2052 6563 6170  .png)..### Recap
-000047d0: 0a0a 496e 2073 756d 6d61 7279 2c20 796f  ..In summary, yo
-000047e0: 7520 6465 636c 6172 6520 2a2a 6f6e 6365  u declare **once
-000047f0: 2a2a 2074 6865 2074 7970 6573 206f 6620  ** the types of 
-00004800: 7061 7261 6d65 7465 7273 2c20 626f 6479  parameters, body
-00004810: 2c20 6574 632e 2061 7320 6675 6e63 7469  , etc. as functi
-00004820: 6f6e 2070 6172 616d 6574 6572 732e 0a0a  on parameters...
-00004830: 596f 7520 646f 2074 6861 7420 7769 7468  You do that with
-00004840: 2073 7461 6e64 6172 6420 6d6f 6465 726e   standard modern
-00004850: 2050 7974 686f 6e20 7479 7065 732e 0a0a   Python types...
-00004860: 596f 7520 646f 6e27 7420 6861 7665 2074  You don't have t
-00004870: 6f20 6c65 6172 6e20 6120 6e65 7720 7379  o learn a new sy
-00004880: 6e74 6178 2c20 7468 6520 6d65 7468 6f64  ntax, the method
-00004890: 7320 6f72 2063 6c61 7373 6573 206f 6620  s or classes of 
-000048a0: 6120 7370 6563 6966 6963 206c 6962 7261  a specific libra
-000048b0: 7279 2c20 6574 632e 0a0a 4a75 7374 2073  ry, etc...Just s
-000048c0: 7461 6e64 6172 6420 2a2a 5079 7468 6f6e  tandard **Python
-000048d0: 2033 2e37 2b2a 2a2e 0a0a 466f 7220 6578   3.7+**...For ex
-000048e0: 616d 706c 652c 2066 6f72 2061 6e20 6069  ample, for an `i
-000048f0: 6e74 603a 0a0a 6060 6050 7974 686f 6e0a  nt`:..```Python.
-00004900: 6974 656d 5f69 643a 2069 6e74 0a60 6060  item_id: int.```
-00004910: 0a0a 6f72 2066 6f72 2061 206d 6f72 6520  ..or for a more 
-00004920: 636f 6d70 6c65 7820 6049 7465 6d60 206d  complex `Item` m
-00004930: 6f64 656c 3a0a 0a60 6060 5079 7468 6f6e  odel:..```Python
-00004940: 0a69 7465 6d3a 2049 7465 6d0a 6060 600a  .item: Item.```.
-00004950: 0a2e 2e2e 616e 6420 7769 7468 2074 6861  ....and with tha
-00004960: 7420 7369 6e67 6c65 2064 6563 6c61 7261  t single declara
-00004970: 7469 6f6e 2079 6f75 2067 6574 3a0a 0a2a  tion you get:..*
-00004980: 2045 6469 746f 7220 7375 7070 6f72 742c   Editor support,
-00004990: 2069 6e63 6c75 6469 6e67 3a0a 2020 2020   including:.    
-000049a0: 2a20 436f 6d70 6c65 7469 6f6e 2e0a 2020  * Completion..  
-000049b0: 2020 2a20 5479 7065 2063 6865 636b 732e    * Type checks.
-000049c0: 0a2a 2056 616c 6964 6174 696f 6e20 6f66  .* Validation of
-000049d0: 2064 6174 613a 0a20 2020 202a 2041 7574   data:.    * Aut
-000049e0: 6f6d 6174 6963 2061 6e64 2063 6c65 6172  omatic and clear
-000049f0: 2065 7272 6f72 7320 7768 656e 2074 6865   errors when the
-00004a00: 2064 6174 6120 6973 2069 6e76 616c 6964   data is invalid
-00004a10: 2e0a 2020 2020 2a20 5661 6c69 6461 7469  ..    * Validati
-00004a20: 6f6e 2065 7665 6e20 666f 7220 6465 6570  on even for deep
-00004a30: 6c79 206e 6573 7465 6420 4a53 4f4e 206f  ly nested JSON o
-00004a40: 626a 6563 7473 2e0a 2a20 3c61 6262 7220  bjects..* <abbr 
-00004a50: 7469 746c 653d 2261 6c73 6f20 6b6e 6f77  title="also know
-00004a60: 6e20 6173 3a20 7365 7269 616c 697a 6174  n as: serializat
-00004a70: 696f 6e2c 2070 6172 7369 6e67 2c20 6d61  ion, parsing, ma
-00004a80: 7273 6861 6c6c 696e 6722 3e43 6f6e 7665  rshalling">Conve
-00004a90: 7273 696f 6e3c 2f61 6262 723e 206f 6620  rsion</abbr> of 
-00004aa0: 696e 7075 7420 6461 7461 3a20 636f 6d69  input data: comi
-00004ab0: 6e67 2066 726f 6d20 7468 6520 6e65 7477  ng from the netw
-00004ac0: 6f72 6b20 746f 2050 7974 686f 6e20 6461  ork to Python da
-00004ad0: 7461 2061 6e64 2074 7970 6573 2e20 5265  ta and types. Re
-00004ae0: 6164 696e 6720 6672 6f6d 3a0a 2020 2020  ading from:.    
-00004af0: 2a20 4a53 4f4e 2e0a 2020 2020 2a20 5061  * JSON..    * Pa
-00004b00: 7468 2070 6172 616d 6574 6572 732e 0a20  th parameters.. 
-00004b10: 2020 202a 2051 7565 7279 2070 6172 616d     * Query param
-00004b20: 6574 6572 732e 0a20 2020 202a 2043 6f6f  eters..    * Coo
-00004b30: 6b69 6573 2e0a 2020 2020 2a20 4865 6164  kies..    * Head
-00004b40: 6572 732e 0a20 2020 202a 2046 6f72 6d73  ers..    * Forms
-00004b50: 2e0a 2020 2020 2a20 4669 6c65 732e 0a2a  ..    * Files..*
-00004b60: 203c 6162 6272 2074 6974 6c65 3d22 616c   <abbr title="al
-00004b70: 736f 206b 6e6f 776e 2061 733a 2073 6572  so known as: ser
-00004b80: 6961 6c69 7a61 7469 6f6e 2c20 7061 7273  ialization, pars
-00004b90: 696e 672c 206d 6172 7368 616c 6c69 6e67  ing, marshalling
-00004ba0: 223e 436f 6e76 6572 7369 6f6e 3c2f 6162  ">Conversion</ab
-00004bb0: 6272 3e20 6f66 206f 7574 7075 7420 6461  br> of output da
-00004bc0: 7461 3a20 636f 6e76 6572 7469 6e67 2066  ta: converting f
-00004bd0: 726f 6d20 5079 7468 6f6e 2064 6174 6120  rom Python data 
-00004be0: 616e 6420 7479 7065 7320 746f 206e 6574  and types to net
-00004bf0: 776f 726b 2064 6174 6120 2861 7320 4a53  work data (as JS
-00004c00: 4f4e 293a 0a20 2020 202a 2043 6f6e 7665  ON):.    * Conve
-00004c10: 7274 2050 7974 686f 6e20 7479 7065 7320  rt Python types 
-00004c20: 2860 7374 7260 2c20 6069 6e74 602c 2060  (`str`, `int`, `
-00004c30: 666c 6f61 7460 2c20 6062 6f6f 6c60 2c20  float`, `bool`, 
-00004c40: 606c 6973 7460 2c20 6574 6329 2e0a 2020  `list`, etc)..  
-00004c50: 2020 2a20 6064 6174 6574 696d 6560 206f    * `datetime` o
-00004c60: 626a 6563 7473 2e0a 2020 2020 2a20 6055  bjects..    * `U
-00004c70: 5549 4460 206f 626a 6563 7473 2e0a 2020  UID` objects..  
-00004c80: 2020 2a20 4461 7461 6261 7365 206d 6f64    * Database mod
-00004c90: 656c 732e 0a20 2020 202a 202e 2e2e 616e  els..    * ...an
-00004ca0: 6420 6d61 6e79 206d 6f72 652e 0a2a 2041  d many more..* A
-00004cb0: 7574 6f6d 6174 6963 2069 6e74 6572 6163  utomatic interac
-00004cc0: 7469 7665 2041 5049 2064 6f63 756d 656e  tive API documen
-00004cd0: 7461 7469 6f6e 2c20 696e 636c 7564 696e  tation, includin
-00004ce0: 6720 3220 616c 7465 726e 6174 6976 6520  g 2 alternative 
-00004cf0: 7573 6572 2069 6e74 6572 6661 6365 733a  user interfaces:
-00004d00: 0a20 2020 202a 2053 7761 6767 6572 2055  .    * Swagger U
-00004d10: 492e 0a20 2020 202a 2052 6544 6f63 2e0a  I..    * ReDoc..
-00004d20: 0a2d 2d2d 0a0a 436f 6d69 6e67 2062 6163  .---..Coming bac
-00004d30: 6b20 746f 2074 6865 2070 7265 7669 6f75  k to the previou
-00004d40: 7320 636f 6465 2065 7861 6d70 6c65 2c20  s code example, 
-00004d50: 2a2a 4661 7374 4150 492a 2a20 7769 6c6c  **FastAPI** will
-00004d60: 3a0a 0a2a 2056 616c 6964 6174 6520 7468  :..* Validate th
-00004d70: 6174 2074 6865 7265 2069 7320 616e 2060  at there is an `
-00004d80: 6974 656d 5f69 6460 2069 6e20 7468 6520  item_id` in the 
-00004d90: 7061 7468 2066 6f72 2060 4745 5460 2061  path for `GET` a
-00004da0: 6e64 2060 5055 5460 2072 6571 7565 7374  nd `PUT` request
-00004db0: 732e 0a2a 2056 616c 6964 6174 6520 7468  s..* Validate th
-00004dc0: 6174 2074 6865 2060 6974 656d 5f69 6460  at the `item_id`
-00004dd0: 2069 7320 6f66 2074 7970 6520 6069 6e74   is of type `int
-00004de0: 6020 666f 7220 6047 4554 6020 616e 6420  ` for `GET` and 
-00004df0: 6050 5554 6020 7265 7175 6573 7473 2e0a  `PUT` requests..
-00004e00: 2020 2020 2a20 4966 2069 7420 6973 206e      * If it is n
-00004e10: 6f74 2c20 7468 6520 636c 6965 6e74 2077  ot, the client w
-00004e20: 696c 6c20 7365 6520 6120 7573 6566 756c  ill see a useful
-00004e30: 2c20 636c 6561 7220 6572 726f 722e 0a2a  , clear error..*
-00004e40: 2043 6865 636b 2069 6620 7468 6572 6520   Check if there 
-00004e50: 6973 2061 6e20 6f70 7469 6f6e 616c 2071  is an optional q
-00004e60: 7565 7279 2070 6172 616d 6574 6572 206e  uery parameter n
-00004e70: 616d 6564 2060 7160 2028 6173 2069 6e20  amed `q` (as in 
-00004e80: 6068 7474 703a 2f2f 3132 372e 302e 302e  `http://127.0.0.
-00004e90: 313a 3830 3030 2f69 7465 6d73 2f66 6f6f  1:8000/items/foo
-00004ea0: 3f71 3d73 6f6d 6571 7565 7279 6029 2066  ?q=somequery`) f
-00004eb0: 6f72 2060 4745 5460 2072 6571 7565 7374  or `GET` request
-00004ec0: 732e 0a20 2020 202a 2041 7320 7468 6520  s..    * As the 
-00004ed0: 6071 6020 7061 7261 6d65 7465 7220 6973  `q` parameter is
-00004ee0: 2064 6563 6c61 7265 6420 7769 7468 2060   declared with `
-00004ef0: 3d20 4e6f 6e65 602c 2069 7420 6973 206f  = None`, it is o
-00004f00: 7074 696f 6e61 6c2e 0a20 2020 202a 2057  ptional..    * W
-00004f10: 6974 686f 7574 2074 6865 2060 4e6f 6e65  ithout the `None
-00004f20: 6020 6974 2077 6f75 6c64 2062 6520 7265  ` it would be re
-00004f30: 7175 6972 6564 2028 6173 2069 7320 7468  quired (as is th
-00004f40: 6520 626f 6479 2069 6e20 7468 6520 6361  e body in the ca
-00004f50: 7365 2077 6974 6820 6050 5554 6029 2e0a  se with `PUT`)..
-00004f60: 2a20 466f 7220 6050 5554 6020 7265 7175  * For `PUT` requ
-00004f70: 6573 7473 2074 6f20 602f 6974 656d 732f  ests to `/items/
-00004f80: 7b69 7465 6d5f 6964 7d60 2c20 5265 6164  {item_id}`, Read
-00004f90: 2074 6865 2062 6f64 7920 6173 204a 534f   the body as JSO
-00004fa0: 4e3a 0a20 2020 202a 2043 6865 636b 2074  N:.    * Check t
-00004fb0: 6861 7420 6974 2068 6173 2061 2072 6571  hat it has a req
-00004fc0: 7569 7265 6420 6174 7472 6962 7574 6520  uired attribute 
-00004fd0: 606e 616d 6560 2074 6861 7420 7368 6f75  `name` that shou
-00004fe0: 6c64 2062 6520 6120 6073 7472 602e 0a20  ld be a `str`.. 
-00004ff0: 2020 202a 2043 6865 636b 2074 6861 7420     * Check that 
-00005000: 6974 2068 6173 2061 2072 6571 7569 7265  it has a require
-00005010: 6420 6174 7472 6962 7574 6520 6070 7269  d attribute `pri
-00005020: 6365 6020 7468 6174 2068 6173 2074 6f20  ce` that has to 
-00005030: 6265 2061 2060 666c 6f61 7460 2e0a 2020  be a `float`..  
-00005040: 2020 2a20 4368 6563 6b20 7468 6174 2069    * Check that i
-00005050: 7420 6861 7320 616e 206f 7074 696f 6e61  t has an optiona
-00005060: 6c20 6174 7472 6962 7574 6520 6069 735f  l attribute `is_
-00005070: 6f66 6665 7260 2c20 7468 6174 2073 686f  offer`, that sho
-00005080: 756c 6420 6265 2061 2060 626f 6f6c 602c  uld be a `bool`,
-00005090: 2069 6620 7072 6573 656e 742e 0a20 2020   if present..   
-000050a0: 202a 2041 6c6c 2074 6869 7320 776f 756c   * All this woul
-000050b0: 6420 616c 736f 2077 6f72 6b20 666f 7220  d also work for 
-000050c0: 6465 6570 6c79 206e 6573 7465 6420 4a53  deeply nested JS
-000050d0: 4f4e 206f 626a 6563 7473 2e0a 2a20 436f  ON objects..* Co
-000050e0: 6e76 6572 7420 6672 6f6d 2061 6e64 2074  nvert from and t
-000050f0: 6f20 4a53 4f4e 2061 7574 6f6d 6174 6963  o JSON automatic
-00005100: 616c 6c79 2e0a 2a20 446f 6375 6d65 6e74  ally..* Document
-00005110: 2065 7665 7279 7468 696e 6720 7769 7468   everything with
-00005120: 204f 7065 6e41 5049 2c20 7468 6174 2063   OpenAPI, that c
-00005130: 616e 2062 6520 7573 6564 2062 793a 0a20  an be used by:. 
-00005140: 2020 202a 2049 6e74 6572 6163 7469 7665     * Interactive
-00005150: 2064 6f63 756d 656e 7461 7469 6f6e 2073   documentation s
-00005160: 7973 7465 6d73 2e0a 2020 2020 2a20 4175  ystems..    * Au
-00005170: 746f 6d61 7469 6320 636c 6965 6e74 2063  tomatic client c
-00005180: 6f64 6520 6765 6e65 7261 7469 6f6e 2073  ode generation s
-00005190: 7973 7465 6d73 2c20 666f 7220 6d61 6e79  ystems, for many
-000051a0: 206c 616e 6775 6167 6573 2e0a 2a20 5072   languages..* Pr
-000051b0: 6f76 6964 6520 3220 696e 7465 7261 6374  ovide 2 interact
-000051c0: 6976 6520 646f 6375 6d65 6e74 6174 696f  ive documentatio
-000051d0: 6e20 7765 6220 696e 7465 7266 6163 6573  n web interfaces
-000051e0: 2064 6972 6563 746c 792e 0a0a 2d2d 2d0a   directly...---.
-000051f0: 0a57 6520 6a75 7374 2073 6372 6174 6368  .We just scratch
-00005200: 6564 2074 6865 2073 7572 6661 6365 2c20  ed the surface, 
-00005210: 6275 7420 796f 7520 616c 7265 6164 7920  but you already 
-00005220: 6765 7420 7468 6520 6964 6561 206f 6620  get the idea of 
-00005230: 686f 7720 6974 2061 6c6c 2077 6f72 6b73  how it all works
-00005240: 2e0a 0a54 7279 2063 6861 6e67 696e 6720  ...Try changing 
-00005250: 7468 6520 6c69 6e65 2077 6974 683a 0a0a  the line with:..
-00005260: 6060 6050 7974 686f 6e0a 2020 2020 7265  ```Python.    re
-00005270: 7475 726e 207b 2269 7465 6d5f 6e61 6d65  turn {"item_name
-00005280: 223a 2069 7465 6d2e 6e61 6d65 2c20 2269  ": item.name, "i
-00005290: 7465 6d5f 6964 223a 2069 7465 6d5f 6964  tem_id": item_id
-000052a0: 7d0a 6060 600a 0a2e 2e2e 6672 6f6d 3a0a  }.```.....from:.
-000052b0: 0a60 6060 5079 7468 6f6e 0a20 2020 2020  .```Python.     
-000052c0: 2020 202e 2e2e 2022 6974 656d 5f6e 616d     ... "item_nam
-000052d0: 6522 3a20 6974 656d 2e6e 616d 6520 2e2e  e": item.name ..
-000052e0: 2e0a 6060 600a 0a2e 2e2e 746f 3a0a 0a60  ..```.....to:..`
-000052f0: 6060 5079 7468 6f6e 0a20 2020 2020 2020  ``Python.       
-00005300: 202e 2e2e 2022 6974 656d 5f70 7269 6365   ... "item_price
-00005310: 223a 2069 7465 6d2e 7072 6963 6520 2e2e  ": item.price ..
-00005320: 2e0a 6060 600a 0a2e 2e2e 616e 6420 7365  ..```.....and se
-00005330: 6520 686f 7720 796f 7572 2065 6469 746f  e how your edito
-00005340: 7220 7769 6c6c 2061 7574 6f2d 636f 6d70  r will auto-comp
-00005350: 6c65 7465 2074 6865 2061 7474 7269 6275  lete the attribu
-00005360: 7465 7320 616e 6420 6b6e 6f77 2074 6865  tes and know the
-00005370: 6972 2074 7970 6573 3a0a 0a21 5b65 6469  ir types:..![edi
-00005380: 746f 7220 7375 7070 6f72 745d 2868 7474  tor support](htt
-00005390: 7073 3a2f 2f66 6173 7461 7069 2e74 6961  ps://fastapi.tia
-000053a0: 6e67 6f6c 6f2e 636f 6d2f 696d 672f 7673  ngolo.com/img/vs
-000053b0: 636f 6465 2d63 6f6d 706c 6574 696f 6e2e  code-completion.
-000053c0: 706e 6729 0a0a 466f 7220 6120 6d6f 7265  png)..For a more
-000053d0: 2063 6f6d 706c 6574 6520 6578 616d 706c   complete exampl
-000053e0: 6520 696e 636c 7564 696e 6720 6d6f 7265  e including more
-000053f0: 2066 6561 7475 7265 732c 2073 6565 2074   features, see t
-00005400: 6865 203c 6120 6872 6566 3d22 6874 7470  he <a href="http
-00005410: 733a 2f2f 6661 7374 6170 692e 7469 616e  s://fastapi.tian
-00005420: 676f 6c6f 2e63 6f6d 2f74 7574 6f72 6961  golo.com/tutoria
-00005430: 6c2f 223e 5475 746f 7269 616c 202d 2055  l/">Tutorial - U
-00005440: 7365 7220 4775 6964 653c 2f61 3e2e 0a0a  ser Guide</a>...
-00005450: 2a2a 5370 6f69 6c65 7220 616c 6572 742a  **Spoiler alert*
-00005460: 2a3a 2074 6865 2074 7574 6f72 6961 6c20  *: the tutorial 
-00005470: 2d20 7573 6572 2067 7569 6465 2069 6e63  - user guide inc
-00005480: 6c75 6465 733a 0a0a 2a20 4465 636c 6172  ludes:..* Declar
-00005490: 6174 696f 6e20 6f66 202a 2a70 6172 616d  ation of **param
-000054a0: 6574 6572 732a 2a20 6672 6f6d 206f 7468  eters** from oth
-000054b0: 6572 2064 6966 6665 7265 6e74 2070 6c61  er different pla
-000054c0: 6365 7320 6173 3a20 2a2a 6865 6164 6572  ces as: **header
-000054d0: 732a 2a2c 202a 2a63 6f6f 6b69 6573 2a2a  s**, **cookies**
-000054e0: 2c20 2a2a 666f 726d 2066 6965 6c64 732a  , **form fields*
-000054f0: 2a20 616e 6420 2a2a 6669 6c65 732a 2a2e  * and **files**.
-00005500: 0a2a 2048 6f77 2074 6f20 7365 7420 2a2a  .* How to set **
-00005510: 7661 6c69 6461 7469 6f6e 2063 6f6e 7374  validation const
-00005520: 7261 696e 7473 2a2a 2061 7320 606d 6178  raints** as `max
-00005530: 696d 756d 5f6c 656e 6774 6860 206f 7220  imum_length` or 
-00005540: 6072 6567 6578 602e 0a2a 2041 2076 6572  `regex`..* A ver
-00005550: 7920 706f 7765 7266 756c 2061 6e64 2065  y powerful and e
-00005560: 6173 7920 746f 2075 7365 202a 2a3c 6162  asy to use **<ab
-00005570: 6272 2074 6974 6c65 3d22 616c 736f 206b  br title="also k
-00005580: 6e6f 776e 2061 7320 636f 6d70 6f6e 656e  nown as componen
-00005590: 7473 2c20 7265 736f 7572 6365 732c 2070  ts, resources, p
-000055a0: 726f 7669 6465 7273 2c20 7365 7276 6963  roviders, servic
-000055b0: 6573 2c20 696e 6a65 6374 6162 6c65 7322  es, injectables"
-000055c0: 3e44 6570 656e 6465 6e63 7920 496e 6a65  >Dependency Inje
-000055d0: 6374 696f 6e3c 2f61 6262 723e 2a2a 2073  ction</abbr>** s
-000055e0: 7973 7465 6d2e 0a2a 2053 6563 7572 6974  ystem..* Securit
-000055f0: 7920 616e 6420 6175 7468 656e 7469 6361  y and authentica
-00005600: 7469 6f6e 2c20 696e 636c 7564 696e 6720  tion, including 
-00005610: 7375 7070 6f72 7420 666f 7220 2a2a 4f41  support for **OA
-00005620: 7574 6832 2a2a 2077 6974 6820 2a2a 4a57  uth2** with **JW
-00005630: 5420 746f 6b65 6e73 2a2a 2061 6e64 202a  T tokens** and *
-00005640: 2a48 5454 5020 4261 7369 632a 2a20 6175  *HTTP Basic** au
-00005650: 7468 2e0a 2a20 4d6f 7265 2061 6476 616e  th..* More advan
-00005660: 6365 6420 2862 7574 2065 7175 616c 6c79  ced (but equally
-00005670: 2065 6173 7929 2074 6563 686e 6971 7565   easy) technique
-00005680: 7320 666f 7220 6465 636c 6172 696e 6720  s for declaring 
-00005690: 2a2a 6465 6570 6c79 206e 6573 7465 6420  **deeply nested 
-000056a0: 4a53 4f4e 206d 6f64 656c 732a 2a20 2874  JSON models** (t
-000056b0: 6861 6e6b 7320 746f 2050 7964 616e 7469  hanks to Pydanti
-000056c0: 6329 2e0a 2a20 2a2a 4772 6170 6851 4c2a  c)..* **GraphQL*
-000056d0: 2a20 696e 7465 6772 6174 696f 6e20 7769  * integration wi
-000056e0: 7468 203c 6120 6872 6566 3d22 6874 7470  th <a href="http
-000056f0: 733a 2f2f 7374 7261 7762 6572 7279 2e72  s://strawberry.r
-00005700: 6f63 6b73 2220 636c 6173 733d 2265 7874  ocks" class="ext
-00005710: 6572 6e61 6c2d 6c69 6e6b 2220 7461 7267  ernal-link" targ
-00005720: 6574 3d22 5f62 6c61 6e6b 223e 5374 7261  et="_blank">Stra
-00005730: 7762 6572 7279 3c2f 613e 2061 6e64 206f  wberry</a> and o
-00005740: 7468 6572 206c 6962 7261 7269 6573 2e0a  ther libraries..
-00005750: 2a20 4d61 6e79 2065 7874 7261 2066 6561  * Many extra fea
-00005760: 7475 7265 7320 2874 6861 6e6b 7320 746f  tures (thanks to
-00005770: 2053 7461 726c 6574 7465 2920 6173 3a0a   Starlette) as:.
-00005780: 2020 2020 2a20 2a2a 5765 6253 6f63 6b65      * **WebSocke
-00005790: 7473 2a2a 0a20 2020 202a 2065 7874 7265  ts**.    * extre
-000057a0: 6d65 6c79 2065 6173 7920 7465 7374 7320  mely easy tests 
-000057b0: 6261 7365 6420 6f6e 2048 5454 5058 2061  based on HTTPX a
-000057c0: 6e64 2060 7079 7465 7374 600a 2020 2020  nd `pytest`.    
-000057d0: 2a20 2a2a 434f 5253 2a2a 0a20 2020 202a  * **CORS**.    *
-000057e0: 202a 2a43 6f6f 6b69 6520 5365 7373 696f   **Cookie Sessio
-000057f0: 6e73 2a2a 0a20 2020 202a 202e 2e2e 616e  ns**.    * ...an
-00005800: 6420 6d6f 7265 2e0a 0a23 2320 5065 7266  d more...## Perf
-00005810: 6f72 6d61 6e63 650a 0a49 6e64 6570 656e  ormance..Indepen
-00005820: 6465 6e74 2054 6563 6845 6d70 6f77 6572  dent TechEmpower
-00005830: 2062 656e 6368 6d61 726b 7320 7368 6f77   benchmarks show
-00005840: 202a 2a46 6173 7441 5049 2a2a 2061 7070   **FastAPI** app
-00005850: 6c69 6361 7469 6f6e 7320 7275 6e6e 696e  lications runnin
-00005860: 6720 756e 6465 7220 5576 6963 6f72 6e20  g under Uvicorn 
-00005870: 6173 203c 6120 6872 6566 3d22 6874 7470  as <a href="http
-00005880: 733a 2f2f 7777 772e 7465 6368 656d 706f  s://www.techempo
-00005890: 7765 722e 636f 6d2f 6265 6e63 686d 6172  wer.com/benchmar
-000058a0: 6b73 2f23 7365 6374 696f 6e3d 7465 7374  ks/#section=test
-000058b0: 2672 756e 6964 3d37 3436 3465 3532 302d  &runid=7464e520-
-000058c0: 3064 6332 2d34 3733 642d 6264 3334 2d64  0dc2-473d-bd34-d
-000058d0: 6264 6664 3765 3835 3931 3126 6877 3d70  bdfd7e85911&hw=p
-000058e0: 6826 7465 7374 3d71 7565 7279 266c 3d7a  h&test=query&l=z
-000058f0: 696a 7a65 6e2d 3722 2063 6c61 7373 3d22  ijzen-7" class="
-00005900: 6578 7465 726e 616c 2d6c 696e 6b22 2074  external-link" t
-00005910: 6172 6765 743d 225f 626c 616e 6b22 3e6f  arget="_blank">o
-00005920: 6e65 206f 6620 7468 6520 6661 7374 6573  ne of the fastes
-00005930: 7420 5079 7468 6f6e 2066 7261 6d65 776f  t Python framewo
-00005940: 726b 7320 6176 6169 6c61 626c 653c 2f61  rks available</a
-00005950: 3e2c 206f 6e6c 7920 6265 6c6f 7720 5374  >, only below St
-00005960: 6172 6c65 7474 6520 616e 6420 5576 6963  arlette and Uvic
-00005970: 6f72 6e20 7468 656d 7365 6c76 6573 2028  orn themselves (
-00005980: 7573 6564 2069 6e74 6572 6e61 6c6c 7920  used internally 
-00005990: 6279 2046 6173 7441 5049 292e 2028 2a29  by FastAPI). (*)
-000059a0: 0a0a 546f 2075 6e64 6572 7374 616e 6420  ..To understand 
-000059b0: 6d6f 7265 2061 626f 7574 2069 742c 2073  more about it, s
-000059c0: 6565 2074 6865 2073 6563 7469 6f6e 203c  ee the section <
-000059d0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-000059e0: 6661 7374 6170 692e 7469 616e 676f 6c6f  fastapi.tiangolo
-000059f0: 2e63 6f6d 2f62 656e 6368 6d61 726b 732f  .com/benchmarks/
-00005a00: 2220 636c 6173 733d 2269 6e74 6572 6e61  " class="interna
-00005a10: 6c2d 6c69 6e6b 2220 7461 7267 6574 3d22  l-link" target="
-00005a20: 5f62 6c61 6e6b 223e 4265 6e63 686d 6172  _blank">Benchmar
-00005a30: 6b73 3c2f 613e 2e0a 0a23 2320 4f70 7469  ks</a>...## Opti
-00005a40: 6f6e 616c 2044 6570 656e 6465 6e63 6965  onal Dependencie
-00005a50: 730a 0a55 7365 6420 6279 2050 7964 616e  s..Used by Pydan
-00005a60: 7469 633a 0a0a 2a20 3c61 2068 7265 663d  tic:..* <a href=
-00005a70: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-00005a80: 636f 6d2f 6573 6e6d 652f 756c 7472 616a  com/esnme/ultraj
-00005a90: 736f 6e22 2074 6172 6765 743d 225f 626c  son" target="_bl
-00005aa0: 616e 6b22 3e3c 636f 6465 3e75 6a73 6f6e  ank"><code>ujson
-00005ab0: 3c2f 636f 6465 3e3c 2f61 3e20 2d20 666f  </code></a> - fo
-00005ac0: 7220 6661 7374 6572 204a 534f 4e20 3c61  r faster JSON <a
-00005ad0: 6262 7220 7469 746c 653d 2263 6f6e 7665  bbr title="conve
-00005ae0: 7274 696e 6720 7468 6520 7374 7269 6e67  rting the string
-00005af0: 2074 6861 7420 636f 6d65 7320 6672 6f6d   that comes from
-00005b00: 2061 6e20 4854 5450 2072 6571 7565 7374   an HTTP request
-00005b10: 2069 6e74 6f20 5079 7468 6f6e 2064 6174   into Python dat
-00005b20: 6122 3e22 7061 7273 696e 6722 3c2f 6162  a">"parsing"</ab
-00005b30: 6272 3e2e 0a2a 203c 6120 6872 6566 3d22  br>..* <a href="
-00005b40: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00005b50: 6f6d 2f4a 6f73 6844 6174 612f 7079 7468  om/JoshData/pyth
-00005b60: 6f6e 2d65 6d61 696c 2d76 616c 6964 6174  on-email-validat
-00005b70: 6f72 2220 7461 7267 6574 3d22 5f62 6c61  or" target="_bla
-00005b80: 6e6b 223e 3c63 6f64 653e 656d 6169 6c5f  nk"><code>email_
-00005b90: 7661 6c69 6461 746f 723c 2f63 6f64 653e  validator</code>
-00005ba0: 3c2f 613e 202d 2066 6f72 2065 6d61 696c  </a> - for email
-00005bb0: 2076 616c 6964 6174 696f 6e2e 0a0a 5573   validation...Us
-00005bc0: 6564 2062 7920 5374 6172 6c65 7474 653a  ed by Starlette:
-00005bd0: 0a0a 2a20 3c61 2068 7265 663d 2268 7474  ..* <a href="htt
-00005be0: 7073 3a2f 2f77 7777 2e70 7974 686f 6e2d  ps://www.python-
-00005bf0: 6874 7470 782e 6f72 6722 2074 6172 6765  httpx.org" targe
-00005c00: 743d 225f 626c 616e 6b22 3e3c 636f 6465  t="_blank"><code
-00005c10: 3e68 7474 7078 3c2f 636f 6465 3e3c 2f61  >httpx</code></a
-00005c20: 3e20 2d20 5265 7175 6972 6564 2069 6620  > - Required if 
-00005c30: 796f 7520 7761 6e74 2074 6f20 7573 6520  you want to use 
-00005c40: 7468 6520 6054 6573 7443 6c69 656e 7460  the `TestClient`
-00005c50: 2e0a 2a20 3c61 2068 7265 663d 2268 7474  ..* <a href="htt
-00005c60: 7073 3a2f 2f6a 696e 6a61 2e70 616c 6c65  ps://jinja.palle
-00005c70: 7473 7072 6f6a 6563 7473 2e63 6f6d 2220  tsprojects.com" 
-00005c80: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
-00005c90: 3c63 6f64 653e 6a69 6e6a 6132 3c2f 636f  <code>jinja2</co
-00005ca0: 6465 3e3c 2f61 3e20 2d20 5265 7175 6972  de></a> - Requir
-00005cb0: 6564 2069 6620 796f 7520 7761 6e74 2074  ed if you want t
-00005cc0: 6f20 7573 6520 7468 6520 6465 6661 756c  o use the defaul
-00005cd0: 7420 7465 6d70 6c61 7465 2063 6f6e 6669  t template confi
-00005ce0: 6775 7261 7469 6f6e 2e0a 2a20 3c61 2068  guration..* <a h
-00005cf0: 7265 663d 2268 7474 7073 3a2f 2f61 6e64  ref="https://and
-00005d00: 7265 772d 642e 6769 7468 7562 2e69 6f2f  rew-d.github.io/
-00005d10: 7079 7468 6f6e 2d6d 756c 7469 7061 7274  python-multipart
-00005d20: 2f22 2074 6172 6765 743d 225f 626c 616e  /" target="_blan
-00005d30: 6b22 3e3c 636f 6465 3e70 7974 686f 6e2d  k"><code>python-
-00005d40: 6d75 6c74 6970 6172 743c 2f63 6f64 653e  multipart</code>
-00005d50: 3c2f 613e 202d 2052 6571 7569 7265 6420  </a> - Required 
-00005d60: 6966 2079 6f75 2077 616e 7420 746f 2073  if you want to s
-00005d70: 7570 706f 7274 2066 6f72 6d20 3c61 6262  upport form <abb
-00005d80: 7220 7469 746c 653d 2263 6f6e 7665 7274  r title="convert
-00005d90: 696e 6720 7468 6520 7374 7269 6e67 2074  ing the string t
-00005da0: 6861 7420 636f 6d65 7320 6672 6f6d 2061  hat comes from a
-00005db0: 6e20 4854 5450 2072 6571 7565 7374 2069  n HTTP request i
-00005dc0: 6e74 6f20 5079 7468 6f6e 2064 6174 6122  nto Python data"
-00005dd0: 3e22 7061 7273 696e 6722 3c2f 6162 6272  >"parsing"</abbr
-00005de0: 3e2c 2077 6974 6820 6072 6571 7565 7374  >, with `request
-00005df0: 2e66 6f72 6d28 2960 2e0a 2a20 3c61 2068  .form()`..* <a h
-00005e00: 7265 663d 2268 7474 7073 3a2f 2f70 7974  ref="https://pyt
-00005e10: 686f 6e68 6f73 7465 642e 6f72 672f 6974  honhosted.org/it
-00005e20: 7364 616e 6765 726f 7573 2f22 2074 6172  sdangerous/" tar
-00005e30: 6765 743d 225f 626c 616e 6b22 3e3c 636f  get="_blank"><co
-00005e40: 6465 3e69 7473 6461 6e67 6572 6f75 733c  de>itsdangerous<
-00005e50: 2f63 6f64 653e 3c2f 613e 202d 2052 6571  /code></a> - Req
-00005e60: 7569 7265 6420 666f 7220 6053 6573 7369  uired for `Sessi
-00005e70: 6f6e 4d69 6464 6c65 7761 7265 6020 7375  onMiddleware` su
-00005e80: 7070 6f72 742e 0a2a 203c 6120 6872 6566  pport..* <a href
-00005e90: 3d22 6874 7470 733a 2f2f 7079 7961 6d6c  ="https://pyyaml
-00005ea0: 2e6f 7267 2f77 696b 692f 5079 5941 4d4c  .org/wiki/PyYAML
-00005eb0: 446f 6375 6d65 6e74 6174 696f 6e22 2074  Documentation" t
-00005ec0: 6172 6765 743d 225f 626c 616e 6b22 3e3c  arget="_blank"><
-00005ed0: 636f 6465 3e70 7979 616d 6c3c 2f63 6f64  code>pyyaml</cod
-00005ee0: 653e 3c2f 613e 202d 2052 6571 7569 7265  e></a> - Require
-00005ef0: 6420 666f 7220 5374 6172 6c65 7474 6527  d for Starlette'
-00005f00: 7320 6053 6368 656d 6147 656e 6572 6174  s `SchemaGenerat
-00005f10: 6f72 6020 7375 7070 6f72 7420 2879 6f75  or` support (you
-00005f20: 2070 726f 6261 626c 7920 646f 6e27 7420   probably don't 
-00005f30: 6e65 6564 2069 7420 7769 7468 2046 6173  need it with Fas
-00005f40: 7441 5049 292e 0a2a 203c 6120 6872 6566  tAPI)..* <a href
-00005f50: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
-00005f60: 2e63 6f6d 2f65 736e 6d65 2f75 6c74 7261  .com/esnme/ultra
-00005f70: 6a73 6f6e 2220 7461 7267 6574 3d22 5f62  json" target="_b
-00005f80: 6c61 6e6b 223e 3c63 6f64 653e 756a 736f  lank"><code>ujso
-00005f90: 6e3c 2f63 6f64 653e 3c2f 613e 202d 2052  n</code></a> - R
-00005fa0: 6571 7569 7265 6420 6966 2079 6f75 2077  equired if you w
-00005fb0: 616e 7420 746f 2075 7365 2060 554a 534f  ant to use `UJSO
-00005fc0: 4e52 6573 706f 6e73 6560 2e0a 0a55 7365  NResponse`...Use
-00005fd0: 6420 6279 2046 6173 7441 5049 202f 2053  d by FastAPI / S
-00005fe0: 7461 726c 6574 7465 3a0a 0a2a 203c 6120  tarlette:..* <a 
-00005ff0: 6872 6566 3d22 6874 7470 733a 2f2f 7777  href="https://ww
-00006000: 772e 7576 6963 6f72 6e2e 6f72 6722 2074  w.uvicorn.org" t
-00006010: 6172 6765 743d 225f 626c 616e 6b22 3e3c  arget="_blank"><
-00006020: 636f 6465 3e75 7669 636f 726e 3c2f 636f  code>uvicorn</co
-00006030: 6465 3e3c 2f61 3e20 2d20 666f 7220 7468  de></a> - for th
-00006040: 6520 7365 7276 6572 2074 6861 7420 6c6f  e server that lo
-00006050: 6164 7320 616e 6420 7365 7276 6573 2079  ads and serves y
-00006060: 6f75 7220 6170 706c 6963 6174 696f 6e2e  our application.
-00006070: 0a2a 203c 6120 6872 6566 3d22 6874 7470  .* <a href="http
-00006080: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f69  s://github.com/i
-00006090: 6a6c 2f6f 726a 736f 6e22 2074 6172 6765  jl/orjson" targe
-000060a0: 743d 225f 626c 616e 6b22 3e3c 636f 6465  t="_blank"><code
-000060b0: 3e6f 726a 736f 6e3c 2f63 6f64 653e 3c2f  >orjson</code></
-000060c0: 613e 202d 2052 6571 7569 7265 6420 6966  a> - Required if
-000060d0: 2079 6f75 2077 616e 7420 746f 2075 7365   you want to use
-000060e0: 2060 4f52 4a53 4f4e 5265 7370 6f6e 7365   `ORJSONResponse
-000060f0: 602e 0a0a 596f 7520 6361 6e20 696e 7374  `...You can inst
-00006100: 616c 6c20 616c 6c20 6f66 2074 6865 7365  all all of these
-00006110: 2077 6974 6820 6070 6970 2069 6e73 7461   with `pip insta
-00006120: 6c6c 2022 6661 7374 6170 695b 616c 6c5d  ll "fastapi[all]
-00006130: 2260 2e0a 0a23 2320 4c69 6365 6e73 650a  "`...## License.
-00006140: 0a54 6869 7320 7072 6f6a 6563 7420 6973  .This project is
-00006150: 206c 6963 656e 7365 6420 756e 6465 7220   licensed under 
-00006160: 7468 6520 7465 726d 7320 6f66 2074 6865  the terms of the
-00006170: 204d 4954 206c 6963 656e 7365 2e0a        MIT license..
+000008e0: 2761 6c6c 270a 4465 7363 7269 7074 696f  'all'.Descriptio
+000008f0: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
+00000900: 7465 7874 2f6d 6172 6b64 6f77 6e0a 0a3c  text/markdown..<
+00000910: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
+00000920: 3e0a 2020 3c61 2068 7265 663d 2268 7474  >.  <a href="htt
+00000930: 7073 3a2f 2f66 6173 7461 7069 2e74 6961  ps://fastapi.tia
+00000940: 6e67 6f6c 6f2e 636f 6d22 3e3c 696d 6720  ngolo.com"><img 
+00000950: 7372 633d 2268 7474 7073 3a2f 2f66 6173  src="https://fas
+00000960: 7461 7069 2e74 6961 6e67 6f6c 6f2e 636f  tapi.tiangolo.co
+00000970: 6d2f 696d 672f 6c6f 676f 2d6d 6172 6769  m/img/logo-margi
+00000980: 6e2f 6c6f 676f 2d74 6561 6c2e 706e 6722  n/logo-teal.png"
+00000990: 2061 6c74 3d22 4661 7374 4150 4922 3e3c   alt="FastAPI"><
+000009a0: 2f61 3e0a 3c2f 703e 0a3c 7020 616c 6967  /a>.</p>.<p alig
+000009b0: 6e3d 2263 656e 7465 7222 3e0a 2020 2020  n="center">.    
+000009c0: 3c65 6d3e 4661 7374 4150 4920 6672 616d  <em>FastAPI fram
+000009d0: 6577 6f72 6b2c 2068 6967 6820 7065 7266  ework, high perf
+000009e0: 6f72 6d61 6e63 652c 2065 6173 7920 746f  ormance, easy to
+000009f0: 206c 6561 726e 2c20 6661 7374 2074 6f20   learn, fast to 
+00000a00: 636f 6465 2c20 7265 6164 7920 666f 7220  code, ready for 
+00000a10: 7072 6f64 7563 7469 6f6e 3c2f 656d 3e0a  production</em>.
+00000a20: 3c2f 703e 0a3c 7020 616c 6967 6e3d 2263  </p>.<p align="c
+00000a30: 656e 7465 7222 3e0a 3c61 2068 7265 663d  enter">.<a href=
+00000a40: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00000a50: 636f 6d2f 7469 616e 676f 6c6f 2f66 6173  com/tiangolo/fas
+00000a60: 7461 7069 2f61 6374 696f 6e73 3f71 7565  tapi/actions?que
+00000a70: 7279 3d77 6f72 6b66 6c6f 7725 3341 5465  ry=workflow%3ATe
+00000a80: 7374 2b65 7665 6e74 2533 4170 7573 682b  st+event%3Apush+
+00000a90: 6272 616e 6368 2533 416d 6173 7465 7222  branch%3Amaster"
+00000aa0: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+00000ab0: 3e0a 2020 2020 3c69 6d67 2073 7263 3d22  >.    <img src="
+00000ac0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000ad0: 6f6d 2f74 6961 6e67 6f6c 6f2f 6661 7374  om/tiangolo/fast
+00000ae0: 6170 692f 776f 726b 666c 6f77 732f 5465  api/workflows/Te
+00000af0: 7374 2f62 6164 6765 2e73 7667 3f65 7665  st/badge.svg?eve
+00000b00: 6e74 3d70 7573 6826 6272 616e 6368 3d6d  nt=push&branch=m
+00000b10: 6173 7465 7222 2061 6c74 3d22 5465 7374  aster" alt="Test
+00000b20: 223e 0a3c 2f61 3e0a 3c61 2068 7265 663d  ">.</a>.<a href=
+00000b30: 2268 7474 7073 3a2f 2f63 6f76 6572 6167  "https://coverag
+00000b40: 652d 6261 6467 652e 7361 6d75 656c 636f  e-badge.samuelco
+00000b50: 6c76 696e 2e77 6f72 6b65 7273 2e64 6576  lvin.workers.dev
+00000b60: 2f72 6564 6972 6563 742f 7469 616e 676f  /redirect/tiango
+00000b70: 6c6f 2f66 6173 7461 7069 2220 7461 7267  lo/fastapi" targ
+00000b80: 6574 3d22 5f62 6c61 6e6b 223e 0a20 2020  et="_blank">.   
+00000b90: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
+00000ba0: 3a2f 2f63 6f76 6572 6167 652d 6261 6467  ://coverage-badg
+00000bb0: 652e 7361 6d75 656c 636f 6c76 696e 2e77  e.samuelcolvin.w
+00000bc0: 6f72 6b65 7273 2e64 6576 2f74 6961 6e67  orkers.dev/tiang
+00000bd0: 6f6c 6f2f 6661 7374 6170 692e 7376 6722  olo/fastapi.svg"
+00000be0: 2061 6c74 3d22 436f 7665 7261 6765 223e   alt="Coverage">
+00000bf0: 0a3c 2f61 3e0a 3c61 2068 7265 663d 2268  .</a>.<a href="h
+00000c00: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
+00000c10: 7072 6f6a 6563 742f 6661 7374 6170 6922  project/fastapi"
+00000c20: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+00000c30: 3e0a 2020 2020 3c69 6d67 2073 7263 3d22  >.    <img src="
+00000c40: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000c50: 6c64 732e 696f 2f70 7970 692f 762f 6661  lds.io/pypi/v/fa
+00000c60: 7374 6170 693f 636f 6c6f 723d 2532 3333  stapi?color=%233
+00000c70: 3444 3035 3826 6c61 6265 6c3d 7079 7069  4D058&label=pypi
+00000c80: 2532 3070 6163 6b61 6765 2220 616c 743d  %20package" alt=
+00000c90: 2250 6163 6b61 6765 2076 6572 7369 6f6e  "Package version
+00000ca0: 223e 0a3c 2f61 3e0a 3c61 2068 7265 663d  ">.</a>.<a href=
+00000cb0: 2268 7474 7073 3a2f 2f70 7970 692e 6f72  "https://pypi.or
+00000cc0: 672f 7072 6f6a 6563 742f 6661 7374 6170  g/project/fastap
+00000cd0: 6922 2074 6172 6765 743d 225f 626c 616e  i" target="_blan
+00000ce0: 6b22 3e0a 2020 2020 3c69 6d67 2073 7263  k">.    <img src
+00000cf0: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+00000d00: 6965 6c64 732e 696f 2f70 7970 692f 7079  ields.io/pypi/py
+00000d10: 7665 7273 696f 6e73 2f66 6173 7461 7069  versions/fastapi
+00000d20: 2e73 7667 3f63 6f6c 6f72 3d25 3233 3334  .svg?color=%2334
+00000d30: 4430 3538 2220 616c 743d 2253 7570 706f  D058" alt="Suppo
+00000d40: 7274 6564 2050 7974 686f 6e20 7665 7273  rted Python vers
+00000d50: 696f 6e73 223e 0a3c 2f61 3e0a 3c2f 703e  ions">.</a>.</p>
+00000d60: 0a0a 2d2d 2d0a 0a2a 2a44 6f63 756d 656e  ..---..**Documen
+00000d70: 7461 7469 6f6e 2a2a 3a20 3c61 2068 7265  tation**: <a hre
+00000d80: 663d 2268 7474 7073 3a2f 2f66 6173 7461  f="https://fasta
+00000d90: 7069 2e74 6961 6e67 6f6c 6f2e 636f 6d22  pi.tiangolo.com"
+00000da0: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+00000db0: 3e68 7474 7073 3a2f 2f66 6173 7461 7069  >https://fastapi
+00000dc0: 2e74 6961 6e67 6f6c 6f2e 636f 6d3c 2f61  .tiangolo.com</a
+00000dd0: 3e0a 0a2a 2a53 6f75 7263 6520 436f 6465  >..**Source Code
+00000de0: 2a2a 3a20 3c61 2068 7265 663d 2268 7474  **: <a href="htt
+00000df0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000e00: 7469 616e 676f 6c6f 2f66 6173 7461 7069  tiangolo/fastapi
+00000e10: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+00000e20: 223e 6874 7470 733a 2f2f 6769 7468 7562  ">https://github
+00000e30: 2e63 6f6d 2f74 6961 6e67 6f6c 6f2f 6661  .com/tiangolo/fa
+00000e40: 7374 6170 693c 2f61 3e0a 0a2d 2d2d 0a0a  stapi</a>..---..
+00000e50: 4661 7374 4150 4920 6973 2061 206d 6f64  FastAPI is a mod
+00000e60: 6572 6e2c 2066 6173 7420 2868 6967 682d  ern, fast (high-
+00000e70: 7065 7266 6f72 6d61 6e63 6529 2c20 7765  performance), we
+00000e80: 6220 6672 616d 6577 6f72 6b20 666f 7220  b framework for 
+00000e90: 6275 696c 6469 6e67 2041 5049 7320 7769  building APIs wi
+00000ea0: 7468 2050 7974 686f 6e20 332e 372b 2062  th Python 3.7+ b
+00000eb0: 6173 6564 206f 6e20 7374 616e 6461 7264  ased on standard
+00000ec0: 2050 7974 686f 6e20 7479 7065 2068 696e   Python type hin
+00000ed0: 7473 2e0a 0a54 6865 206b 6579 2066 6561  ts...The key fea
+00000ee0: 7475 7265 7320 6172 653a 0a0a 2a20 2a2a  tures are:..* **
+00000ef0: 4661 7374 2a2a 3a20 5665 7279 2068 6967  Fast**: Very hig
+00000f00: 6820 7065 7266 6f72 6d61 6e63 652c 206f  h performance, o
+00000f10: 6e20 7061 7220 7769 7468 202a 2a4e 6f64  n par with **Nod
+00000f20: 654a 532a 2a20 616e 6420 2a2a 476f 2a2a  eJS** and **Go**
+00000f30: 2028 7468 616e 6b73 2074 6f20 5374 6172   (thanks to Star
+00000f40: 6c65 7474 6520 616e 6420 5079 6461 6e74  lette and Pydant
+00000f50: 6963 292e 205b 4f6e 6520 6f66 2074 6865  ic). [One of the
+00000f60: 2066 6173 7465 7374 2050 7974 686f 6e20   fastest Python 
+00000f70: 6672 616d 6577 6f72 6b73 2061 7661 696c  frameworks avail
+00000f80: 6162 6c65 5d28 2370 6572 666f 726d 616e  able](#performan
+00000f90: 6365 292e 0a2a 202a 2a46 6173 7420 746f  ce)..* **Fast to
+00000fa0: 2063 6f64 652a 2a3a 2049 6e63 7265 6173   code**: Increas
+00000fb0: 6520 7468 6520 7370 6565 6420 746f 2064  e the speed to d
+00000fc0: 6576 656c 6f70 2066 6561 7475 7265 7320  evelop features 
+00000fd0: 6279 2061 626f 7574 2032 3030 2520 746f  by about 200% to
+00000fe0: 2033 3030 252e 202a 0a2a 202a 2a46 6577   300%. *.* **Few
+00000ff0: 6572 2062 7567 732a 2a3a 2052 6564 7563  er bugs**: Reduc
+00001000: 6520 6162 6f75 7420 3430 2520 6f66 2068  e about 40% of h
+00001010: 756d 616e 2028 6465 7665 6c6f 7065 7229  uman (developer)
+00001020: 2069 6e64 7563 6564 2065 7272 6f72 732e   induced errors.
+00001030: 202a 0a2a 202a 2a49 6e74 7569 7469 7665   *.* **Intuitive
+00001040: 2a2a 3a20 4772 6561 7420 6564 6974 6f72  **: Great editor
+00001050: 2073 7570 706f 7274 2e20 3c61 6262 7220   support. <abbr 
+00001060: 7469 746c 653d 2261 6c73 6f20 6b6e 6f77  title="also know
+00001070: 6e20 6173 2061 7574 6f2d 636f 6d70 6c65  n as auto-comple
+00001080: 7465 2c20 6175 746f 636f 6d70 6c65 7469  te, autocompleti
+00001090: 6f6e 2c20 496e 7465 6c6c 6953 656e 7365  on, IntelliSense
+000010a0: 223e 436f 6d70 6c65 7469 6f6e 3c2f 6162  ">Completion</ab
+000010b0: 6272 3e20 6576 6572 7977 6865 7265 2e20  br> everywhere. 
+000010c0: 4c65 7373 2074 696d 6520 6465 6275 6767  Less time debugg
+000010d0: 696e 672e 0a2a 202a 2a45 6173 792a 2a3a  ing..* **Easy**:
+000010e0: 2044 6573 6967 6e65 6420 746f 2062 6520   Designed to be 
+000010f0: 6561 7379 2074 6f20 7573 6520 616e 6420  easy to use and 
+00001100: 6c65 6172 6e2e 204c 6573 7320 7469 6d65  learn. Less time
+00001110: 2072 6561 6469 6e67 2064 6f63 732e 0a2a   reading docs..*
+00001120: 202a 2a53 686f 7274 2a2a 3a20 4d69 6e69   **Short**: Mini
+00001130: 6d69 7a65 2063 6f64 6520 6475 706c 6963  mize code duplic
+00001140: 6174 696f 6e2e 204d 756c 7469 706c 6520  ation. Multiple 
+00001150: 6665 6174 7572 6573 2066 726f 6d20 6561  features from ea
+00001160: 6368 2070 6172 616d 6574 6572 2064 6563  ch parameter dec
+00001170: 6c61 7261 7469 6f6e 2e20 4665 7765 7220  laration. Fewer 
+00001180: 6275 6773 2e0a 2a20 2a2a 526f 6275 7374  bugs..* **Robust
+00001190: 2a2a 3a20 4765 7420 7072 6f64 7563 7469  **: Get producti
+000011a0: 6f6e 2d72 6561 6479 2063 6f64 652e 2057  on-ready code. W
+000011b0: 6974 6820 6175 746f 6d61 7469 6320 696e  ith automatic in
+000011c0: 7465 7261 6374 6976 6520 646f 6375 6d65  teractive docume
+000011d0: 6e74 6174 696f 6e2e 0a2a 202a 2a53 7461  ntation..* **Sta
+000011e0: 6e64 6172 6473 2d62 6173 6564 2a2a 3a20  ndards-based**: 
+000011f0: 4261 7365 6420 6f6e 2028 616e 6420 6675  Based on (and fu
+00001200: 6c6c 7920 636f 6d70 6174 6962 6c65 2077  lly compatible w
+00001210: 6974 6829 2074 6865 206f 7065 6e20 7374  ith) the open st
+00001220: 616e 6461 7264 7320 666f 7220 4150 4973  andards for APIs
+00001230: 3a20 3c61 2068 7265 663d 2268 7474 7073  : <a href="https
+00001240: 3a2f 2f67 6974 6875 622e 636f 6d2f 4f41  ://github.com/OA
+00001250: 492f 4f70 656e 4150 492d 5370 6563 6966  I/OpenAPI-Specif
+00001260: 6963 6174 696f 6e22 2063 6c61 7373 3d22  ication" class="
+00001270: 6578 7465 726e 616c 2d6c 696e 6b22 2074  external-link" t
+00001280: 6172 6765 743d 225f 626c 616e 6b22 3e4f  arget="_blank">O
+00001290: 7065 6e41 5049 3c2f 613e 2028 7072 6576  penAPI</a> (prev
+000012a0: 696f 7573 6c79 206b 6e6f 776e 2061 7320  iously known as 
+000012b0: 5377 6167 6765 7229 2061 6e64 203c 6120  Swagger) and <a 
+000012c0: 6872 6566 3d22 6874 7470 733a 2f2f 6a73  href="https://js
+000012d0: 6f6e 2d73 6368 656d 612e 6f72 672f 2220  on-schema.org/" 
+000012e0: 636c 6173 733d 2265 7874 6572 6e61 6c2d  class="external-
+000012f0: 6c69 6e6b 2220 7461 7267 6574 3d22 5f62  link" target="_b
+00001300: 6c61 6e6b 223e 4a53 4f4e 2053 6368 656d  lank">JSON Schem
+00001310: 613c 2f61 3e2e 0a0a 3c73 6d61 6c6c 3e2a  a</a>...<small>*
+00001320: 2065 7374 696d 6174 696f 6e20 6261 7365   estimation base
+00001330: 6420 6f6e 2074 6573 7473 206f 6e20 616e  d on tests on an
+00001340: 2069 6e74 6572 6e61 6c20 6465 7665 6c6f   internal develo
+00001350: 706d 656e 7420 7465 616d 2c20 6275 696c  pment team, buil
+00001360: 6469 6e67 2070 726f 6475 6374 696f 6e20  ding production 
+00001370: 6170 706c 6963 6174 696f 6e73 2e3c 2f73  applications.</s
+00001380: 6d61 6c6c 3e0a 0a23 2320 5370 6f6e 736f  mall>..## Sponso
+00001390: 7273 0a0a 3c21 2d2d 2073 706f 6e73 6f72  rs..<!-- sponsor
+000013a0: 7320 2d2d 3e0a 0a3c 6120 6872 6566 3d22  s -->..<a href="
+000013b0: 6874 7470 733a 2f2f 6372 7970 7461 7069  https://cryptapi
+000013c0: 2e69 6f2f 2220 7461 7267 6574 3d22 5f62  .io/" target="_b
+000013d0: 6c61 6e6b 2220 7469 746c 653d 2243 7279  lank" title="Cry
+000013e0: 7074 4150 493a 2059 6f75 7220 6561 7379  ptAPI: Your easy
+000013f0: 2074 6f20 7573 652c 2073 6563 7572 6520   to use, secure 
+00001400: 616e 6420 7072 6976 6163 7920 6f72 6965  and privacy orie
+00001410: 6e74 6564 2070 6179 6d65 6e74 2067 6174  nted payment gat
+00001420: 6577 6179 2e22 3e3c 696d 6720 7372 633d  eway."><img src=
+00001430: 2268 7474 7073 3a2f 2f66 6173 7461 7069  "https://fastapi
+00001440: 2e74 6961 6e67 6f6c 6f2e 636f 6d2f 696d  .tiangolo.com/im
+00001450: 672f 7370 6f6e 736f 7273 2f63 7279 7074  g/sponsors/crypt
+00001460: 6170 692e 7376 6722 3e3c 2f61 3e0a 3c61  api.svg"></a>.<a
+00001470: 2068 7265 663d 2268 7474 7073 3a2f 2f70   href="https://p
+00001480: 6c61 7466 6f72 6d2e 7368 2f74 7279 2d69  latform.sh/try-i
+00001490: 742d 6e6f 772f 3f75 746d 5f73 6f75 7263  t-now/?utm_sourc
+000014a0: 653d 6661 7374 6170 692d 7369 676e 7570  e=fastapi-signup
+000014b0: 2675 746d 5f6d 6564 6975 6d3d 6261 6e6e  &utm_medium=bann
+000014c0: 6572 2675 746d 5f63 616d 7061 6967 6e3d  er&utm_campaign=
+000014d0: 4661 7374 4150 492d 7369 676e 7570 2d4a  FastAPI-signup-J
+000014e0: 756e 652d 3230 3233 2220 7461 7267 6574  une-2023" target
+000014f0: 3d22 5f62 6c61 6e6b 2220 7469 746c 653d  ="_blank" title=
+00001500: 2242 7569 6c64 2c20 7275 6e20 616e 6420  "Build, run and 
+00001510: 7363 616c 6520 796f 7572 2061 7070 7320  scale your apps 
+00001520: 6f6e 2061 206d 6f64 6572 6e2c 2072 656c  on a modern, rel
+00001530: 6961 626c 652c 2061 6e64 2073 6563 7572  iable, and secur
+00001540: 6520 5061 6153 2e22 3e3c 696d 6720 7372  e PaaS."><img sr
+00001550: 633d 2268 7474 7073 3a2f 2f66 6173 7461  c="https://fasta
+00001560: 7069 2e74 6961 6e67 6f6c 6f2e 636f 6d2f  pi.tiangolo.com/
+00001570: 696d 672f 7370 6f6e 736f 7273 2f70 6c61  img/sponsors/pla
+00001580: 7466 6f72 6d2d 7368 2e70 6e67 223e 3c2f  tform-sh.png"></
+00001590: 613e 0a3c 6120 6872 6566 3d22 6874 7470  a>.<a href="http
+000015a0: 733a 2f2f 7777 772e 6465 7461 2e73 682f  s://www.deta.sh/
+000015b0: 3f72 6566 3d66 6173 7461 7069 2220 7461  ?ref=fastapi" ta
+000015c0: 7267 6574 3d22 5f62 6c61 6e6b 2220 7469  rget="_blank" ti
+000015d0: 746c 653d 2254 6865 206c 6175 6e63 6870  tle="The launchp
+000015e0: 6164 2066 6f72 2061 6c6c 2079 6f75 7220  ad for all your 
+000015f0: 2874 6561 6d27 7329 2069 6465 6173 223e  (team's) ideas">
+00001600: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00001610: 2f2f 6661 7374 6170 692e 7469 616e 676f  //fastapi.tiango
+00001620: 6c6f 2e63 6f6d 2f69 6d67 2f73 706f 6e73  lo.com/img/spons
+00001630: 6f72 732f 6465 7461 2e73 7667 223e 3c2f  ors/deta.svg"></
+00001640: 613e 0a3c 6120 6872 6566 3d22 6874 7470  a>.<a href="http
+00001650: 733a 2f2f 7472 6169 6e69 6e67 2e74 616c  s://training.tal
+00001660: 6b70 7974 686f 6e2e 666d 2f66 6173 7461  kpython.fm/fasta
+00001670: 7069 2d63 6f75 7273 6573 2220 7461 7267  pi-courses" targ
+00001680: 6574 3d22 5f62 6c61 6e6b 2220 7469 746c  et="_blank" titl
+00001690: 653d 2246 6173 7441 5049 2076 6964 656f  e="FastAPI video
+000016a0: 2063 6f75 7273 6573 206f 6e20 6465 6d61   courses on dema
+000016b0: 6e64 2066 726f 6d20 7065 6f70 6c65 2079  nd from people y
+000016c0: 6f75 2074 7275 7374 223e 3c69 6d67 2073  ou trust"><img s
+000016d0: 7263 3d22 6874 7470 733a 2f2f 6661 7374  rc="https://fast
+000016e0: 6170 692e 7469 616e 676f 6c6f 2e63 6f6d  api.tiangolo.com
+000016f0: 2f69 6d67 2f73 706f 6e73 6f72 732f 7461  /img/sponsors/ta
+00001700: 6c6b 7079 7468 6f6e 2e70 6e67 223e 3c2f  lkpython.png"></
+00001710: 613e 0a3c 6120 6872 6566 3d22 6874 7470  a>.<a href="http
+00001720: 733a 2f2f 7465 7374 6472 6976 656e 2e69  s://testdriven.i
+00001730: 6f2f 636f 7572 7365 732f 7464 642d 6661  o/courses/tdd-fa
+00001740: 7374 6170 692f 2220 7461 7267 6574 3d22  stapi/" target="
+00001750: 5f62 6c61 6e6b 2220 7469 746c 653d 224c  _blank" title="L
+00001760: 6561 726e 2074 6f20 6275 696c 6420 6869  earn to build hi
+00001770: 6768 2d71 7561 6c69 7479 2077 6562 2061  gh-quality web a
+00001780: 7070 7320 7769 7468 2062 6573 7420 7072  pps with best pr
+00001790: 6163 7469 6365 7322 3e3c 696d 6720 7372  actices"><img sr
+000017a0: 633d 2268 7474 7073 3a2f 2f66 6173 7461  c="https://fasta
+000017b0: 7069 2e74 6961 6e67 6f6c 6f2e 636f 6d2f  pi.tiangolo.com/
+000017c0: 696d 672f 7370 6f6e 736f 7273 2f74 6573  img/sponsors/tes
+000017d0: 7464 7269 7665 6e2e 7376 6722 3e3c 2f61  tdriven.svg"></a
+000017e0: 3e0a 3c61 2068 7265 663d 2268 7474 7073  >.<a href="https
+000017f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6465  ://github.com/de
+00001800: 6570 7365 742d 6169 2f68 6179 7374 6163  epset-ai/haystac
+00001810: 6b2f 2220 7461 7267 6574 3d22 5f62 6c61  k/" target="_bla
+00001820: 6e6b 2220 7469 746c 653d 2242 7569 6c64  nk" title="Build
+00001830: 2070 6f77 6572 6675 6c20 7365 6172 6368   powerful search
+00001840: 2066 726f 6d20 636f 6d70 6f73 6162 6c65   from composable
+00001850: 2c20 6f70 656e 2073 6f75 7263 6520 6275  , open source bu
+00001860: 696c 6469 6e67 2062 6c6f 636b 7322 3e3c  ilding blocks"><
+00001870: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00001880: 2f66 6173 7461 7069 2e74 6961 6e67 6f6c  /fastapi.tiangol
+00001890: 6f2e 636f 6d2f 696d 672f 7370 6f6e 736f  o.com/img/sponso
+000018a0: 7273 2f68 6179 7374 6163 6b2d 6661 7374  rs/haystack-fast
+000018b0: 6170 692e 7376 6722 3e3c 2f61 3e0a 3c61  api.svg"></a>.<a
+000018c0: 2068 7265 663d 2268 7474 7073 3a2f 2f63   href="https://c
+000018d0: 6172 6565 7273 2e70 6f77 656e 732e 636f  areers.powens.co
+000018e0: 6d2f 2220 7461 7267 6574 3d22 5f62 6c61  m/" target="_bla
+000018f0: 6e6b 2220 7469 746c 653d 2250 6f77 656e  nk" title="Powen
+00001900: 7320 6973 2068 6972 696e 6721 223e 3c69  s is hiring!"><i
+00001910: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00001920: 6661 7374 6170 692e 7469 616e 676f 6c6f  fastapi.tiangolo
+00001930: 2e63 6f6d 2f69 6d67 2f73 706f 6e73 6f72  .com/img/sponsor
+00001940: 732f 706f 7765 6e73 2e70 6e67 223e 3c2f  s/powens.png"></
+00001950: 613e 0a3c 6120 6872 6566 3d22 6874 7470  a>.<a href="http
+00001960: 733a 2f2f 7777 772e 7376 6978 2e63 6f6d  s://www.svix.com
+00001970: 2f22 2074 6172 6765 743d 225f 626c 616e  /" target="_blan
+00001980: 6b22 2074 6974 6c65 3d22 5376 6978 202d  k" title="Svix -
+00001990: 2057 6562 686f 6f6b 7320 6173 2061 2073   Webhooks as a s
+000019a0: 6572 7669 6365 223e 3c69 6d67 2073 7263  ervice"><img src
+000019b0: 3d22 6874 7470 733a 2f2f 6661 7374 6170  ="https://fastap
+000019c0: 692e 7469 616e 676f 6c6f 2e63 6f6d 2f69  i.tiangolo.com/i
+000019d0: 6d67 2f73 706f 6e73 6f72 732f 7376 6978  mg/sponsors/svix
+000019e0: 2e73 7667 223e 3c2f 613e 0a3c 6120 6872  .svg"></a>.<a hr
+000019f0: 6566 3d22 6874 7470 733a 2f2f 6461 7461  ef="https://data
+00001a00: 6265 6e74 6f2e 636f 6d2f 2220 7461 7267  bento.com/" targ
+00001a10: 6574 3d22 5f62 6c61 6e6b 2220 7469 746c  et="_blank" titl
+00001a20: 653d 2250 6179 2061 7320 796f 7520 676f  e="Pay as you go
+00001a30: 2066 6f72 206d 6172 6b65 7420 6461 7461   for market data
+00001a40: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+00001a50: 733a 2f2f 6661 7374 6170 692e 7469 616e  s://fastapi.tian
+00001a60: 676f 6c6f 2e63 6f6d 2f69 6d67 2f73 706f  golo.com/img/spo
+00001a70: 6e73 6f72 732f 6461 7461 6265 6e74 6f2e  nsors/databento.
+00001a80: 7376 6722 3e3c 2f61 3e0a 0a3c 212d 2d20  svg"></a>..<!-- 
+00001a90: 2f73 706f 6e73 6f72 7320 2d2d 3e0a 0a3c  /sponsors -->..<
+00001aa0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00001ab0: 6661 7374 6170 692e 7469 616e 676f 6c6f  fastapi.tiangolo
+00001ac0: 2e63 6f6d 2f66 6173 7461 7069 2d70 656f  .com/fastapi-peo
+00001ad0: 706c 652f 2373 706f 6e73 6f72 7322 2063  ple/#sponsors" c
+00001ae0: 6c61 7373 3d22 6578 7465 726e 616c 2d6c  lass="external-l
+00001af0: 696e 6b22 2074 6172 6765 743d 225f 626c  ink" target="_bl
+00001b00: 616e 6b22 3e4f 7468 6572 2073 706f 6e73  ank">Other spons
+00001b10: 6f72 733c 2f61 3e0a 0a23 2320 4f70 696e  ors</a>..## Opin
+00001b20: 696f 6e73 0a0a 225f 5b2e 2e2e 5d20 4927  ions.."_[...] I'
+00001b30: 6d20 7573 696e 6720 2a2a 4661 7374 4150  m using **FastAP
+00001b40: 492a 2a20 6120 746f 6e20 7468 6573 6520  I** a ton these 
+00001b50: 6461 7973 2e20 5b2e 2e2e 5d20 4927 6d20  days. [...] I'm 
+00001b60: 6163 7475 616c 6c79 2070 6c61 6e6e 696e  actually plannin
+00001b70: 6720 746f 2075 7365 2069 7420 666f 7220  g to use it for 
+00001b80: 616c 6c20 6f66 206d 7920 7465 616d 2773  all of my team's
+00001b90: 202a 2a4d 4c20 7365 7276 6963 6573 2061   **ML services a
+00001ba0: 7420 4d69 6372 6f73 6f66 742a 2a2e 2053  t Microsoft**. S
+00001bb0: 6f6d 6520 6f66 2074 6865 6d20 6172 6520  ome of them are 
+00001bc0: 6765 7474 696e 6720 696e 7465 6772 6174  getting integrat
+00001bd0: 6564 2069 6e74 6f20 7468 6520 636f 7265  ed into the core
+00001be0: 202a 2a57 696e 646f 7773 2a2a 2070 726f   **Windows** pro
+00001bf0: 6475 6374 2061 6e64 2073 6f6d 6520 2a2a  duct and some **
+00001c00: 4f66 6669 6365 2a2a 2070 726f 6475 6374  Office** product
+00001c10: 732e 5f22 0a0a 3c64 6976 2073 7479 6c65  s._"..<div style
+00001c20: 3d22 7465 7874 2d61 6c69 676e 3a20 7269  ="text-align: ri
+00001c30: 6768 743b 206d 6172 6769 6e2d 7269 6768  ght; margin-righ
+00001c40: 743a 2031 3025 3b22 3e4b 6162 6972 204b  t: 10%;">Kabir K
+00001c50: 6861 6e20 2d20 3c73 7472 6f6e 673e 4d69  han - <strong>Mi
+00001c60: 6372 6f73 6f66 743c 2f73 7472 6f6e 673e  crosoft</strong>
+00001c70: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+00001c80: 2f2f 6769 7468 7562 2e63 6f6d 2f74 6961  //github.com/tia
+00001c90: 6e67 6f6c 6f2f 6661 7374 6170 692f 7075  ngolo/fastapi/pu
+00001ca0: 6c6c 2f32 3622 2074 6172 6765 743d 225f  ll/26" target="_
+00001cb0: 626c 616e 6b22 3e3c 736d 616c 6c3e 2872  blank"><small>(r
+00001cc0: 6566 293c 2f73 6d61 6c6c 3e3c 2f61 3e3c  ef)</small></a><
+00001cd0: 2f64 6976 3e0a 0a2d 2d2d 0a0a 225f 5765  /div>..---.."_We
+00001ce0: 2061 646f 7074 6564 2074 6865 202a 2a46   adopted the **F
+00001cf0: 6173 7441 5049 2a2a 206c 6962 7261 7279  astAPI** library
+00001d00: 2074 6f20 7370 6177 6e20 6120 2a2a 5245   to spawn a **RE
+00001d10: 5354 2a2a 2073 6572 7665 7220 7468 6174  ST** server that
+00001d20: 2063 616e 2062 6520 7175 6572 6965 6420   can be queried 
+00001d30: 746f 206f 6274 6169 6e20 2a2a 7072 6564  to obtain **pred
+00001d40: 6963 7469 6f6e 732a 2a2e 205b 666f 7220  ictions**. [for 
+00001d50: 4c75 6477 6967 5d5f 220a 0a3c 6469 7620  Ludwig]_"..<div 
+00001d60: 7374 796c 653d 2274 6578 742d 616c 6967  style="text-alig
+00001d70: 6e3a 2072 6967 6874 3b20 6d61 7267 696e  n: right; margin
+00001d80: 2d72 6967 6874 3a20 3130 253b 223e 5069  -right: 10%;">Pi
+00001d90: 6572 6f20 4d6f 6c69 6e6f 2c20 5961 726f  ero Molino, Yaro
+00001da0: 736c 6176 2044 7564 696e 2c20 616e 6420  slav Dudin, and 
+00001db0: 5361 6920 5375 6d61 6e74 6820 4d69 7279  Sai Sumanth Miry
+00001dc0: 616c 6120 2d20 3c73 7472 6f6e 673e 5562  ala - <strong>Ub
+00001dd0: 6572 3c2f 7374 726f 6e67 3e20 3c61 2068  er</strong> <a h
+00001de0: 7265 663d 2268 7474 7073 3a2f 2f65 6e67  ref="https://eng
+00001df0: 2e75 6265 722e 636f 6d2f 6c75 6477 6967  .uber.com/ludwig
+00001e00: 2d76 302d 322f 2220 7461 7267 6574 3d22  -v0-2/" target="
+00001e10: 5f62 6c61 6e6b 223e 3c73 6d61 6c6c 3e28  _blank"><small>(
+00001e20: 7265 6629 3c2f 736d 616c 6c3e 3c2f 613e  ref)</small></a>
+00001e30: 3c2f 6469 763e 0a0a 2d2d 2d0a 0a22 5f2a  </div>..---.."_*
+00001e40: 2a4e 6574 666c 6978 2a2a 2069 7320 706c  *Netflix** is pl
+00001e50: 6561 7365 6420 746f 2061 6e6e 6f75 6e63  eased to announc
+00001e60: 6520 7468 6520 6f70 656e 2d73 6f75 7263  e the open-sourc
+00001e70: 6520 7265 6c65 6173 6520 6f66 206f 7572  e release of our
+00001e80: 202a 2a63 7269 7369 7320 6d61 6e61 6765   **crisis manage
+00001e90: 6d65 6e74 2a2a 206f 7263 6865 7374 7261  ment** orchestra
+00001ea0: 7469 6f6e 2066 7261 6d65 776f 726b 3a20  tion framework: 
+00001eb0: 2a2a 4469 7370 6174 6368 2a2a 2120 5b62  **Dispatch**! [b
+00001ec0: 7569 6c74 2077 6974 6820 2a2a 4661 7374  uilt with **Fast
+00001ed0: 4150 492a 2a5d 5f22 0a0a 3c64 6976 2073  API**]_"..<div s
+00001ee0: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
+00001ef0: 3a20 7269 6768 743b 206d 6172 6769 6e2d  : right; margin-
+00001f00: 7269 6768 743a 2031 3025 3b22 3e4b 6576  right: 10%;">Kev
+00001f10: 696e 2047 6c69 7373 6f6e 2c20 4d61 7263  in Glisson, Marc
+00001f20: 2056 696c 616e 6f76 612c 2046 6f72 6573   Vilanova, Fores
+00001f30: 7420 4d6f 6e73 656e 202d 203c 7374 726f  t Monsen - <stro
+00001f40: 6e67 3e4e 6574 666c 6978 3c2f 7374 726f  ng>Netflix</stro
+00001f50: 6e67 3e20 3c61 2068 7265 663d 2268 7474  ng> <a href="htt
+00001f60: 7073 3a2f 2f6e 6574 666c 6978 7465 6368  ps://netflixtech
+00001f70: 626c 6f67 2e63 6f6d 2f69 6e74 726f 6475  blog.com/introdu
+00001f80: 6369 6e67 2d64 6973 7061 7463 682d 6461  cing-dispatch-da
+00001f90: 3462 3861 3261 3830 3732 2220 7461 7267  4b8a2a8072" targ
+00001fa0: 6574 3d22 5f62 6c61 6e6b 223e 3c73 6d61  et="_blank"><sma
+00001fb0: 6c6c 3e28 7265 6629 3c2f 736d 616c 6c3e  ll>(ref)</small>
+00001fc0: 3c2f 613e 3c2f 6469 763e 0a0a 2d2d 2d0a  </a></div>..---.
+00001fd0: 0a22 5f49 e280 996d 206f 7665 7220 7468  ."_I...m over th
+00001fe0: 6520 6d6f 6f6e 2065 7863 6974 6564 2061  e moon excited a
+00001ff0: 626f 7574 202a 2a46 6173 7441 5049 2a2a  bout **FastAPI**
+00002000: 2e20 4974 e280 9973 2073 6f20 6675 6e21  . It...s so fun!
+00002010: 5f22 0a0a 3c64 6976 2073 7479 6c65 3d22  _"..<div style="
+00002020: 7465 7874 2d61 6c69 676e 3a20 7269 6768  text-align: righ
+00002030: 743b 206d 6172 6769 6e2d 7269 6768 743a  t; margin-right:
+00002040: 2031 3025 3b22 3e42 7269 616e 204f 6b6b   10%;">Brian Okk
+00002050: 656e 202d 203c 7374 726f 6e67 3e3c 6120  en - <strong><a 
+00002060: 6872 6566 3d22 6874 7470 733a 2f2f 7079  href="https://py
+00002070: 7468 6f6e 6279 7465 732e 666d 2f65 7069  thonbytes.fm/epi
+00002080: 736f 6465 732f 7368 6f77 2f31 3233 2f74  sodes/show/123/t
+00002090: 696d 652d 746f 2d72 6967 6874 2d74 6865  ime-to-right-the
+000020a0: 2d70 792d 7772 6f6e 6773 3f74 696d 655f  -py-wrongs?time_
+000020b0: 696e 5f73 6563 3d38 3535 2220 7461 7267  in_sec=855" targ
+000020c0: 6574 3d22 5f62 6c61 6e6b 223e 5079 7468  et="_blank">Pyth
+000020d0: 6f6e 2042 7974 6573 3c2f 613e 2070 6f64  on Bytes</a> pod
+000020e0: 6361 7374 2068 6f73 743c 2f73 7472 6f6e  cast host</stron
+000020f0: 673e 203c 6120 6872 6566 3d22 6874 7470  g> <a href="http
+00002100: 733a 2f2f 7477 6974 7465 722e 636f 6d2f  s://twitter.com/
+00002110: 6272 6961 6e6f 6b6b 656e 2f73 7461 7475  brianokken/statu
+00002120: 732f 3131 3132 3232 3030 3739 3937 3237  s/11122200799727
+00002130: 3238 3833 3222 2074 6172 6765 743d 225f  28832" target="_
+00002140: 626c 616e 6b22 3e3c 736d 616c 6c3e 2872  blank"><small>(r
+00002150: 6566 293c 2f73 6d61 6c6c 3e3c 2f61 3e3c  ef)</small></a><
+00002160: 2f64 6976 3e0a 0a2d 2d2d 0a0a 225f 486f  /div>..---.."_Ho
+00002170: 6e65 7374 6c79 2c20 7768 6174 2079 6f75  nestly, what you
+00002180: 2776 6520 6275 696c 7420 6c6f 6f6b 7320  've built looks 
+00002190: 7375 7065 7220 736f 6c69 6420 616e 6420  super solid and 
+000021a0: 706f 6c69 7368 6564 2e20 496e 206d 616e  polished. In man
+000021b0: 7920 7761 7973 2c20 6974 2773 2077 6861  y ways, it's wha
+000021c0: 7420 4920 7761 6e74 6564 202a 2a48 7567  t I wanted **Hug
+000021d0: 2a2a 2074 6f20 6265 202d 2069 7427 7320  ** to be - it's 
+000021e0: 7265 616c 6c79 2069 6e73 7069 7269 6e67  really inspiring
+000021f0: 2074 6f20 7365 6520 736f 6d65 6f6e 6520   to see someone 
+00002200: 6275 696c 6420 7468 6174 2e5f 220a 0a3c  build that._"..<
+00002210: 6469 7620 7374 796c 653d 2274 6578 742d  div style="text-
+00002220: 616c 6967 6e3a 2072 6967 6874 3b20 6d61  align: right; ma
+00002230: 7267 696e 2d72 6967 6874 3a20 3130 253b  rgin-right: 10%;
+00002240: 223e 5469 6d6f 7468 7920 4372 6f73 6c65  ">Timothy Crosle
+00002250: 7920 2d20 3c73 7472 6f6e 673e 3c61 2068  y - <strong><a h
+00002260: 7265 663d 2268 7474 7073 3a2f 2f77 7777  ref="https://www
+00002270: 2e68 7567 2e72 6573 742f 2220 7461 7267  .hug.rest/" targ
+00002280: 6574 3d22 5f62 6c61 6e6b 223e 4875 673c  et="_blank">Hug<
+00002290: 2f61 3e20 6372 6561 746f 723c 2f73 7472  /a> creator</str
+000022a0: 6f6e 673e 203c 6120 6872 6566 3d22 6874  ong> <a href="ht
+000022b0: 7470 733a 2f2f 6e65 7773 2e79 636f 6d62  tps://news.ycomb
+000022c0: 696e 6174 6f72 2e63 6f6d 2f69 7465 6d3f  inator.com/item?
+000022d0: 6964 3d31 3934 3535 3436 3522 2074 6172  id=19455465" tar
+000022e0: 6765 743d 225f 626c 616e 6b22 3e3c 736d  get="_blank"><sm
+000022f0: 616c 6c3e 2872 6566 293c 2f73 6d61 6c6c  all>(ref)</small
+00002300: 3e3c 2f61 3e3c 2f64 6976 3e0a 0a2d 2d2d  ></a></div>..---
+00002310: 0a0a 225f 4966 2079 6f75 2772 6520 6c6f  .."_If you're lo
+00002320: 6f6b 696e 6720 746f 206c 6561 726e 206f  oking to learn o
+00002330: 6e65 202a 2a6d 6f64 6572 6e20 6672 616d  ne **modern fram
+00002340: 6577 6f72 6b2a 2a20 666f 7220 6275 696c  ework** for buil
+00002350: 6469 6e67 2052 4553 5420 4150 4973 2c20  ding REST APIs, 
+00002360: 6368 6563 6b20 6f75 7420 2a2a 4661 7374  check out **Fast
+00002370: 4150 492a 2a20 5b2e 2e2e 5d20 4974 2773  API** [...] It's
+00002380: 2066 6173 742c 2065 6173 7920 746f 2075   fast, easy to u
+00002390: 7365 2061 6e64 2065 6173 7920 746f 206c  se and easy to l
+000023a0: 6561 726e 205b 2e2e 2e5d 5f22 0a0a 225f  earn [...]_".."_
+000023b0: 5765 2776 6520 7377 6974 6368 6564 206f  We've switched o
+000023c0: 7665 7220 746f 202a 2a46 6173 7441 5049  ver to **FastAPI
+000023d0: 2a2a 2066 6f72 206f 7572 202a 2a41 5049  ** for our **API
+000023e0: 732a 2a20 5b2e 2e2e 5d20 4920 7468 696e  s** [...] I thin
+000023f0: 6b20 796f 7527 6c6c 206c 696b 6520 6974  k you'll like it
+00002400: 205b 2e2e 2e5d 5f22 0a0a 3c64 6976 2073   [...]_"..<div s
+00002410: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
+00002420: 3a20 7269 6768 743b 206d 6172 6769 6e2d  : right; margin-
+00002430: 7269 6768 743a 2031 3025 3b22 3e49 6e65  right: 10%;">Ine
+00002440: 7320 4d6f 6e74 616e 6920 2d20 4d61 7474  s Montani - Matt
+00002450: 6865 7720 486f 6e6e 6962 616c 202d 203c  hew Honnibal - <
+00002460: 7374 726f 6e67 3e3c 6120 6872 6566 3d22  strong><a href="
+00002470: 6874 7470 733a 2f2f 6578 706c 6f73 696f  https://explosio
+00002480: 6e2e 6169 2220 7461 7267 6574 3d22 5f62  n.ai" target="_b
+00002490: 6c61 6e6b 223e 4578 706c 6f73 696f 6e20  lank">Explosion 
+000024a0: 4149 3c2f 613e 2066 6f75 6e64 6572 7320  AI</a> founders 
+000024b0: 2d20 3c61 2068 7265 663d 2268 7474 7073  - <a href="https
+000024c0: 3a2f 2f73 7061 6379 2e69 6f22 2074 6172  ://spacy.io" tar
+000024d0: 6765 743d 225f 626c 616e 6b22 3e73 7061  get="_blank">spa
+000024e0: 4379 3c2f 613e 2063 7265 6174 6f72 733c  Cy</a> creators<
+000024f0: 2f73 7472 6f6e 673e 203c 6120 6872 6566  /strong> <a href
+00002500: 3d22 6874 7470 733a 2f2f 7477 6974 7465  ="https://twitte
+00002510: 722e 636f 6d2f 5f69 6e65 736d 6f6e 7461  r.com/_inesmonta
+00002520: 6e69 2f73 7461 7475 732f 3131 3434 3137  ni/status/114417
+00002530: 3332 3235 3332 3231 3433 3734 3422 2074  3225322143744" t
+00002540: 6172 6765 743d 225f 626c 616e 6b22 3e3c  arget="_blank"><
+00002550: 736d 616c 6c3e 2872 6566 293c 2f73 6d61  small>(ref)</sma
+00002560: 6c6c 3e3c 2f61 3e20 2d20 3c61 2068 7265  ll></a> - <a hre
+00002570: 663d 2268 7474 7073 3a2f 2f74 7769 7474  f="https://twitt
+00002580: 6572 2e63 6f6d 2f68 6f6e 6e69 6261 6c2f  er.com/honnibal/
+00002590: 7374 6174 7573 2f31 3134 3430 3331 3432  status/114403142
+000025a0: 3138 3539 3635 3536 3830 2220 7461 7267  1859655680" targ
+000025b0: 6574 3d22 5f62 6c61 6e6b 223e 3c73 6d61  et="_blank"><sma
+000025c0: 6c6c 3e28 7265 6629 3c2f 736d 616c 6c3e  ll>(ref)</small>
+000025d0: 3c2f 613e 3c2f 6469 763e 0a0a 2d2d 2d0a  </a></div>..---.
+000025e0: 0a22 5f49 6620 616e 796f 6e65 2069 7320  ."_If anyone is 
+000025f0: 6c6f 6f6b 696e 6720 746f 2062 7569 6c64  looking to build
+00002600: 2061 2070 726f 6475 6374 696f 6e20 5079   a production Py
+00002610: 7468 6f6e 2041 5049 2c20 4920 776f 756c  thon API, I woul
+00002620: 6420 6869 6768 6c79 2072 6563 6f6d 6d65  d highly recomme
+00002630: 6e64 202a 2a46 6173 7441 5049 2a2a 2e20  nd **FastAPI**. 
+00002640: 4974 2069 7320 2a2a 6265 6175 7469 6675  It is **beautifu
+00002650: 6c6c 7920 6465 7369 676e 6564 2a2a 2c20  lly designed**, 
+00002660: 2a2a 7369 6d70 6c65 2074 6f20 7573 652a  **simple to use*
+00002670: 2a20 616e 6420 2a2a 6869 6768 6c79 2073  * and **highly s
+00002680: 6361 6c61 626c 652a 2a2c 2069 7420 6861  calable**, it ha
+00002690: 7320 6265 636f 6d65 2061 202a 2a6b 6579  s become a **key
+000026a0: 2063 6f6d 706f 6e65 6e74 2a2a 2069 6e20   component** in 
+000026b0: 6f75 7220 4150 4920 6669 7273 7420 6465  our API first de
+000026c0: 7665 6c6f 706d 656e 7420 7374 7261 7465  velopment strate
+000026d0: 6779 2061 6e64 2069 7320 6472 6976 696e  gy and is drivin
+000026e0: 6720 6d61 6e79 2061 7574 6f6d 6174 696f  g many automatio
+000026f0: 6e73 2061 6e64 2073 6572 7669 6365 7320  ns and services 
+00002700: 7375 6368 2061 7320 6f75 7220 5669 7274  such as our Virt
+00002710: 7561 6c20 5441 4320 456e 6769 6e65 6572  ual TAC Engineer
+00002720: 2e5f 220a 0a3c 6469 7620 7374 796c 653d  ._"..<div style=
+00002730: 2274 6578 742d 616c 6967 6e3a 2072 6967  "text-align: rig
+00002740: 6874 3b20 6d61 7267 696e 2d72 6967 6874  ht; margin-right
+00002750: 3a20 3130 253b 223e 4465 6f6e 2050 696c  : 10%;">Deon Pil
+00002760: 6c73 6275 7279 202d 203c 7374 726f 6e67  lsbury - <strong
+00002770: 3e43 6973 636f 3c2f 7374 726f 6e67 3e20  >Cisco</strong> 
+00002780: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00002790: 2f77 7777 2e6c 696e 6b65 6469 6e2e 636f  /www.linkedin.co
+000027a0: 6d2f 706f 7374 732f 6465 6f6e 7069 6c6c  m/posts/deonpill
+000027b0: 7362 7572 795f 6369 7363 6f2d 6378 2d70  sbury_cisco-cx-p
+000027c0: 7974 686f 6e2d 6163 7469 7669 7479 2d36  ython-activity-6
+000027d0: 3936 3332 3432 3632 3835 3336 3438 3739  9632426285364879
+000027e0: 3336 2d74 7241 702f 2220 7461 7267 6574  36-trAp/" target
+000027f0: 3d22 5f62 6c61 6e6b 223e 3c73 6d61 6c6c  ="_blank"><small
+00002800: 3e28 7265 6629 3c2f 736d 616c 6c3e 3c2f  >(ref)</small></
+00002810: 613e 3c2f 6469 763e 0a0a 2d2d 2d0a 0a23  a></div>..---..#
+00002820: 2320 2a2a 5479 7065 722a 2a2c 2074 6865  # **Typer**, the
+00002830: 2046 6173 7441 5049 206f 6620 434c 4973   FastAPI of CLIs
+00002840: 0a0a 3c61 2068 7265 663d 2268 7474 7073  ..<a href="https
+00002850: 3a2f 2f74 7970 6572 2e74 6961 6e67 6f6c  ://typer.tiangol
+00002860: 6f2e 636f 6d22 2074 6172 6765 743d 225f  o.com" target="_
+00002870: 626c 616e 6b22 3e3c 696d 6720 7372 633d  blank"><img src=
+00002880: 2268 7474 7073 3a2f 2f74 7970 6572 2e74  "https://typer.t
+00002890: 6961 6e67 6f6c 6f2e 636f 6d2f 696d 672f  iangolo.com/img/
+000028a0: 6c6f 676f 2d6d 6172 6769 6e2f 6c6f 676f  logo-margin/logo
+000028b0: 2d6d 6172 6769 6e2d 7665 6374 6f72 2e73  -margin-vector.s
+000028c0: 7667 2220 7374 796c 653d 2277 6964 7468  vg" style="width
+000028d0: 3a20 3230 253b 223e 3c2f 613e 0a0a 4966  : 20%;"></a>..If
+000028e0: 2079 6f75 2061 7265 2062 7569 6c64 696e   you are buildin
+000028f0: 6720 6120 3c61 6262 7220 7469 746c 653d  g a <abbr title=
+00002900: 2243 6f6d 6d61 6e64 204c 696e 6520 496e  "Command Line In
+00002910: 7465 7266 6163 6522 3e43 4c49 3c2f 6162  terface">CLI</ab
+00002920: 6272 3e20 6170 7020 746f 2062 6520 7573  br> app to be us
+00002930: 6564 2069 6e20 7468 6520 7465 726d 696e  ed in the termin
+00002940: 616c 2069 6e73 7465 6164 206f 6620 6120  al instead of a 
+00002950: 7765 6220 4150 492c 2063 6865 636b 206f  web API, check o
+00002960: 7574 203c 6120 6872 6566 3d22 6874 7470  ut <a href="http
+00002970: 733a 2f2f 7479 7065 722e 7469 616e 676f  s://typer.tiango
+00002980: 6c6f 2e63 6f6d 2f22 2063 6c61 7373 3d22  lo.com/" class="
+00002990: 6578 7465 726e 616c 2d6c 696e 6b22 2074  external-link" t
+000029a0: 6172 6765 743d 225f 626c 616e 6b22 3e2a  arget="_blank">*
+000029b0: 2a54 7970 6572 2a2a 3c2f 613e 2e0a 0a2a  *Typer**</a>...*
+000029c0: 2a54 7970 6572 2a2a 2069 7320 4661 7374  *Typer** is Fast
+000029d0: 4150 4927 7320 6c69 7474 6c65 2073 6962  API's little sib
+000029e0: 6c69 6e67 2e20 416e 6420 6974 2773 2069  ling. And it's i
+000029f0: 6e74 656e 6465 6420 746f 2062 6520 7468  ntended to be th
+00002a00: 6520 2a2a 4661 7374 4150 4920 6f66 2043  e **FastAPI of C
+00002a10: 4c49 732a 2a2e 20e2 8ca8 efb8 8f20 f09f  LIs**. ...... ..
+00002a20: 9a80 0a0a 2323 2052 6571 7569 7265 6d65  ....## Requireme
+00002a30: 6e74 730a 0a50 7974 686f 6e20 332e 372b  nts..Python 3.7+
+00002a40: 0a0a 4661 7374 4150 4920 7374 616e 6473  ..FastAPI stands
+00002a50: 206f 6e20 7468 6520 7368 6f75 6c64 6572   on the shoulder
+00002a60: 7320 6f66 2067 6961 6e74 733a 0a0a 2a20  s of giants:..* 
+00002a70: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00002a80: 2f77 7777 2e73 7461 726c 6574 7465 2e69  /www.starlette.i
+00002a90: 6f2f 2220 636c 6173 733d 2265 7874 6572  o/" class="exter
+00002aa0: 6e61 6c2d 6c69 6e6b 2220 7461 7267 6574  nal-link" target
+00002ab0: 3d22 5f62 6c61 6e6b 223e 5374 6172 6c65  ="_blank">Starle
+00002ac0: 7474 653c 2f61 3e20 666f 7220 7468 6520  tte</a> for the 
+00002ad0: 7765 6220 7061 7274 732e 0a2a 203c 6120  web parts..* <a 
+00002ae0: 6872 6566 3d22 6874 7470 733a 2f2f 7079  href="https://py
+00002af0: 6461 6e74 6963 2d64 6f63 732e 6865 6c70  dantic-docs.help
+00002b00: 6d61 6e75 616c 2e69 6f2f 2220 636c 6173  manual.io/" clas
+00002b10: 733d 2265 7874 6572 6e61 6c2d 6c69 6e6b  s="external-link
+00002b20: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+00002b30: 223e 5079 6461 6e74 6963 3c2f 613e 2066  ">Pydantic</a> f
+00002b40: 6f72 2074 6865 2064 6174 6120 7061 7274  or the data part
+00002b50: 732e 0a0a 2323 2049 6e73 7461 6c6c 6174  s...## Installat
+00002b60: 696f 6e0a 0a3c 6469 7620 636c 6173 733d  ion..<div class=
+00002b70: 2274 6572 6d79 223e 0a0a 6060 6063 6f6e  "termy">..```con
+00002b80: 736f 6c65 0a24 2070 6970 2069 6e73 7461  sole.$ pip insta
+00002b90: 6c6c 2066 6173 7461 7069 0a0a 2d2d 2d3e  ll fastapi..--->
+00002ba0: 2031 3030 250a 6060 600a 0a3c 2f64 6976   100%.```..</div
+00002bb0: 3e0a 0a59 6f75 2077 696c 6c20 616c 736f  >..You will also
+00002bc0: 206e 6565 6420 616e 2041 5347 4920 7365   need an ASGI se
+00002bd0: 7276 6572 2c20 666f 7220 7072 6f64 7563  rver, for produc
+00002be0: 7469 6f6e 2073 7563 6820 6173 203c 6120  tion such as <a 
+00002bf0: 6872 6566 3d22 6874 7470 733a 2f2f 7777  href="https://ww
+00002c00: 772e 7576 6963 6f72 6e2e 6f72 6722 2063  w.uvicorn.org" c
+00002c10: 6c61 7373 3d22 6578 7465 726e 616c 2d6c  lass="external-l
+00002c20: 696e 6b22 2074 6172 6765 743d 225f 626c  ink" target="_bl
+00002c30: 616e 6b22 3e55 7669 636f 726e 3c2f 613e  ank">Uvicorn</a>
+00002c40: 206f 7220 3c61 2068 7265 663d 2268 7474   or <a href="htt
+00002c50: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00002c60: 7067 6a6f 6e65 732f 6879 7065 7263 6f72  pgjones/hypercor
+00002c70: 6e22 2063 6c61 7373 3d22 6578 7465 726e  n" class="extern
+00002c80: 616c 2d6c 696e 6b22 2074 6172 6765 743d  al-link" target=
+00002c90: 225f 626c 616e 6b22 3e48 7970 6572 636f  "_blank">Hyperco
+00002ca0: 726e 3c2f 613e 2e0a 0a3c 6469 7620 636c  rn</a>...<div cl
+00002cb0: 6173 733d 2274 6572 6d79 223e 0a0a 6060  ass="termy">..``
+00002cc0: 6063 6f6e 736f 6c65 0a24 2070 6970 2069  `console.$ pip i
+00002cd0: 6e73 7461 6c6c 2022 7576 6963 6f72 6e5b  nstall "uvicorn[
+00002ce0: 7374 616e 6461 7264 5d22 0a0a 2d2d 2d3e  standard]"..--->
+00002cf0: 2031 3030 250a 6060 600a 0a3c 2f64 6976   100%.```..</div
+00002d00: 3e0a 0a23 2320 4578 616d 706c 650a 0a23  >..## Example..#
+00002d10: 2323 2043 7265 6174 6520 6974 0a0a 2a20  ## Create it..* 
+00002d20: 4372 6561 7465 2061 2066 696c 6520 606d  Create a file `m
+00002d30: 6169 6e2e 7079 6020 7769 7468 3a0a 0a60  ain.py` with:..`
+00002d40: 6060 5079 7468 6f6e 0a66 726f 6d20 7479  ``Python.from ty
+00002d50: 7069 6e67 2069 6d70 6f72 7420 556e 696f  ping import Unio
+00002d60: 6e0a 0a66 726f 6d20 6661 7374 6170 6920  n..from fastapi 
+00002d70: 696d 706f 7274 2046 6173 7441 5049 0a0a  import FastAPI..
+00002d80: 6170 7020 3d20 4661 7374 4150 4928 290a  app = FastAPI().
+00002d90: 0a0a 4061 7070 2e67 6574 2822 2f22 290a  ..@app.get("/").
+00002da0: 6465 6620 7265 6164 5f72 6f6f 7428 293a  def read_root():
+00002db0: 0a20 2020 2072 6574 7572 6e20 7b22 4865  .    return {"He
+00002dc0: 6c6c 6f22 3a20 2257 6f72 6c64 227d 0a0a  llo": "World"}..
+00002dd0: 0a40 6170 702e 6765 7428 222f 6974 656d  .@app.get("/item
+00002de0: 732f 7b69 7465 6d5f 6964 7d22 290a 6465  s/{item_id}").de
+00002df0: 6620 7265 6164 5f69 7465 6d28 6974 656d  f read_item(item
+00002e00: 5f69 643a 2069 6e74 2c20 713a 2055 6e69  _id: int, q: Uni
+00002e10: 6f6e 5b73 7472 2c20 4e6f 6e65 5d20 3d20  on[str, None] = 
+00002e20: 4e6f 6e65 293a 0a20 2020 2072 6574 7572  None):.    retur
+00002e30: 6e20 7b22 6974 656d 5f69 6422 3a20 6974  n {"item_id": it
+00002e40: 656d 5f69 642c 2022 7122 3a20 717d 0a60  em_id, "q": q}.`
+00002e50: 6060 0a0a 3c64 6574 6169 6c73 206d 6172  ``..<details mar
+00002e60: 6b64 6f77 6e3d 2231 223e 0a3c 7375 6d6d  kdown="1">.<summ
+00002e70: 6172 793e 4f72 2075 7365 203c 636f 6465  ary>Or use <code
+00002e80: 3e61 7379 6e63 2064 6566 3c2f 636f 6465  >async def</code
+00002e90: 3e2e 2e2e 3c2f 7375 6d6d 6172 793e 0a0a  >...</summary>..
+00002ea0: 4966 2079 6f75 7220 636f 6465 2075 7365  If your code use
+00002eb0: 7320 6061 7379 6e63 6020 2f20 6061 7761  s `async` / `awa
+00002ec0: 6974 602c 2075 7365 2060 6173 796e 6320  it`, use `async 
+00002ed0: 6465 6660 3a0a 0a60 6060 5079 7468 6f6e  def`:..```Python
+00002ee0: 2068 6c5f 6c69 6e65 733d 2239 2020 3134   hl_lines="9  14
+00002ef0: 220a 6672 6f6d 2074 7970 696e 6720 696d  ".from typing im
+00002f00: 706f 7274 2055 6e69 6f6e 0a0a 6672 6f6d  port Union..from
+00002f10: 2066 6173 7461 7069 2069 6d70 6f72 7420   fastapi import 
+00002f20: 4661 7374 4150 490a 0a61 7070 203d 2046  FastAPI..app = F
+00002f30: 6173 7441 5049 2829 0a0a 0a40 6170 702e  astAPI()...@app.
+00002f40: 6765 7428 222f 2229 0a61 7379 6e63 2064  get("/").async d
+00002f50: 6566 2072 6561 645f 726f 6f74 2829 3a0a  ef read_root():.
+00002f60: 2020 2020 7265 7475 726e 207b 2248 656c      return {"Hel
+00002f70: 6c6f 223a 2022 576f 726c 6422 7d0a 0a0a  lo": "World"}...
+00002f80: 4061 7070 2e67 6574 2822 2f69 7465 6d73  @app.get("/items
+00002f90: 2f7b 6974 656d 5f69 647d 2229 0a61 7379  /{item_id}").asy
+00002fa0: 6e63 2064 6566 2072 6561 645f 6974 656d  nc def read_item
+00002fb0: 2869 7465 6d5f 6964 3a20 696e 742c 2071  (item_id: int, q
+00002fc0: 3a20 556e 696f 6e5b 7374 722c 204e 6f6e  : Union[str, Non
+00002fd0: 655d 203d 204e 6f6e 6529 3a0a 2020 2020  e] = None):.    
+00002fe0: 7265 7475 726e 207b 2269 7465 6d5f 6964  return {"item_id
+00002ff0: 223a 2069 7465 6d5f 6964 2c20 2271 223a  ": item_id, "q":
+00003000: 2071 7d0a 6060 600a 0a2a 2a4e 6f74 652a   q}.```..**Note*
+00003010: 2a3a 0a0a 4966 2079 6f75 2064 6f6e 2774  *:..If you don't
+00003020: 206b 6e6f 772c 2063 6865 636b 2074 6865   know, check the
+00003030: 205f 2249 6e20 6120 6875 7272 793f 225f   _"In a hurry?"_
+00003040: 2073 6563 7469 6f6e 2061 626f 7574 203c   section about <
+00003050: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00003060: 6661 7374 6170 692e 7469 616e 676f 6c6f  fastapi.tiangolo
+00003070: 2e63 6f6d 2f61 7379 6e63 2f23 696e 2d61  .com/async/#in-a
+00003080: 2d68 7572 7279 2220 7461 7267 6574 3d22  -hurry" target="
+00003090: 5f62 6c61 6e6b 223e 6061 7379 6e63 6020  _blank">`async` 
+000030a0: 616e 6420 6061 7761 6974 6020 696e 2074  and `await` in t
+000030b0: 6865 2064 6f63 733c 2f61 3e2e 0a0a 3c2f  he docs</a>...</
+000030c0: 6465 7461 696c 733e 0a0a 2323 2320 5275  details>..### Ru
+000030d0: 6e20 6974 0a0a 5275 6e20 7468 6520 7365  n it..Run the se
+000030e0: 7276 6572 2077 6974 683a 0a0a 3c64 6976  rver with:..<div
+000030f0: 2063 6c61 7373 3d22 7465 726d 7922 3e0a   class="termy">.
+00003100: 0a60 6060 636f 6e73 6f6c 650a 2420 7576  .```console.$ uv
+00003110: 6963 6f72 6e20 6d61 696e 3a61 7070 202d  icorn main:app -
+00003120: 2d72 656c 6f61 640a 0a49 4e46 4f3a 2020  -reload..INFO:  
+00003130: 2020 2055 7669 636f 726e 2072 756e 6e69     Uvicorn runni
+00003140: 6e67 206f 6e20 6874 7470 3a2f 2f31 3237  ng on http://127
+00003150: 2e30 2e30 2e31 3a38 3030 3020 2850 7265  .0.0.1:8000 (Pre
+00003160: 7373 2043 5452 4c2b 4320 746f 2071 7569  ss CTRL+C to qui
+00003170: 7429 0a49 4e46 4f3a 2020 2020 2053 7461  t).INFO:     Sta
+00003180: 7274 6564 2072 656c 6f61 6465 7220 7072  rted reloader pr
+00003190: 6f63 6573 7320 5b32 3837 3230 5d0a 494e  ocess [28720].IN
+000031a0: 464f 3a20 2020 2020 5374 6172 7465 6420  FO:     Started 
+000031b0: 7365 7276 6572 2070 726f 6365 7373 205b  server process [
+000031c0: 3238 3732 325d 0a49 4e46 4f3a 2020 2020  28722].INFO:    
+000031d0: 2057 6169 7469 6e67 2066 6f72 2061 7070   Waiting for app
+000031e0: 6c69 6361 7469 6f6e 2073 7461 7274 7570  lication startup
+000031f0: 2e0a 494e 464f 3a20 2020 2020 4170 706c  ..INFO:     Appl
+00003200: 6963 6174 696f 6e20 7374 6172 7475 7020  ication startup 
+00003210: 636f 6d70 6c65 7465 2e0a 6060 600a 0a3c  complete..```..<
+00003220: 2f64 6976 3e0a 0a3c 6465 7461 696c 7320  /div>..<details 
+00003230: 6d61 726b 646f 776e 3d22 3122 3e0a 3c73  markdown="1">.<s
+00003240: 756d 6d61 7279 3e41 626f 7574 2074 6865  ummary>About the
+00003250: 2063 6f6d 6d61 6e64 203c 636f 6465 3e75   command <code>u
+00003260: 7669 636f 726e 206d 6169 6e3a 6170 7020  vicorn main:app 
+00003270: 2d2d 7265 6c6f 6164 3c2f 636f 6465 3e2e  --reload</code>.
+00003280: 2e2e 3c2f 7375 6d6d 6172 793e 0a0a 5468  ..</summary>..Th
+00003290: 6520 636f 6d6d 616e 6420 6075 7669 636f  e command `uvico
+000032a0: 726e 206d 6169 6e3a 6170 7060 2072 6566  rn main:app` ref
+000032b0: 6572 7320 746f 3a0a 0a2a 2060 6d61 696e  ers to:..* `main
+000032c0: 603a 2074 6865 2066 696c 6520 606d 6169  `: the file `mai
+000032d0: 6e2e 7079 6020 2874 6865 2050 7974 686f  n.py` (the Pytho
+000032e0: 6e20 226d 6f64 756c 6522 292e 0a2a 2060  n "module")..* `
+000032f0: 6170 7060 3a20 7468 6520 6f62 6a65 6374  app`: the object
+00003300: 2063 7265 6174 6564 2069 6e73 6964 6520   created inside 
+00003310: 6f66 2060 6d61 696e 2e70 7960 2077 6974  of `main.py` wit
+00003320: 6820 7468 6520 6c69 6e65 2060 6170 7020  h the line `app 
+00003330: 3d20 4661 7374 4150 4928 2960 2e0a 2a20  = FastAPI()`..* 
+00003340: 602d 2d72 656c 6f61 6460 3a20 6d61 6b65  `--reload`: make
+00003350: 2074 6865 2073 6572 7665 7220 7265 7374   the server rest
+00003360: 6172 7420 6166 7465 7220 636f 6465 2063  art after code c
+00003370: 6861 6e67 6573 2e20 4f6e 6c79 2064 6f20  hanges. Only do 
+00003380: 7468 6973 2066 6f72 2064 6576 656c 6f70  this for develop
+00003390: 6d65 6e74 2e0a 0a3c 2f64 6574 6169 6c73  ment...</details
+000033a0: 3e0a 0a23 2323 2043 6865 636b 2069 740a  >..### Check it.
+000033b0: 0a4f 7065 6e20 796f 7572 2062 726f 7773  .Open your brows
+000033c0: 6572 2061 7420 3c61 2068 7265 663d 2268  er at <a href="h
+000033d0: 7474 703a 2f2f 3132 372e 302e 302e 313a  ttp://127.0.0.1:
+000033e0: 3830 3030 2f69 7465 6d73 2f35 3f71 3d73  8000/items/5?q=s
+000033f0: 6f6d 6571 7565 7279 2220 636c 6173 733d  omequery" class=
+00003400: 2265 7874 6572 6e61 6c2d 6c69 6e6b 2220  "external-link" 
+00003410: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
+00003420: 6874 7470 3a2f 2f31 3237 2e30 2e30 2e31  http://127.0.0.1
+00003430: 3a38 3030 302f 6974 656d 732f 353f 713d  :8000/items/5?q=
+00003440: 736f 6d65 7175 6572 793c 2f61 3e2e 0a0a  somequery</a>...
+00003450: 596f 7520 7769 6c6c 2073 6565 2074 6865  You will see the
+00003460: 204a 534f 4e20 7265 7370 6f6e 7365 2061   JSON response a
+00003470: 733a 0a0a 6060 604a 534f 4e0a 7b22 6974  s:..```JSON.{"it
+00003480: 656d 5f69 6422 3a20 352c 2022 7122 3a20  em_id": 5, "q": 
+00003490: 2273 6f6d 6571 7565 7279 227d 0a60 6060  "somequery"}.```
+000034a0: 0a0a 596f 7520 616c 7265 6164 7920 6372  ..You already cr
+000034b0: 6561 7465 6420 616e 2041 5049 2074 6861  eated an API tha
+000034c0: 743a 0a0a 2a20 5265 6365 6976 6573 2048  t:..* Receives H
+000034d0: 5454 5020 7265 7175 6573 7473 2069 6e20  TTP requests in 
+000034e0: 7468 6520 5f70 6174 6873 5f20 602f 6020  the _paths_ `/` 
+000034f0: 616e 6420 602f 6974 656d 732f 7b69 7465  and `/items/{ite
+00003500: 6d5f 6964 7d60 2e0a 2a20 426f 7468 205f  m_id}`..* Both _
+00003510: 7061 7468 735f 2074 616b 6520 6047 4554  paths_ take `GET
+00003520: 6020 3c65 6d3e 6f70 6572 6174 696f 6e73  ` <em>operations
+00003530: 3c2f 656d 3e20 2861 6c73 6f20 6b6e 6f77  </em> (also know
+00003540: 6e20 6173 2048 5454 5020 5f6d 6574 686f  n as HTTP _metho
+00003550: 6473 5f29 2e0a 2a20 5468 6520 5f70 6174  ds_)..* The _pat
+00003560: 685f 2060 2f69 7465 6d73 2f7b 6974 656d  h_ `/items/{item
+00003570: 5f69 647d 6020 6861 7320 6120 5f70 6174  _id}` has a _pat
+00003580: 6820 7061 7261 6d65 7465 725f 2060 6974  h parameter_ `it
+00003590: 656d 5f69 6460 2074 6861 7420 7368 6f75  em_id` that shou
+000035a0: 6c64 2062 6520 616e 2060 696e 7460 2e0a  ld be an `int`..
+000035b0: 2a20 5468 6520 5f70 6174 685f 2060 2f69  * The _path_ `/i
+000035c0: 7465 6d73 2f7b 6974 656d 5f69 647d 6020  tems/{item_id}` 
+000035d0: 6861 7320 616e 206f 7074 696f 6e61 6c20  has an optional 
+000035e0: 6073 7472 6020 5f71 7565 7279 2070 6172  `str` _query par
+000035f0: 616d 6574 6572 5f20 6071 602e 0a0a 2323  ameter_ `q`...##
+00003600: 2320 496e 7465 7261 6374 6976 6520 4150  # Interactive AP
+00003610: 4920 646f 6373 0a0a 4e6f 7720 676f 2074  I docs..Now go t
+00003620: 6f20 3c61 2068 7265 663d 2268 7474 703a  o <a href="http:
+00003630: 2f2f 3132 372e 302e 302e 313a 3830 3030  //127.0.0.1:8000
+00003640: 2f64 6f63 7322 2063 6c61 7373 3d22 6578  /docs" class="ex
+00003650: 7465 726e 616c 2d6c 696e 6b22 2074 6172  ternal-link" tar
+00003660: 6765 743d 225f 626c 616e 6b22 3e68 7474  get="_blank">htt
+00003670: 703a 2f2f 3132 372e 302e 302e 313a 3830  p://127.0.0.1:80
+00003680: 3030 2f64 6f63 733c 2f61 3e2e 0a0a 596f  00/docs</a>...Yo
+00003690: 7520 7769 6c6c 2073 6565 2074 6865 2061  u will see the a
+000036a0: 7574 6f6d 6174 6963 2069 6e74 6572 6163  utomatic interac
+000036b0: 7469 7665 2041 5049 2064 6f63 756d 656e  tive API documen
+000036c0: 7461 7469 6f6e 2028 7072 6f76 6964 6564  tation (provided
+000036d0: 2062 7920 3c61 2068 7265 663d 2268 7474   by <a href="htt
+000036e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000036f0: 7377 6167 6765 722d 6170 692f 7377 6167  swagger-api/swag
+00003700: 6765 722d 7569 2220 636c 6173 733d 2265  ger-ui" class="e
+00003710: 7874 6572 6e61 6c2d 6c69 6e6b 2220 7461  xternal-link" ta
+00003720: 7267 6574 3d22 5f62 6c61 6e6b 223e 5377  rget="_blank">Sw
+00003730: 6167 6765 7220 5549 3c2f 613e 293a 0a0a  agger UI</a>):..
+00003740: 215b 5377 6167 6765 7220 5549 5d28 6874  ![Swagger UI](ht
+00003750: 7470 733a 2f2f 6661 7374 6170 692e 7469  tps://fastapi.ti
+00003760: 616e 676f 6c6f 2e63 6f6d 2f69 6d67 2f69  angolo.com/img/i
+00003770: 6e64 6578 2f69 6e64 6578 2d30 312d 7377  ndex/index-01-sw
+00003780: 6167 6765 722d 7569 2d73 696d 706c 652e  agger-ui-simple.
+00003790: 706e 6729 0a0a 2323 2320 416c 7465 726e  png)..### Altern
+000037a0: 6174 6976 6520 4150 4920 646f 6373 0a0a  ative API docs..
+000037b0: 416e 6420 6e6f 772c 2067 6f20 746f 203c  And now, go to <
+000037c0: 6120 6872 6566 3d22 6874 7470 3a2f 2f31  a href="http://1
+000037d0: 3237 2e30 2e30 2e31 3a38 3030 302f 7265  27.0.0.1:8000/re
+000037e0: 646f 6322 2063 6c61 7373 3d22 6578 7465  doc" class="exte
+000037f0: 726e 616c 2d6c 696e 6b22 2074 6172 6765  rnal-link" targe
+00003800: 743d 225f 626c 616e 6b22 3e68 7474 703a  t="_blank">http:
+00003810: 2f2f 3132 372e 302e 302e 313a 3830 3030  //127.0.0.1:8000
+00003820: 2f72 6564 6f63 3c2f 613e 2e0a 0a59 6f75  /redoc</a>...You
+00003830: 2077 696c 6c20 7365 6520 7468 6520 616c   will see the al
+00003840: 7465 726e 6174 6976 6520 6175 746f 6d61  ternative automa
+00003850: 7469 6320 646f 6375 6d65 6e74 6174 696f  tic documentatio
+00003860: 6e20 2870 726f 7669 6465 6420 6279 203c  n (provided by <
+00003870: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00003880: 6769 7468 7562 2e63 6f6d 2f52 6562 696c  github.com/Rebil
+00003890: 6c79 2f52 6544 6f63 2220 636c 6173 733d  ly/ReDoc" class=
+000038a0: 2265 7874 6572 6e61 6c2d 6c69 6e6b 2220  "external-link" 
+000038b0: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
+000038c0: 5265 446f 633c 2f61 3e29 3a0a 0a21 5b52  ReDoc</a>):..![R
+000038d0: 6544 6f63 5d28 6874 7470 733a 2f2f 6661  eDoc](https://fa
+000038e0: 7374 6170 692e 7469 616e 676f 6c6f 2e63  stapi.tiangolo.c
+000038f0: 6f6d 2f69 6d67 2f69 6e64 6578 2f69 6e64  om/img/index/ind
+00003900: 6578 2d30 322d 7265 646f 632d 7369 6d70  ex-02-redoc-simp
+00003910: 6c65 2e70 6e67 290a 0a23 2320 4578 616d  le.png)..## Exam
+00003920: 706c 6520 7570 6772 6164 650a 0a4e 6f77  ple upgrade..Now
+00003930: 206d 6f64 6966 7920 7468 6520 6669 6c65   modify the file
+00003940: 2060 6d61 696e 2e70 7960 2074 6f20 7265   `main.py` to re
+00003950: 6365 6976 6520 6120 626f 6479 2066 726f  ceive a body fro
+00003960: 6d20 6120 6050 5554 6020 7265 7175 6573  m a `PUT` reques
+00003970: 742e 0a0a 4465 636c 6172 6520 7468 6520  t...Declare the 
+00003980: 626f 6479 2075 7369 6e67 2073 7461 6e64  body using stand
+00003990: 6172 6420 5079 7468 6f6e 2074 7970 6573  ard Python types
+000039a0: 2c20 7468 616e 6b73 2074 6f20 5079 6461  , thanks to Pyda
+000039b0: 6e74 6963 2e0a 0a60 6060 5079 7468 6f6e  ntic...```Python
+000039c0: 2068 6c5f 6c69 6e65 733d 2234 2020 392d   hl_lines="4  9-
+000039d0: 3132 2020 3235 2d32 3722 0a66 726f 6d20  12  25-27".from 
+000039e0: 7479 7069 6e67 2069 6d70 6f72 7420 556e  typing import Un
+000039f0: 696f 6e0a 0a66 726f 6d20 6661 7374 6170  ion..from fastap
+00003a00: 6920 696d 706f 7274 2046 6173 7441 5049  i import FastAPI
+00003a10: 0a66 726f 6d20 7079 6461 6e74 6963 2069  .from pydantic i
+00003a20: 6d70 6f72 7420 4261 7365 4d6f 6465 6c0a  mport BaseModel.
+00003a30: 0a61 7070 203d 2046 6173 7441 5049 2829  .app = FastAPI()
+00003a40: 0a0a 0a63 6c61 7373 2049 7465 6d28 4261  ...class Item(Ba
+00003a50: 7365 4d6f 6465 6c29 3a0a 2020 2020 6e61  seModel):.    na
+00003a60: 6d65 3a20 7374 720a 2020 2020 7072 6963  me: str.    pric
+00003a70: 653a 2066 6c6f 6174 0a20 2020 2069 735f  e: float.    is_
+00003a80: 6f66 6665 723a 2055 6e69 6f6e 5b62 6f6f  offer: Union[boo
+00003a90: 6c2c 204e 6f6e 655d 203d 204e 6f6e 650a  l, None] = None.
+00003aa0: 0a0a 4061 7070 2e67 6574 2822 2f22 290a  ..@app.get("/").
+00003ab0: 6465 6620 7265 6164 5f72 6f6f 7428 293a  def read_root():
+00003ac0: 0a20 2020 2072 6574 7572 6e20 7b22 4865  .    return {"He
+00003ad0: 6c6c 6f22 3a20 2257 6f72 6c64 227d 0a0a  llo": "World"}..
+00003ae0: 0a40 6170 702e 6765 7428 222f 6974 656d  .@app.get("/item
+00003af0: 732f 7b69 7465 6d5f 6964 7d22 290a 6465  s/{item_id}").de
+00003b00: 6620 7265 6164 5f69 7465 6d28 6974 656d  f read_item(item
+00003b10: 5f69 643a 2069 6e74 2c20 713a 2055 6e69  _id: int, q: Uni
+00003b20: 6f6e 5b73 7472 2c20 4e6f 6e65 5d20 3d20  on[str, None] = 
+00003b30: 4e6f 6e65 293a 0a20 2020 2072 6574 7572  None):.    retur
+00003b40: 6e20 7b22 6974 656d 5f69 6422 3a20 6974  n {"item_id": it
+00003b50: 656d 5f69 642c 2022 7122 3a20 717d 0a0a  em_id, "q": q}..
+00003b60: 0a40 6170 702e 7075 7428 222f 6974 656d  .@app.put("/item
+00003b70: 732f 7b69 7465 6d5f 6964 7d22 290a 6465  s/{item_id}").de
+00003b80: 6620 7570 6461 7465 5f69 7465 6d28 6974  f update_item(it
+00003b90: 656d 5f69 643a 2069 6e74 2c20 6974 656d  em_id: int, item
+00003ba0: 3a20 4974 656d 293a 0a20 2020 2072 6574  : Item):.    ret
+00003bb0: 7572 6e20 7b22 6974 656d 5f6e 616d 6522  urn {"item_name"
+00003bc0: 3a20 6974 656d 2e6e 616d 652c 2022 6974  : item.name, "it
+00003bd0: 656d 5f69 6422 3a20 6974 656d 5f69 647d  em_id": item_id}
+00003be0: 0a60 6060 0a0a 5468 6520 7365 7276 6572  .```..The server
+00003bf0: 2073 686f 756c 6420 7265 6c6f 6164 2061   should reload a
+00003c00: 7574 6f6d 6174 6963 616c 6c79 2028 6265  utomatically (be
+00003c10: 6361 7573 6520 796f 7520 6164 6465 6420  cause you added 
+00003c20: 602d 2d72 656c 6f61 6460 2074 6f20 7468  `--reload` to th
+00003c30: 6520 6075 7669 636f 726e 6020 636f 6d6d  e `uvicorn` comm
+00003c40: 616e 6420 6162 6f76 6529 2e0a 0a23 2323  and above)...###
+00003c50: 2049 6e74 6572 6163 7469 7665 2041 5049   Interactive API
+00003c60: 2064 6f63 7320 7570 6772 6164 650a 0a4e   docs upgrade..N
+00003c70: 6f77 2067 6f20 746f 203c 6120 6872 6566  ow go to <a href
+00003c80: 3d22 6874 7470 3a2f 2f31 3237 2e30 2e30  ="http://127.0.0
+00003c90: 2e31 3a38 3030 302f 646f 6373 2220 636c  .1:8000/docs" cl
+00003ca0: 6173 733d 2265 7874 6572 6e61 6c2d 6c69  ass="external-li
+00003cb0: 6e6b 2220 7461 7267 6574 3d22 5f62 6c61  nk" target="_bla
+00003cc0: 6e6b 223e 6874 7470 3a2f 2f31 3237 2e30  nk">http://127.0
+00003cd0: 2e30 2e31 3a38 3030 302f 646f 6373 3c2f  .0.1:8000/docs</
+00003ce0: 613e 2e0a 0a2a 2054 6865 2069 6e74 6572  a>...* The inter
+00003cf0: 6163 7469 7665 2041 5049 2064 6f63 756d  active API docum
+00003d00: 656e 7461 7469 6f6e 2077 696c 6c20 6265  entation will be
+00003d10: 2061 7574 6f6d 6174 6963 616c 6c79 2075   automatically u
+00003d20: 7064 6174 6564 2c20 696e 636c 7564 696e  pdated, includin
+00003d30: 6720 7468 6520 6e65 7720 626f 6479 3a0a  g the new body:.
+00003d40: 0a21 5b53 7761 6767 6572 2055 495d 2868  .![Swagger UI](h
+00003d50: 7474 7073 3a2f 2f66 6173 7461 7069 2e74  ttps://fastapi.t
+00003d60: 6961 6e67 6f6c 6f2e 636f 6d2f 696d 672f  iangolo.com/img/
+00003d70: 696e 6465 782f 696e 6465 782d 3033 2d73  index/index-03-s
+00003d80: 7761 6767 6572 2d30 322e 706e 6729 0a0a  wagger-02.png)..
+00003d90: 2a20 436c 6963 6b20 6f6e 2074 6865 2062  * Click on the b
+00003da0: 7574 746f 6e20 2254 7279 2069 7420 6f75  utton "Try it ou
+00003db0: 7422 2c20 6974 2061 6c6c 6f77 7320 796f  t", it allows yo
+00003dc0: 7520 746f 2066 696c 6c20 7468 6520 7061  u to fill the pa
+00003dd0: 7261 6d65 7465 7273 2061 6e64 2064 6972  rameters and dir
+00003de0: 6563 746c 7920 696e 7465 7261 6374 2077  ectly interact w
+00003df0: 6974 6820 7468 6520 4150 493a 0a0a 215b  ith the API:..![
+00003e00: 5377 6167 6765 7220 5549 2069 6e74 6572  Swagger UI inter
+00003e10: 6163 7469 6f6e 5d28 6874 7470 733a 2f2f  action](https://
+00003e20: 6661 7374 6170 692e 7469 616e 676f 6c6f  fastapi.tiangolo
+00003e30: 2e63 6f6d 2f69 6d67 2f69 6e64 6578 2f69  .com/img/index/i
+00003e40: 6e64 6578 2d30 342d 7377 6167 6765 722d  ndex-04-swagger-
+00003e50: 3033 2e70 6e67 290a 0a2a 2054 6865 6e20  03.png)..* Then 
+00003e60: 636c 6963 6b20 6f6e 2074 6865 2022 4578  click on the "Ex
+00003e70: 6563 7574 6522 2062 7574 746f 6e2c 2074  ecute" button, t
+00003e80: 6865 2075 7365 7220 696e 7465 7266 6163  he user interfac
+00003e90: 6520 7769 6c6c 2063 6f6d 6d75 6e69 6361  e will communica
+00003ea0: 7465 2077 6974 6820 796f 7572 2041 5049  te with your API
+00003eb0: 2c20 7365 6e64 2074 6865 2070 6172 616d  , send the param
+00003ec0: 6574 6572 732c 2067 6574 2074 6865 2072  eters, get the r
+00003ed0: 6573 756c 7473 2061 6e64 2073 686f 7720  esults and show 
+00003ee0: 7468 656d 206f 6e20 7468 6520 7363 7265  them on the scre
+00003ef0: 656e 3a0a 0a21 5b53 7761 6767 6572 2055  en:..![Swagger U
+00003f00: 4920 696e 7465 7261 6374 696f 6e5d 2868  I interaction](h
+00003f10: 7474 7073 3a2f 2f66 6173 7461 7069 2e74  ttps://fastapi.t
+00003f20: 6961 6e67 6f6c 6f2e 636f 6d2f 696d 672f  iangolo.com/img/
+00003f30: 696e 6465 782f 696e 6465 782d 3035 2d73  index/index-05-s
+00003f40: 7761 6767 6572 2d30 342e 706e 6729 0a0a  wagger-04.png)..
+00003f50: 2323 2320 416c 7465 726e 6174 6976 6520  ### Alternative 
+00003f60: 4150 4920 646f 6373 2075 7067 7261 6465  API docs upgrade
+00003f70: 0a0a 416e 6420 6e6f 772c 2067 6f20 746f  ..And now, go to
+00003f80: 203c 6120 6872 6566 3d22 6874 7470 3a2f   <a href="http:/
+00003f90: 2f31 3237 2e30 2e30 2e31 3a38 3030 302f  /127.0.0.1:8000/
+00003fa0: 7265 646f 6322 2063 6c61 7373 3d22 6578  redoc" class="ex
+00003fb0: 7465 726e 616c 2d6c 696e 6b22 2074 6172  ternal-link" tar
+00003fc0: 6765 743d 225f 626c 616e 6b22 3e68 7474  get="_blank">htt
+00003fd0: 703a 2f2f 3132 372e 302e 302e 313a 3830  p://127.0.0.1:80
+00003fe0: 3030 2f72 6564 6f63 3c2f 613e 2e0a 0a2a  00/redoc</a>...*
+00003ff0: 2054 6865 2061 6c74 6572 6e61 7469 7665   The alternative
+00004000: 2064 6f63 756d 656e 7461 7469 6f6e 2077   documentation w
+00004010: 696c 6c20 616c 736f 2072 6566 6c65 6374  ill also reflect
+00004020: 2074 6865 206e 6577 2071 7565 7279 2070   the new query p
+00004030: 6172 616d 6574 6572 2061 6e64 2062 6f64  arameter and bod
+00004040: 793a 0a0a 215b 5265 446f 635d 2868 7474  y:..![ReDoc](htt
+00004050: 7073 3a2f 2f66 6173 7461 7069 2e74 6961  ps://fastapi.tia
+00004060: 6e67 6f6c 6f2e 636f 6d2f 696d 672f 696e  ngolo.com/img/in
+00004070: 6465 782f 696e 6465 782d 3036 2d72 6564  dex/index-06-red
+00004080: 6f63 2d30 322e 706e 6729 0a0a 2323 2320  oc-02.png)..### 
+00004090: 5265 6361 700a 0a49 6e20 7375 6d6d 6172  Recap..In summar
+000040a0: 792c 2079 6f75 2064 6563 6c61 7265 202a  y, you declare *
+000040b0: 2a6f 6e63 652a 2a20 7468 6520 7479 7065  *once** the type
+000040c0: 7320 6f66 2070 6172 616d 6574 6572 732c  s of parameters,
+000040d0: 2062 6f64 792c 2065 7463 2e20 6173 2066   body, etc. as f
+000040e0: 756e 6374 696f 6e20 7061 7261 6d65 7465  unction paramete
+000040f0: 7273 2e0a 0a59 6f75 2064 6f20 7468 6174  rs...You do that
+00004100: 2077 6974 6820 7374 616e 6461 7264 206d   with standard m
+00004110: 6f64 6572 6e20 5079 7468 6f6e 2074 7970  odern Python typ
+00004120: 6573 2e0a 0a59 6f75 2064 6f6e 2774 2068  es...You don't h
+00004130: 6176 6520 746f 206c 6561 726e 2061 206e  ave to learn a n
+00004140: 6577 2073 796e 7461 782c 2074 6865 206d  ew syntax, the m
+00004150: 6574 686f 6473 206f 7220 636c 6173 7365  ethods or classe
+00004160: 7320 6f66 2061 2073 7065 6369 6669 6320  s of a specific 
+00004170: 6c69 6272 6172 792c 2065 7463 2e0a 0a4a  library, etc...J
+00004180: 7573 7420 7374 616e 6461 7264 202a 2a50  ust standard **P
+00004190: 7974 686f 6e20 332e 372b 2a2a 2e0a 0a46  ython 3.7+**...F
+000041a0: 6f72 2065 7861 6d70 6c65 2c20 666f 7220  or example, for 
+000041b0: 616e 2060 696e 7460 3a0a 0a60 6060 5079  an `int`:..```Py
+000041c0: 7468 6f6e 0a69 7465 6d5f 6964 3a20 696e  thon.item_id: in
+000041d0: 740a 6060 600a 0a6f 7220 666f 7220 6120  t.```..or for a 
+000041e0: 6d6f 7265 2063 6f6d 706c 6578 2060 4974  more complex `It
+000041f0: 656d 6020 6d6f 6465 6c3a 0a0a 6060 6050  em` model:..```P
+00004200: 7974 686f 6e0a 6974 656d 3a20 4974 656d  ython.item: Item
+00004210: 0a60 6060 0a0a 2e2e 2e61 6e64 2077 6974  .```.....and wit
+00004220: 6820 7468 6174 2073 696e 676c 6520 6465  h that single de
+00004230: 636c 6172 6174 696f 6e20 796f 7520 6765  claration you ge
+00004240: 743a 0a0a 2a20 4564 6974 6f72 2073 7570  t:..* Editor sup
+00004250: 706f 7274 2c20 696e 636c 7564 696e 673a  port, including:
+00004260: 0a20 2020 202a 2043 6f6d 706c 6574 696f  .    * Completio
+00004270: 6e2e 0a20 2020 202a 2054 7970 6520 6368  n..    * Type ch
+00004280: 6563 6b73 2e0a 2a20 5661 6c69 6461 7469  ecks..* Validati
+00004290: 6f6e 206f 6620 6461 7461 3a0a 2020 2020  on of data:.    
+000042a0: 2a20 4175 746f 6d61 7469 6320 616e 6420  * Automatic and 
+000042b0: 636c 6561 7220 6572 726f 7273 2077 6865  clear errors whe
+000042c0: 6e20 7468 6520 6461 7461 2069 7320 696e  n the data is in
+000042d0: 7661 6c69 642e 0a20 2020 202a 2056 616c  valid..    * Val
+000042e0: 6964 6174 696f 6e20 6576 656e 2066 6f72  idation even for
+000042f0: 2064 6565 706c 7920 6e65 7374 6564 204a   deeply nested J
+00004300: 534f 4e20 6f62 6a65 6374 732e 0a2a 203c  SON objects..* <
+00004310: 6162 6272 2074 6974 6c65 3d22 616c 736f  abbr title="also
+00004320: 206b 6e6f 776e 2061 733a 2073 6572 6961   known as: seria
+00004330: 6c69 7a61 7469 6f6e 2c20 7061 7273 696e  lization, parsin
+00004340: 672c 206d 6172 7368 616c 6c69 6e67 223e  g, marshalling">
+00004350: 436f 6e76 6572 7369 6f6e 3c2f 6162 6272  Conversion</abbr
+00004360: 3e20 6f66 2069 6e70 7574 2064 6174 613a  > of input data:
+00004370: 2063 6f6d 696e 6720 6672 6f6d 2074 6865   coming from the
+00004380: 206e 6574 776f 726b 2074 6f20 5079 7468   network to Pyth
+00004390: 6f6e 2064 6174 6120 616e 6420 7479 7065  on data and type
+000043a0: 732e 2052 6561 6469 6e67 2066 726f 6d3a  s. Reading from:
+000043b0: 0a20 2020 202a 204a 534f 4e2e 0a20 2020  .    * JSON..   
+000043c0: 202a 2050 6174 6820 7061 7261 6d65 7465   * Path paramete
+000043d0: 7273 2e0a 2020 2020 2a20 5175 6572 7920  rs..    * Query 
+000043e0: 7061 7261 6d65 7465 7273 2e0a 2020 2020  parameters..    
+000043f0: 2a20 436f 6f6b 6965 732e 0a20 2020 202a  * Cookies..    *
+00004400: 2048 6561 6465 7273 2e0a 2020 2020 2a20   Headers..    * 
+00004410: 466f 726d 732e 0a20 2020 202a 2046 696c  Forms..    * Fil
+00004420: 6573 2e0a 2a20 3c61 6262 7220 7469 746c  es..* <abbr titl
+00004430: 653d 2261 6c73 6f20 6b6e 6f77 6e20 6173  e="also known as
+00004440: 3a20 7365 7269 616c 697a 6174 696f 6e2c  : serialization,
+00004450: 2070 6172 7369 6e67 2c20 6d61 7273 6861   parsing, marsha
+00004460: 6c6c 696e 6722 3e43 6f6e 7665 7273 696f  lling">Conversio
+00004470: 6e3c 2f61 6262 723e 206f 6620 6f75 7470  n</abbr> of outp
+00004480: 7574 2064 6174 613a 2063 6f6e 7665 7274  ut data: convert
+00004490: 696e 6720 6672 6f6d 2050 7974 686f 6e20  ing from Python 
+000044a0: 6461 7461 2061 6e64 2074 7970 6573 2074  data and types t
+000044b0: 6f20 6e65 7477 6f72 6b20 6461 7461 2028  o network data (
+000044c0: 6173 204a 534f 4e29 3a0a 2020 2020 2a20  as JSON):.    * 
+000044d0: 436f 6e76 6572 7420 5079 7468 6f6e 2074  Convert Python t
+000044e0: 7970 6573 2028 6073 7472 602c 2060 696e  ypes (`str`, `in
+000044f0: 7460 2c20 6066 6c6f 6174 602c 2060 626f  t`, `float`, `bo
+00004500: 6f6c 602c 2060 6c69 7374 602c 2065 7463  ol`, `list`, etc
+00004510: 292e 0a20 2020 202a 2060 6461 7465 7469  )..    * `dateti
+00004520: 6d65 6020 6f62 6a65 6374 732e 0a20 2020  me` objects..   
+00004530: 202a 2060 5555 4944 6020 6f62 6a65 6374   * `UUID` object
+00004540: 732e 0a20 2020 202a 2044 6174 6162 6173  s..    * Databas
+00004550: 6520 6d6f 6465 6c73 2e0a 2020 2020 2a20  e models..    * 
+00004560: 2e2e 2e61 6e64 206d 616e 7920 6d6f 7265  ...and many more
+00004570: 2e0a 2a20 4175 746f 6d61 7469 6320 696e  ..* Automatic in
+00004580: 7465 7261 6374 6976 6520 4150 4920 646f  teractive API do
+00004590: 6375 6d65 6e74 6174 696f 6e2c 2069 6e63  cumentation, inc
+000045a0: 6c75 6469 6e67 2032 2061 6c74 6572 6e61  luding 2 alterna
+000045b0: 7469 7665 2075 7365 7220 696e 7465 7266  tive user interf
+000045c0: 6163 6573 3a0a 2020 2020 2a20 5377 6167  aces:.    * Swag
+000045d0: 6765 7220 5549 2e0a 2020 2020 2a20 5265  ger UI..    * Re
+000045e0: 446f 632e 0a0a 2d2d 2d0a 0a43 6f6d 696e  Doc...---..Comin
+000045f0: 6720 6261 636b 2074 6f20 7468 6520 7072  g back to the pr
+00004600: 6576 696f 7573 2063 6f64 6520 6578 616d  evious code exam
+00004610: 706c 652c 202a 2a46 6173 7441 5049 2a2a  ple, **FastAPI**
+00004620: 2077 696c 6c3a 0a0a 2a20 5661 6c69 6461   will:..* Valida
+00004630: 7465 2074 6861 7420 7468 6572 6520 6973  te that there is
+00004640: 2061 6e20 6069 7465 6d5f 6964 6020 696e   an `item_id` in
+00004650: 2074 6865 2070 6174 6820 666f 7220 6047   the path for `G
+00004660: 4554 6020 616e 6420 6050 5554 6020 7265  ET` and `PUT` re
+00004670: 7175 6573 7473 2e0a 2a20 5661 6c69 6461  quests..* Valida
+00004680: 7465 2074 6861 7420 7468 6520 6069 7465  te that the `ite
+00004690: 6d5f 6964 6020 6973 206f 6620 7479 7065  m_id` is of type
+000046a0: 2060 696e 7460 2066 6f72 2060 4745 5460   `int` for `GET`
+000046b0: 2061 6e64 2060 5055 5460 2072 6571 7565   and `PUT` reque
+000046c0: 7374 732e 0a20 2020 202a 2049 6620 6974  sts..    * If it
+000046d0: 2069 7320 6e6f 742c 2074 6865 2063 6c69   is not, the cli
+000046e0: 656e 7420 7769 6c6c 2073 6565 2061 2075  ent will see a u
+000046f0: 7365 6675 6c2c 2063 6c65 6172 2065 7272  seful, clear err
+00004700: 6f72 2e0a 2a20 4368 6563 6b20 6966 2074  or..* Check if t
+00004710: 6865 7265 2069 7320 616e 206f 7074 696f  here is an optio
+00004720: 6e61 6c20 7175 6572 7920 7061 7261 6d65  nal query parame
+00004730: 7465 7220 6e61 6d65 6420 6071 6020 2861  ter named `q` (a
+00004740: 7320 696e 2060 6874 7470 3a2f 2f31 3237  s in `http://127
+00004750: 2e30 2e30 2e31 3a38 3030 302f 6974 656d  .0.0.1:8000/item
+00004760: 732f 666f 6f3f 713d 736f 6d65 7175 6572  s/foo?q=somequer
+00004770: 7960 2920 666f 7220 6047 4554 6020 7265  y`) for `GET` re
+00004780: 7175 6573 7473 2e0a 2020 2020 2a20 4173  quests..    * As
+00004790: 2074 6865 2060 7160 2070 6172 616d 6574   the `q` paramet
+000047a0: 6572 2069 7320 6465 636c 6172 6564 2077  er is declared w
+000047b0: 6974 6820 603d 204e 6f6e 6560 2c20 6974  ith `= None`, it
+000047c0: 2069 7320 6f70 7469 6f6e 616c 2e0a 2020   is optional..  
+000047d0: 2020 2a20 5769 7468 6f75 7420 7468 6520    * Without the 
+000047e0: 604e 6f6e 6560 2069 7420 776f 756c 6420  `None` it would 
+000047f0: 6265 2072 6571 7569 7265 6420 2861 7320  be required (as 
+00004800: 6973 2074 6865 2062 6f64 7920 696e 2074  is the body in t
+00004810: 6865 2063 6173 6520 7769 7468 2060 5055  he case with `PU
+00004820: 5460 292e 0a2a 2046 6f72 2060 5055 5460  T`)..* For `PUT`
+00004830: 2072 6571 7565 7374 7320 746f 2060 2f69   requests to `/i
+00004840: 7465 6d73 2f7b 6974 656d 5f69 647d 602c  tems/{item_id}`,
+00004850: 2052 6561 6420 7468 6520 626f 6479 2061   Read the body a
+00004860: 7320 4a53 4f4e 3a0a 2020 2020 2a20 4368  s JSON:.    * Ch
+00004870: 6563 6b20 7468 6174 2069 7420 6861 7320  eck that it has 
+00004880: 6120 7265 7175 6972 6564 2061 7474 7269  a required attri
+00004890: 6275 7465 2060 6e61 6d65 6020 7468 6174  bute `name` that
+000048a0: 2073 686f 756c 6420 6265 2061 2060 7374   should be a `st
+000048b0: 7260 2e0a 2020 2020 2a20 4368 6563 6b20  r`..    * Check 
+000048c0: 7468 6174 2069 7420 6861 7320 6120 7265  that it has a re
+000048d0: 7175 6972 6564 2061 7474 7269 6275 7465  quired attribute
+000048e0: 2060 7072 6963 6560 2074 6861 7420 6861   `price` that ha
+000048f0: 7320 746f 2062 6520 6120 6066 6c6f 6174  s to be a `float
+00004900: 602e 0a20 2020 202a 2043 6865 636b 2074  `..    * Check t
+00004910: 6861 7420 6974 2068 6173 2061 6e20 6f70  hat it has an op
+00004920: 7469 6f6e 616c 2061 7474 7269 6275 7465  tional attribute
+00004930: 2060 6973 5f6f 6666 6572 602c 2074 6861   `is_offer`, tha
+00004940: 7420 7368 6f75 6c64 2062 6520 6120 6062  t should be a `b
+00004950: 6f6f 6c60 2c20 6966 2070 7265 7365 6e74  ool`, if present
+00004960: 2e0a 2020 2020 2a20 416c 6c20 7468 6973  ..    * All this
+00004970: 2077 6f75 6c64 2061 6c73 6f20 776f 726b   would also work
+00004980: 2066 6f72 2064 6565 706c 7920 6e65 7374   for deeply nest
+00004990: 6564 204a 534f 4e20 6f62 6a65 6374 732e  ed JSON objects.
+000049a0: 0a2a 2043 6f6e 7665 7274 2066 726f 6d20  .* Convert from 
+000049b0: 616e 6420 746f 204a 534f 4e20 6175 746f  and to JSON auto
+000049c0: 6d61 7469 6361 6c6c 792e 0a2a 2044 6f63  matically..* Doc
+000049d0: 756d 656e 7420 6576 6572 7974 6869 6e67  ument everything
+000049e0: 2077 6974 6820 4f70 656e 4150 492c 2074   with OpenAPI, t
+000049f0: 6861 7420 6361 6e20 6265 2075 7365 6420  hat can be used 
+00004a00: 6279 3a0a 2020 2020 2a20 496e 7465 7261  by:.    * Intera
+00004a10: 6374 6976 6520 646f 6375 6d65 6e74 6174  ctive documentat
+00004a20: 696f 6e20 7379 7374 656d 732e 0a20 2020  ion systems..   
+00004a30: 202a 2041 7574 6f6d 6174 6963 2063 6c69   * Automatic cli
+00004a40: 656e 7420 636f 6465 2067 656e 6572 6174  ent code generat
+00004a50: 696f 6e20 7379 7374 656d 732c 2066 6f72  ion systems, for
+00004a60: 206d 616e 7920 6c61 6e67 7561 6765 732e   many languages.
+00004a70: 0a2a 2050 726f 7669 6465 2032 2069 6e74  .* Provide 2 int
+00004a80: 6572 6163 7469 7665 2064 6f63 756d 656e  eractive documen
+00004a90: 7461 7469 6f6e 2077 6562 2069 6e74 6572  tation web inter
+00004aa0: 6661 6365 7320 6469 7265 6374 6c79 2e0a  faces directly..
+00004ab0: 0a2d 2d2d 0a0a 5765 206a 7573 7420 7363  .---..We just sc
+00004ac0: 7261 7463 6865 6420 7468 6520 7375 7266  ratched the surf
+00004ad0: 6163 652c 2062 7574 2079 6f75 2061 6c72  ace, but you alr
+00004ae0: 6561 6479 2067 6574 2074 6865 2069 6465  eady get the ide
+00004af0: 6120 6f66 2068 6f77 2069 7420 616c 6c20  a of how it all 
+00004b00: 776f 726b 732e 0a0a 5472 7920 6368 616e  works...Try chan
+00004b10: 6769 6e67 2074 6865 206c 696e 6520 7769  ging the line wi
+00004b20: 7468 3a0a 0a60 6060 5079 7468 6f6e 0a20  th:..```Python. 
+00004b30: 2020 2072 6574 7572 6e20 7b22 6974 656d     return {"item
+00004b40: 5f6e 616d 6522 3a20 6974 656d 2e6e 616d  _name": item.nam
+00004b50: 652c 2022 6974 656d 5f69 6422 3a20 6974  e, "item_id": it
+00004b60: 656d 5f69 647d 0a60 6060 0a0a 2e2e 2e66  em_id}.```.....f
+00004b70: 726f 6d3a 0a0a 6060 6050 7974 686f 6e0a  rom:..```Python.
+00004b80: 2020 2020 2020 2020 2e2e 2e20 2269 7465          ... "ite
+00004b90: 6d5f 6e61 6d65 223a 2069 7465 6d2e 6e61  m_name": item.na
+00004ba0: 6d65 202e 2e2e 0a60 6060 0a0a 2e2e 2e74  me ....```.....t
+00004bb0: 6f3a 0a0a 6060 6050 7974 686f 6e0a 2020  o:..```Python.  
+00004bc0: 2020 2020 2020 2e2e 2e20 2269 7465 6d5f        ... "item_
+00004bd0: 7072 6963 6522 3a20 6974 656d 2e70 7269  price": item.pri
+00004be0: 6365 202e 2e2e 0a60 6060 0a0a 2e2e 2e61  ce ....```.....a
+00004bf0: 6e64 2073 6565 2068 6f77 2079 6f75 7220  nd see how your 
+00004c00: 6564 6974 6f72 2077 696c 6c20 6175 746f  editor will auto
+00004c10: 2d63 6f6d 706c 6574 6520 7468 6520 6174  -complete the at
+00004c20: 7472 6962 7574 6573 2061 6e64 206b 6e6f  tributes and kno
+00004c30: 7720 7468 6569 7220 7479 7065 733a 0a0a  w their types:..
+00004c40: 215b 6564 6974 6f72 2073 7570 706f 7274  ![editor support
+00004c50: 5d28 6874 7470 733a 2f2f 6661 7374 6170  ](https://fastap
+00004c60: 692e 7469 616e 676f 6c6f 2e63 6f6d 2f69  i.tiangolo.com/i
+00004c70: 6d67 2f76 7363 6f64 652d 636f 6d70 6c65  mg/vscode-comple
+00004c80: 7469 6f6e 2e70 6e67 290a 0a46 6f72 2061  tion.png)..For a
+00004c90: 206d 6f72 6520 636f 6d70 6c65 7465 2065   more complete e
+00004ca0: 7861 6d70 6c65 2069 6e63 6c75 6469 6e67  xample including
+00004cb0: 206d 6f72 6520 6665 6174 7572 6573 2c20   more features, 
+00004cc0: 7365 6520 7468 6520 3c61 2068 7265 663d  see the <a href=
+00004cd0: 2268 7474 7073 3a2f 2f66 6173 7461 7069  "https://fastapi
+00004ce0: 2e74 6961 6e67 6f6c 6f2e 636f 6d2f 7475  .tiangolo.com/tu
+00004cf0: 746f 7269 616c 2f22 3e54 7574 6f72 6961  torial/">Tutoria
+00004d00: 6c20 2d20 5573 6572 2047 7569 6465 3c2f  l - User Guide</
+00004d10: 613e 2e0a 0a2a 2a53 706f 696c 6572 2061  a>...**Spoiler a
+00004d20: 6c65 7274 2a2a 3a20 7468 6520 7475 746f  lert**: the tuto
+00004d30: 7269 616c 202d 2075 7365 7220 6775 6964  rial - user guid
+00004d40: 6520 696e 636c 7564 6573 3a0a 0a2a 2044  e includes:..* D
+00004d50: 6563 6c61 7261 7469 6f6e 206f 6620 2a2a  eclaration of **
+00004d60: 7061 7261 6d65 7465 7273 2a2a 2066 726f  parameters** fro
+00004d70: 6d20 6f74 6865 7220 6469 6666 6572 656e  m other differen
+00004d80: 7420 706c 6163 6573 2061 733a 202a 2a68  t places as: **h
+00004d90: 6561 6465 7273 2a2a 2c20 2a2a 636f 6f6b  eaders**, **cook
+00004da0: 6965 732a 2a2c 202a 2a66 6f72 6d20 6669  ies**, **form fi
+00004db0: 656c 6473 2a2a 2061 6e64 202a 2a66 696c  elds** and **fil
+00004dc0: 6573 2a2a 2e0a 2a20 486f 7720 746f 2073  es**..* How to s
+00004dd0: 6574 202a 2a76 616c 6964 6174 696f 6e20  et **validation 
+00004de0: 636f 6e73 7472 6169 6e74 732a 2a20 6173  constraints** as
+00004df0: 2060 6d61 7869 6d75 6d5f 6c65 6e67 7468   `maximum_length
+00004e00: 6020 6f72 2060 7265 6765 7860 2e0a 2a20  ` or `regex`..* 
+00004e10: 4120 7665 7279 2070 6f77 6572 6675 6c20  A very powerful 
+00004e20: 616e 6420 6561 7379 2074 6f20 7573 6520  and easy to use 
+00004e30: 2a2a 3c61 6262 7220 7469 746c 653d 2261  **<abbr title="a
+00004e40: 6c73 6f20 6b6e 6f77 6e20 6173 2063 6f6d  lso known as com
+00004e50: 706f 6e65 6e74 732c 2072 6573 6f75 7263  ponents, resourc
+00004e60: 6573 2c20 7072 6f76 6964 6572 732c 2073  es, providers, s
+00004e70: 6572 7669 6365 732c 2069 6e6a 6563 7461  ervices, injecta
+00004e80: 626c 6573 223e 4465 7065 6e64 656e 6379  bles">Dependency
+00004e90: 2049 6e6a 6563 7469 6f6e 3c2f 6162 6272   Injection</abbr
+00004ea0: 3e2a 2a20 7379 7374 656d 2e0a 2a20 5365  >** system..* Se
+00004eb0: 6375 7269 7479 2061 6e64 2061 7574 6865  curity and authe
+00004ec0: 6e74 6963 6174 696f 6e2c 2069 6e63 6c75  ntication, inclu
+00004ed0: 6469 6e67 2073 7570 706f 7274 2066 6f72  ding support for
+00004ee0: 202a 2a4f 4175 7468 322a 2a20 7769 7468   **OAuth2** with
+00004ef0: 202a 2a4a 5754 2074 6f6b 656e 732a 2a20   **JWT tokens** 
+00004f00: 616e 6420 2a2a 4854 5450 2042 6173 6963  and **HTTP Basic
+00004f10: 2a2a 2061 7574 682e 0a2a 204d 6f72 6520  ** auth..* More 
+00004f20: 6164 7661 6e63 6564 2028 6275 7420 6571  advanced (but eq
+00004f30: 7561 6c6c 7920 6561 7379 2920 7465 6368  ually easy) tech
+00004f40: 6e69 7175 6573 2066 6f72 2064 6563 6c61  niques for decla
+00004f50: 7269 6e67 202a 2a64 6565 706c 7920 6e65  ring **deeply ne
+00004f60: 7374 6564 204a 534f 4e20 6d6f 6465 6c73  sted JSON models
+00004f70: 2a2a 2028 7468 616e 6b73 2074 6f20 5079  ** (thanks to Py
+00004f80: 6461 6e74 6963 292e 0a2a 202a 2a47 7261  dantic)..* **Gra
+00004f90: 7068 514c 2a2a 2069 6e74 6567 7261 7469  phQL** integrati
+00004fa0: 6f6e 2077 6974 6820 3c61 2068 7265 663d  on with <a href=
+00004fb0: 2268 7474 7073 3a2f 2f73 7472 6177 6265  "https://strawbe
+00004fc0: 7272 792e 726f 636b 7322 2063 6c61 7373  rry.rocks" class
+00004fd0: 3d22 6578 7465 726e 616c 2d6c 696e 6b22  ="external-link"
+00004fe0: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+00004ff0: 3e53 7472 6177 6265 7272 793c 2f61 3e20  >Strawberry</a> 
+00005000: 616e 6420 6f74 6865 7220 6c69 6272 6172  and other librar
+00005010: 6965 732e 0a2a 204d 616e 7920 6578 7472  ies..* Many extr
+00005020: 6120 6665 6174 7572 6573 2028 7468 616e  a features (than
+00005030: 6b73 2074 6f20 5374 6172 6c65 7474 6529  ks to Starlette)
+00005040: 2061 733a 0a20 2020 202a 202a 2a57 6562   as:.    * **Web
+00005050: 536f 636b 6574 732a 2a0a 2020 2020 2a20  Sockets**.    * 
+00005060: 6578 7472 656d 656c 7920 6561 7379 2074  extremely easy t
+00005070: 6573 7473 2062 6173 6564 206f 6e20 4854  ests based on HT
+00005080: 5450 5820 616e 6420 6070 7974 6573 7460  TPX and `pytest`
+00005090: 0a20 2020 202a 202a 2a43 4f52 532a 2a0a  .    * **CORS**.
+000050a0: 2020 2020 2a20 2a2a 436f 6f6b 6965 2053      * **Cookie S
+000050b0: 6573 7369 6f6e 732a 2a0a 2020 2020 2a20  essions**.    * 
+000050c0: 2e2e 2e61 6e64 206d 6f72 652e 0a0a 2323  ...and more...##
+000050d0: 2050 6572 666f 726d 616e 6365 0a0a 496e   Performance..In
+000050e0: 6465 7065 6e64 656e 7420 5465 6368 456d  dependent TechEm
+000050f0: 706f 7765 7220 6265 6e63 686d 6172 6b73  power benchmarks
+00005100: 2073 686f 7720 2a2a 4661 7374 4150 492a   show **FastAPI*
+00005110: 2a20 6170 706c 6963 6174 696f 6e73 2072  * applications r
+00005120: 756e 6e69 6e67 2075 6e64 6572 2055 7669  unning under Uvi
+00005130: 636f 726e 2061 7320 3c61 2068 7265 663d  corn as <a href=
+00005140: 2268 7474 7073 3a2f 2f77 7777 2e74 6563  "https://www.tec
+00005150: 6865 6d70 6f77 6572 2e63 6f6d 2f62 656e  hempower.com/ben
+00005160: 6368 6d61 726b 732f 2373 6563 7469 6f6e  chmarks/#section
+00005170: 3d74 6573 7426 7275 6e69 643d 3734 3634  =test&runid=7464
+00005180: 6535 3230 2d30 6463 322d 3437 3364 2d62  e520-0dc2-473d-b
+00005190: 6433 342d 6462 6466 6437 6538 3539 3131  d34-dbdfd7e85911
+000051a0: 2668 773d 7068 2674 6573 743d 7175 6572  &hw=ph&test=quer
+000051b0: 7926 6c3d 7a69 6a7a 656e 2d37 2220 636c  y&l=zijzen-7" cl
+000051c0: 6173 733d 2265 7874 6572 6e61 6c2d 6c69  ass="external-li
+000051d0: 6e6b 2220 7461 7267 6574 3d22 5f62 6c61  nk" target="_bla
+000051e0: 6e6b 223e 6f6e 6520 6f66 2074 6865 2066  nk">one of the f
+000051f0: 6173 7465 7374 2050 7974 686f 6e20 6672  astest Python fr
+00005200: 616d 6577 6f72 6b73 2061 7661 696c 6162  ameworks availab
+00005210: 6c65 3c2f 613e 2c20 6f6e 6c79 2062 656c  le</a>, only bel
+00005220: 6f77 2053 7461 726c 6574 7465 2061 6e64  ow Starlette and
+00005230: 2055 7669 636f 726e 2074 6865 6d73 656c   Uvicorn themsel
+00005240: 7665 7320 2875 7365 6420 696e 7465 726e  ves (used intern
+00005250: 616c 6c79 2062 7920 4661 7374 4150 4929  ally by FastAPI)
+00005260: 2e20 282a 290a 0a54 6f20 756e 6465 7273  . (*)..To unders
+00005270: 7461 6e64 206d 6f72 6520 6162 6f75 7420  tand more about 
+00005280: 6974 2c20 7365 6520 7468 6520 7365 6374  it, see the sect
+00005290: 696f 6e20 3c61 2068 7265 663d 2268 7474  ion <a href="htt
+000052a0: 7073 3a2f 2f66 6173 7461 7069 2e74 6961  ps://fastapi.tia
+000052b0: 6e67 6f6c 6f2e 636f 6d2f 6265 6e63 686d  ngolo.com/benchm
+000052c0: 6172 6b73 2f22 2063 6c61 7373 3d22 696e  arks/" class="in
+000052d0: 7465 726e 616c 2d6c 696e 6b22 2074 6172  ternal-link" tar
+000052e0: 6765 743d 225f 626c 616e 6b22 3e42 656e  get="_blank">Ben
+000052f0: 6368 6d61 726b 733c 2f61 3e2e 0a0a 2323  chmarks</a>...##
+00005300: 204f 7074 696f 6e61 6c20 4465 7065 6e64   Optional Depend
+00005310: 656e 6369 6573 0a0a 5573 6564 2062 7920  encies..Used by 
+00005320: 5079 6461 6e74 6963 3a0a 0a2a 203c 6120  Pydantic:..* <a 
+00005330: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+00005340: 7468 7562 2e63 6f6d 2f65 736e 6d65 2f75  thub.com/esnme/u
+00005350: 6c74 7261 6a73 6f6e 2220 7461 7267 6574  ltrajson" target
+00005360: 3d22 5f62 6c61 6e6b 223e 3c63 6f64 653e  ="_blank"><code>
+00005370: 756a 736f 6e3c 2f63 6f64 653e 3c2f 613e  ujson</code></a>
+00005380: 202d 2066 6f72 2066 6173 7465 7220 4a53   - for faster JS
+00005390: 4f4e 203c 6162 6272 2074 6974 6c65 3d22  ON <abbr title="
+000053a0: 636f 6e76 6572 7469 6e67 2074 6865 2073  converting the s
+000053b0: 7472 696e 6720 7468 6174 2063 6f6d 6573  tring that comes
+000053c0: 2066 726f 6d20 616e 2048 5454 5020 7265   from an HTTP re
+000053d0: 7175 6573 7420 696e 746f 2050 7974 686f  quest into Pytho
+000053e0: 6e20 6461 7461 223e 2270 6172 7369 6e67  n data">"parsing
+000053f0: 223c 2f61 6262 723e 2e0a 2a20 3c61 2068  "</abbr>..* <a h
+00005400: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+00005410: 6875 622e 636f 6d2f 4a6f 7368 4461 7461  hub.com/JoshData
+00005420: 2f70 7974 686f 6e2d 656d 6169 6c2d 7661  /python-email-va
+00005430: 6c69 6461 746f 7222 2074 6172 6765 743d  lidator" target=
+00005440: 225f 626c 616e 6b22 3e3c 636f 6465 3e65  "_blank"><code>e
+00005450: 6d61 696c 5f76 616c 6964 6174 6f72 3c2f  mail_validator</
+00005460: 636f 6465 3e3c 2f61 3e20 2d20 666f 7220  code></a> - for 
+00005470: 656d 6169 6c20 7661 6c69 6461 7469 6f6e  email validation
+00005480: 2e0a 0a55 7365 6420 6279 2053 7461 726c  ...Used by Starl
+00005490: 6574 7465 3a0a 0a2a 203c 6120 6872 6566  ette:..* <a href
+000054a0: 3d22 6874 7470 733a 2f2f 7777 772e 7079  ="https://www.py
+000054b0: 7468 6f6e 2d68 7474 7078 2e6f 7267 2220  thon-httpx.org" 
+000054c0: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
+000054d0: 3c63 6f64 653e 6874 7470 783c 2f63 6f64  <code>httpx</cod
+000054e0: 653e 3c2f 613e 202d 2052 6571 7569 7265  e></a> - Require
+000054f0: 6420 6966 2079 6f75 2077 616e 7420 746f  d if you want to
+00005500: 2075 7365 2074 6865 2060 5465 7374 436c   use the `TestCl
+00005510: 6965 6e74 602e 0a2a 203c 6120 6872 6566  ient`..* <a href
+00005520: 3d22 6874 7470 733a 2f2f 6a69 6e6a 612e  ="https://jinja.
+00005530: 7061 6c6c 6574 7370 726f 6a65 6374 732e  palletsprojects.
+00005540: 636f 6d22 2074 6172 6765 743d 225f 626c  com" target="_bl
+00005550: 616e 6b22 3e3c 636f 6465 3e6a 696e 6a61  ank"><code>jinja
+00005560: 323c 2f63 6f64 653e 3c2f 613e 202d 2052  2</code></a> - R
+00005570: 6571 7569 7265 6420 6966 2079 6f75 2077  equired if you w
+00005580: 616e 7420 746f 2075 7365 2074 6865 2064  ant to use the d
+00005590: 6566 6175 6c74 2074 656d 706c 6174 6520  efault template 
+000055a0: 636f 6e66 6967 7572 6174 696f 6e2e 0a2a  configuration..*
+000055b0: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+000055c0: 2f2f 616e 6472 6577 2d64 2e67 6974 6875  //andrew-d.githu
+000055d0: 622e 696f 2f70 7974 686f 6e2d 6d75 6c74  b.io/python-mult
+000055e0: 6970 6172 742f 2220 7461 7267 6574 3d22  ipart/" target="
+000055f0: 5f62 6c61 6e6b 223e 3c63 6f64 653e 7079  _blank"><code>py
+00005600: 7468 6f6e 2d6d 756c 7469 7061 7274 3c2f  thon-multipart</
+00005610: 636f 6465 3e3c 2f61 3e20 2d20 5265 7175  code></a> - Requ
+00005620: 6972 6564 2069 6620 796f 7520 7761 6e74  ired if you want
+00005630: 2074 6f20 7375 7070 6f72 7420 666f 726d   to support form
+00005640: 203c 6162 6272 2074 6974 6c65 3d22 636f   <abbr title="co
+00005650: 6e76 6572 7469 6e67 2074 6865 2073 7472  nverting the str
+00005660: 696e 6720 7468 6174 2063 6f6d 6573 2066  ing that comes f
+00005670: 726f 6d20 616e 2048 5454 5020 7265 7175  rom an HTTP requ
+00005680: 6573 7420 696e 746f 2050 7974 686f 6e20  est into Python 
+00005690: 6461 7461 223e 2270 6172 7369 6e67 223c  data">"parsing"<
+000056a0: 2f61 6262 723e 2c20 7769 7468 2060 7265  /abbr>, with `re
+000056b0: 7175 6573 742e 666f 726d 2829 602e 0a2a  quest.form()`..*
+000056c0: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+000056d0: 2f2f 7079 7468 6f6e 686f 7374 6564 2e6f  //pythonhosted.o
+000056e0: 7267 2f69 7473 6461 6e67 6572 6f75 732f  rg/itsdangerous/
+000056f0: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+00005700: 223e 3c63 6f64 653e 6974 7364 616e 6765  "><code>itsdange
+00005710: 726f 7573 3c2f 636f 6465 3e3c 2f61 3e20  rous</code></a> 
+00005720: 2d20 5265 7175 6972 6564 2066 6f72 2060  - Required for `
+00005730: 5365 7373 696f 6e4d 6964 646c 6577 6172  SessionMiddlewar
+00005740: 6560 2073 7570 706f 7274 2e0a 2a20 3c61  e` support..* <a
+00005750: 2068 7265 663d 2268 7474 7073 3a2f 2f70   href="https://p
+00005760: 7979 616d 6c2e 6f72 672f 7769 6b69 2f50  yyaml.org/wiki/P
+00005770: 7959 414d 4c44 6f63 756d 656e 7461 7469  yYAMLDocumentati
+00005780: 6f6e 2220 7461 7267 6574 3d22 5f62 6c61  on" target="_bla
+00005790: 6e6b 223e 3c63 6f64 653e 7079 7961 6d6c  nk"><code>pyyaml
+000057a0: 3c2f 636f 6465 3e3c 2f61 3e20 2d20 5265  </code></a> - Re
+000057b0: 7175 6972 6564 2066 6f72 2053 7461 726c  quired for Starl
+000057c0: 6574 7465 2773 2060 5363 6865 6d61 4765  ette's `SchemaGe
+000057d0: 6e65 7261 746f 7260 2073 7570 706f 7274  nerator` support
+000057e0: 2028 796f 7520 7072 6f62 6162 6c79 2064   (you probably d
+000057f0: 6f6e 2774 206e 6565 6420 6974 2077 6974  on't need it wit
+00005800: 6820 4661 7374 4150 4929 2e0a 2a20 3c61  h FastAPI)..* <a
+00005810: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+00005820: 6974 6875 622e 636f 6d2f 6573 6e6d 652f  ithub.com/esnme/
+00005830: 756c 7472 616a 736f 6e22 2074 6172 6765  ultrajson" targe
+00005840: 743d 225f 626c 616e 6b22 3e3c 636f 6465  t="_blank"><code
+00005850: 3e75 6a73 6f6e 3c2f 636f 6465 3e3c 2f61  >ujson</code></a
+00005860: 3e20 2d20 5265 7175 6972 6564 2069 6620  > - Required if 
+00005870: 796f 7520 7761 6e74 2074 6f20 7573 6520  you want to use 
+00005880: 6055 4a53 4f4e 5265 7370 6f6e 7365 602e  `UJSONResponse`.
+00005890: 0a0a 5573 6564 2062 7920 4661 7374 4150  ..Used by FastAP
+000058a0: 4920 2f20 5374 6172 6c65 7474 653a 0a0a  I / Starlette:..
+000058b0: 2a20 3c61 2068 7265 663d 2268 7474 7073  * <a href="https
+000058c0: 3a2f 2f77 7777 2e75 7669 636f 726e 2e6f  ://www.uvicorn.o
+000058d0: 7267 2220 7461 7267 6574 3d22 5f62 6c61  rg" target="_bla
+000058e0: 6e6b 223e 3c63 6f64 653e 7576 6963 6f72  nk"><code>uvicor
+000058f0: 6e3c 2f63 6f64 653e 3c2f 613e 202d 2066  n</code></a> - f
+00005900: 6f72 2074 6865 2073 6572 7665 7220 7468  or the server th
+00005910: 6174 206c 6f61 6473 2061 6e64 2073 6572  at loads and ser
+00005920: 7665 7320 796f 7572 2061 7070 6c69 6361  ves your applica
+00005930: 7469 6f6e 2e0a 2a20 3c61 2068 7265 663d  tion..* <a href=
+00005940: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00005950: 636f 6d2f 696a 6c2f 6f72 6a73 6f6e 2220  com/ijl/orjson" 
+00005960: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
+00005970: 3c63 6f64 653e 6f72 6a73 6f6e 3c2f 636f  <code>orjson</co
+00005980: 6465 3e3c 2f61 3e20 2d20 5265 7175 6972  de></a> - Requir
+00005990: 6564 2069 6620 796f 7520 7761 6e74 2074  ed if you want t
+000059a0: 6f20 7573 6520 604f 524a 534f 4e52 6573  o use `ORJSONRes
+000059b0: 706f 6e73 6560 2e0a 0a59 6f75 2063 616e  ponse`...You can
+000059c0: 2069 6e73 7461 6c6c 2061 6c6c 206f 6620   install all of 
+000059d0: 7468 6573 6520 7769 7468 2060 7069 7020  these with `pip 
+000059e0: 696e 7374 616c 6c20 2266 6173 7461 7069  install "fastapi
+000059f0: 5b61 6c6c 5d22 602e 0a0a 2323 204c 6963  [all]"`...## Lic
+00005a00: 656e 7365 0a0a 5468 6973 2070 726f 6a65  ense..This proje
+00005a10: 6374 2069 7320 6c69 6365 6e73 6564 2075  ct is licensed u
+00005a20: 6e64 6572 2074 6865 2074 6572 6d73 206f  nder the terms o
+00005a30: 6620 7468 6520 4d49 5420 6c69 6365 6e73  f the MIT licens
+00005a40: 652e 0a                                  e..
```

