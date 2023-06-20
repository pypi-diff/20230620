# Comparing `tmp/jupyter_releaser-1.1.6.tar.gz` & `tmp/jupyter_releaser-1.2.0.tar.gz`

## Comparing `jupyter_releaser-1.1.6.tar` & `jupyter_releaser-1.2.0.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/.readthedocs.yml
--rw-r--r--   0        0        0   125164 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/CHANGELOG.md
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/CONTRIBUTING.md
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/RELEASE.md
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/.github/dependabot.yml
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/.github/actions/check-release/action.yml
--rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/.github/actions/finalize-release/action.yml
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/.github/actions/install-releaser/action.yml
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/.github/actions/populate-release/action.yml
--rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/.github/actions/prep-release/action.yml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/.github/scripts/bump_tag.sh
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/.github/workflows/check-release.yml
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/.github/workflows/enforce-label.yml
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/.github/workflows/generate-changelog.yml
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/.github/workflows/prep-release.yml
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/.github/workflows/publish-release.yml
--rw-r--r--   0        0        0     4984 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/.github/workflows/test.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/Makefile
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/make.bat
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/conf.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/index.rst
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/_static/custom.css
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/_static/images/logo/favicon.svg
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/_static/images/logo/logo.svg
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/background/index.rst
--rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/background/theory.md
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/get_started/generate_changelog.md
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/get_started/index.rst
--rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/get_started/making_release_from_releaser.md
--rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/get_started/making_release_from_repo.md
--rw-r--r--   0        0        0     5831 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/how_to_guides/convert_repo_from_releaser.md
--rw-r--r--   0        0        0     5996 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/how_to_guides/convert_repo_from_repo.md
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/how_to_guides/index.rst
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/how_to_guides/maintain_fork.md
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/how_to_guides/write_config.md
--rw-r--r--   0        0        0   507289 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/images/draft_github_release.png
--rw-r--r--   0        0        0   586032 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/images/final_github_release.png
--rw-r--r--   0        0        0   169812 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/images/fork_fetch.png
--rw-r--r--   0        0        0   276246 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/images/generate_changelog.png
--rw-r--r--   0        0        0    99291 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/images/prep_release.png
--rw-r--r--   0        0        0   212895 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/images/prep_release_next_step.png
--rw-r--r--   0        0        0   237681 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/images/prep_release_repo.png
--rw-r--r--   0        0        0    74988 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/images/publish_release.png
--rw-r--r--   0        0        0   177023 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/images/publish_release_next_step.png
--rw-r--r--   0        0        0   191024 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/images/publish_release_repo.png
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/reference/api_docs.rst
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/reference/configuration.md
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/reference/faq.md
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/reference/index.rst
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/docs/source/reference/releaser_cli.rst
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/example-workflows/full-release.yml
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/example-workflows/prep-release.yml
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/example-workflows/publish-release.yml
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/__init__.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/__main__.py
--rw-r--r--   0        0        0    10551 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/changelog.py
--rw-r--r--   0        0        0    19367 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/cli.py
--rw-r--r--   0        0        0    18954 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/lib.py
--rw-r--r--   0        0        0     8147 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/mock_github.py
--rw-r--r--   0        0        0     6288 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/npm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/py.typed
--rw-r--r--   0        0        0     4904 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/python.py
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/schema.json
--rw-r--r--   0        0        0     6026 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/tee.py
--rw-r--r--   0        0        0    24466 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/actions/__init__.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/actions/common.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/actions/finalize_release.py
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/actions/generate_changelog.py
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/actions/populate_release.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/actions/prep_release.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/tests/__init__.py
--rw-r--r--   0        0        0     6589 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/tests/conftest.py
--rw-r--r--   0        0        0    26407 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/tests/test_cli.py
--rw-r--r--   0        0        0    12126 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/tests/test_functions.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/tests/test_mock_github.py
--rw-r--r--   0        0        0     8815 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/jupyter_releaser/tests/util.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/.gitignore
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/LICENSE
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/README.md
--rw-r--r--   0        0        0     5815 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/pyproject.toml
--rw-r--r--   0        0        0     5469 2020-02-02 00:00:00.000000 jupyter_releaser-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/.readthedocs.yml
+-rw-r--r--   0        0        0   126470 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/RELEASE.md
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/.github/actions/check-release/action.yml
+-rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/.github/actions/finalize-release/action.yml
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/.github/actions/install-releaser/action.yml
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/.github/actions/populate-release/action.yml
+-rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/.github/actions/prep-release/action.yml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/.github/scripts/bump_tag.sh
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/.github/workflows/check-release.yml
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/.github/workflows/enforce-label.yml
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/.github/workflows/generate-changelog.yml
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/.github/workflows/prep-release.yml
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/.github/workflows/publish-release.yml
+-rw-r--r--   0        0        0     4984 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/Makefile
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/make.bat
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/conf.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/index.rst
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/_static/custom.css
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/_static/images/logo/favicon.svg
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/_static/images/logo/logo.svg
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/background/index.rst
+-rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/background/theory.md
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/get_started/generate_changelog.md
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/get_started/index.rst
+-rw-r--r--   0        0        0     6044 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/get_started/making_release_from_releaser.md
+-rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/get_started/making_release_from_repo.md
+-rw-r--r--   0        0        0     6706 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/how_to_guides/convert_repo_from_releaser.md
+-rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/how_to_guides/convert_repo_from_repo.md
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/how_to_guides/index.rst
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/how_to_guides/maintain_fork.md
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/how_to_guides/write_config.md
+-rw-r--r--   0        0        0   507289 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/images/draft_github_release.png
+-rw-r--r--   0        0        0   586032 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/images/final_github_release.png
+-rw-r--r--   0        0        0   169812 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/images/fork_fetch.png
+-rw-r--r--   0        0        0   276246 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/images/generate_changelog.png
+-rw-r--r--   0        0        0    99291 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/images/prep_release.png
+-rw-r--r--   0        0        0   212895 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/images/prep_release_next_step.png
+-rw-r--r--   0        0        0   237681 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/images/prep_release_repo.png
+-rw-r--r--   0        0        0    74988 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/images/publish_release.png
+-rw-r--r--   0        0        0   177023 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/images/publish_release_next_step.png
+-rw-r--r--   0        0        0   191024 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/images/publish_release_repo.png
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/reference/api_docs.rst
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/reference/configuration.md
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/reference/faq.md
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/reference/index.rst
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/docs/source/reference/releaser_cli.rst
+-rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/example-workflows/full-release.yml
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/example-workflows/prep-release.yml
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/example-workflows/publish-release.yml
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/__init__.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/__main__.py
+-rw-r--r--   0        0        0    10551 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/changelog.py
+-rw-r--r--   0        0        0    19620 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/cli.py
+-rw-r--r--   0        0        0    19880 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/lib.py
+-rw-r--r--   0        0        0     8147 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/mock_github.py
+-rw-r--r--   0        0        0     6624 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/npm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/py.typed
+-rw-r--r--   0        0        0     6678 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/python.py
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/schema.json
+-rw-r--r--   0        0        0     6026 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/tee.py
+-rw-r--r--   0        0        0    24593 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/actions/__init__.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/actions/common.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/actions/finalize_release.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/actions/generate_changelog.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/actions/populate_release.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/actions/prep_release.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/tests/__init__.py
+-rw-r--r--   0        0        0     6589 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/tests/conftest.py
+-rw-r--r--   0        0        0    26596 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/tests/test_cli.py
+-rw-r--r--   0        0        0    12126 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/tests/test_functions.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/tests/test_mock_github.py
+-rw-r--r--   0        0        0     8815 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/jupyter_releaser/tests/util.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/README.md
+-rw-r--r--   0        0        0     5815 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5469 2020-02-02 00:00:00.000000 jupyter_releaser-1.2.0/PKG-INFO
```

### Comparing `jupyter_releaser-1.1.6/.pre-commit-config.yaml` & `jupyter_releaser-1.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/CHANGELOG.md` & `jupyter_releaser-1.2.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,36 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 1.2.0
+
+([Full Changelog](https://github.com/jupyter-server/jupyter_releaser/compare/v2...b1388d01b8d28ea077fab281bd78ecc1c9c18773))
+
+### Enhancements made
+
+- Add support for PyPI trusted publisher and NPM provenance [#511](https://github.com/jupyter-server/jupyter_releaser/pull/511) ([@fcollonval](https://github.com/fcollonval))
+- Dynamically set the NPM tag [#510](https://github.com/jupyter-server/jupyter_releaser/pull/510) ([@fcollonval](https://github.com/fcollonval))
+
+### Bugs fixed
+
+- Fix package version target [#514](https://github.com/jupyter-server/jupyter_releaser/pull/514) ([@fcollonval](https://github.com/fcollonval))
+
+### Documentation improvements
+
+- Fix doc edition links [#515](https://github.com/jupyter-server/jupyter_releaser/pull/515) ([@fcollonval](https://github.com/fcollonval))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter-server/jupyter_releaser/graphs/contributors?from=2023-06-19&to=2023-06-20&type=c))
+
+[@blink1073](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_releaser+involves%3Ablink1073+updated%3A2023-06-19..2023-06-20&type=Issues) | [@fcollonval](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_releaser+involves%3Afcollonval+updated%3A2023-06-19..2023-06-20&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 1.1.6
 
 ([Full Changelog](https://github.com/jupyter-server/jupyter_releaser/compare/v2...0b4c9cc2b257e799794c6d02735b659da09e2336))
 
 ### Maintenance and upkeep improvements
 
 - Pin ghapi [#512](https://github.com/jupyter-server/jupyter_releaser/pull/512) ([@blink1073](https://github.com/blink1073))
@@ -20,16 +45,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyter-server/jupyter_releaser/graphs/contributors?from=2023-01-26&to=2023-06-19&type=c))
 
 [@blink1073](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_releaser+involves%3Ablink1073+updated%3A2023-01-26..2023-06-19&type=Issues) | [@codecov](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_releaser+involves%3Acodecov+updated%3A2023-01-26..2023-06-19&type=Issues) | [@jtpio](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_releaser+involves%3Ajtpio+updated%3A2023-01-26..2023-06-19&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter_releaser+involves%3Apre-commit-ci+updated%3A2023-01-26..2023-06-19&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 1.1.5
 
 ([Full Changelog](https://github.com/jupyter-server/jupyter_releaser/compare/v2...2acb616f67cf9edc926bf5d877a434f59dbb0ee6))
 
 ### Enhancements made
 
 - Add whitelist for http request in yarn [#491](https://github.com/jupyter-server/jupyter_releaser/pull/491) ([@brichet](https://github.com/brichet))
```

### Comparing `jupyter_releaser-1.1.6/CONTRIBUTING.md` & `jupyter_releaser-1.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/.github/actions/check-release/action.yml` & `jupyter_releaser-1.2.0/.github/actions/check-release/action.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/.github/actions/finalize-release/action.yml` & `jupyter_releaser-1.2.0/.github/actions/finalize-release/action.yml`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
   steps:
     - name: install-releaser
       shell: bash -eux {0}
       run: |
         # Install Jupyter Releaser from git unless we are testing Releaser itself
         if ! command -v jupyter-releaser &> /dev/null
         then
-            pip install -q git+https://github.com/jupyter-server/jupyter_releaser.git@v1
+            pip install -q git+https://github.com/jupyter-server/jupyter_releaser.git@v2
         fi
 
     - id: finalize-release
       shell: bash -eux {0}
       run: |
         export GITHUB_ACCESS_TOKEN=${{ inputs.token }}
         export GITHUB_ACTOR=${{ github.triggering_actor }}
```

### Comparing `jupyter_releaser-1.1.6/.github/actions/populate-release/action.yml` & `jupyter_releaser-1.2.0/.github/actions/populate-release/action.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/.github/actions/prep-release/action.yml` & `jupyter_releaser-1.2.0/.github/actions/prep-release/action.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/.github/workflows/check-release.yml` & `jupyter_releaser-1.2.0/.github/workflows/check-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/.github/workflows/generate-changelog.yml` & `jupyter_releaser-1.2.0/.github/workflows/generate-changelog.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/.github/workflows/prep-release.yml` & `jupyter_releaser-1.2.0/.github/workflows/prep-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/.github/workflows/publish-release.yml` & `jupyter_releaser-1.2.0/.github/workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/.github/workflows/test.yml` & `jupyter_releaser-1.2.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/docs/Makefile` & `jupyter_releaser-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/docs/make.bat` & `jupyter_releaser-1.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/docs/source/conf.py` & `jupyter_releaser-1.2.0/docs/source/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,16 +77,16 @@
 # Add an Edit this Page button
 html_theme_options = {
     "use_edit_page_button": True,
 }
 
 # Output for github to be used in links
 html_context = {
-    "github_user": "jupyterlab",  # Username
-    "github_repo": "jupyterlab_server",  # Repo name
+    "github_user": "jupyter-server",  # Username
+    "github_repo": "jupyter_releaser",  # Repo name
     "github_version": "main",  # Version
     "doc_path": "/docs/source/",  # Path in the checkout to the docs root
 }
 
 
 def setup(app):
     dest = osp.join(HERE, "reference", "changelog.md")
```

### Comparing `jupyter_releaser-1.1.6/docs/source/_static/images/logo/favicon.svg` & `jupyter_releaser-1.2.0/docs/source/_static/images/logo/favicon.svg`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/docs/source/_static/images/logo/logo.svg` & `jupyter_releaser-1.2.0/docs/source/_static/images/logo/logo.svg`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/docs/source/background/theory.md` & `jupyter_releaser-1.2.0/docs/source/background/theory.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/docs/source/get_started/generate_changelog.md` & `jupyter_releaser-1.2.0/docs/source/get_started/generate_changelog.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/docs/source/get_started/making_release_from_releaser.md` & `jupyter_releaser-1.2.0/docs/source/get_started/making_release_from_releaser.md`

 * *Files 14% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 
 - Fork `jupyter_releaser`
 
 - Generate a [GitHub Access token](https://docs.github.com/en/github/authenticating-to-github/creating-a-personal-access-token) with access to target GitHub repo to run GitHub Actions
 
 - Add the token as `ADMIN_GITHUB_TOKEN` in the [repository secrets](https://docs.github.com/en/actions/reference/encrypted-secrets#creating-encrypted-secrets-for-a-repository) of your fork. The token must have `repo` and `workflow` scopes.
 
+- Set up PyPI:
+
+<details><summary>Using PyPI token (legacy way)</summary>
+
 - If the repo generates PyPI release(s), create a scoped PyPI [token](https://packaging.python.org/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/#saving-credentials-on-github). We recommend using a scoped token for security reasons.
 
 - You can store the token as `PYPI_TOKEN` in your fork's `Secrets`.
 
   - Advanced usage: if you are releasing multiple repos, you can create a secret named `PYPI_TOKEN_MAP` instead of `PYPI_TOKEN` that is formatted as follows:
 
     ```text
@@ -30,16 +34,29 @@
     If you have multiple Python packages in the same repository, you can point to them as follows:
 
     ```text
     owner1/repo1/path/to/package1,token1
     owner1/repo1/path/to/package2,token2
     ```
 
+</details>
+
+<details><summary>Using PyPI trusted publisher (modern way)</summary>
+
+- Set up your PyPI project by [adding a trusted publisher](https://docs.pypi.org/trusted-publishers/adding-a-publisher/)
+  - if you use the example workflows, the _workflow name_ is `publish-release.yml` (or `full-release.yml`) and the
+    _environment_ should be left blank.
+- Ensure the publish release job as `permissions`: `id-token : write` (see the [documentation](https://docs.pypi.org/trusted-publishers/using-a-publisher/))
+
+</details>
+
 - If the repo generates npm release(s), add access token for [npm](https://docs.npmjs.com/creating-and-viewing-access-tokens), saved as `NPM_TOKEN` in "Secrets".
 
+> If you want to set _provenance_ on your package, you need to ensure the publish release job as `permissions`: `id-token : write` (see the [documentation](https://docs.npmjs.com/generating-provenance-statements#publishing-packages-with-provenance-via-github-actions)).
+
 ## Prep Release
 
 - Go to the "Actions" tab in your fork of `jupyter_releaser`
 
 - Select the "Step 1: Prep Release" workflow on the left
 
 - Click on the "Run workflow" dropdown button on the right
```

### Comparing `jupyter_releaser-1.1.6/docs/source/get_started/making_release_from_repo.md` & `jupyter_releaser-1.2.0/docs/source/get_started/making_release_from_repo.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/docs/source/how_to_guides/convert_repo_from_releaser.md` & `jupyter_releaser-1.2.0/docs/source/how_to_guides/convert_repo_from_repo.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,52 +1,58 @@
-# Convert a Repo to Use Releaser from Releaser
+# Convert a Repo to Use Releaser from Repo
 
-Follow the steps below to convert a repository to use Jupyter Releaser for releases, where maintainers make releases from a fork of Jupyter Releaser.
+Follow the steps below to convert a repository to use Jupyter Releaser for releases, where maintainers make releases from the repository itself.
 
 ## Prerequisites
 
 See checklist below for details:
 
 - Markdown changelog
-- Bump version configuration (if using Python), for example [tbump](https://github.com/dmerejkowsky/tbump)
+- Bump version configuration (if using Python), for example [hatch](https://hatch.pypa.io/latest/)
 - [Access token](https://docs.github.com/en/github/authenticating-to-github/creating-a-personal-access-token) with access to target GitHub repo to run GitHub Actions.
-- Access token for the [PyPI registry](https://packaging.python.org/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/#saving-credentials-on-github)
+- Set up:
+  - \[_modern way_\] [Add a trusted publisher](https://docs.pypi.org/trusted-publishers/adding-a-publisher/) to your PyPI project
+  - \[_legacy way_\] Access token for the [PyPI registry](https://packaging.python.org/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/#saving-credentials-on-github)
 - If needed, access token for [npm](https://docs.npmjs.com/creating-and-viewing-access-tokens).
 
 ## Checklist for Adoption
 
-A. Prep the `jupyter_releaser` fork:
+- [ ] Add a GitHub [personal access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token), preferably from a "machine user" GitHub
+  account that has admin access to the repository. The token itself will
+  need "public_repo", and "repo:status" permissions. Save the token as
+  `ADMIN_GITHUB_TOKEN`
+  in the [repository secrets](https://docs.github.com/en/actions/reference/encrypted-secrets#creating-encrypted-secrets-for-a-repository). We need this
+  access token to allow for branch protection rules, which block the pushing
+  of commits when using the `GITHUB_TOKEN`, even when run from an admin user
+  account.
 
-- [ ] Clone this repository onto your GitHub user account.
+- [ ] Set up PyPI:
 
-- [ ] Add a GitHub [personal access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) with access to target GitHub repo to run
-  GitHub Actions, saved as `ADMIN_GITHUB_TOKEN` in the
-  [repository secrets](https://docs.github.com/en/actions/reference/encrypted-secrets#creating-encrypted-secrets-for-a-repository).
-  The token will need "public_repo", and "repo:status" permissions.
+<details><summary>Using PyPI token (legacy way)</summary>
 
-- [ ] Add access token for the [PyPI registry](https://packaging.python.org/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/#saving-credentials-on-github) stored as `PYPI_TOKEN`.
+- Add access token for the [PyPI registry](https://packaging.python.org/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/#saving-credentials-on-github) stored as `PYPI_TOKEN`.
   _Note_ For security reasons, it is recommended that you scope the access
-  to a single repository, and use a variable called `PYPI_TOKEN_MAP` that is formatted as follows:
+  to a single repository. Additionally, this token should belong to a
+  machine account and not a user account.
 
-  ```text
-  owner1/repo1,token1
-  owner2/repo2,token2
-  ```
+</details>
 
-  If you have multiple Python packages in the same repository, you can point to them as follows:
+<details><summary>Using PyPI trusted publisher (modern way)</summary>
 
-  ```text
-  owner1/repo1/path/to/package1,token1
-  owner1/repo1/path/to/package2,token2
-  ```
+- Set up your PyPI project by [adding a trusted publisher](https://docs.pypi.org/trusted-publishers/adding-a-publisher/)
+  - if you use the example workflows, the _workflow name_ is `publish-release.yml` (or `full-release.yml`) and the
+    _environment_ should be left blank.
+- Ensure the publish release job as `permissions`: `id-token : write` (see the [documentation](https://docs.pypi.org/trusted-publishers/using-a-publisher/))
 
-- [ ] If needed, add access token for [npm](https://docs.npmjs.com/creating-and-viewing-access-tokens), saved as `NPM_TOKEN`.
-
-B. Prep target repository:
+</details>
 
+- [ ] If needed, add access token for [npm](https://docs.npmjs.com/creating-and-viewing-access-tokens), saved as `NPM_TOKEN`. Again this should
+  be created using a machine account that only has publish access.
+- [ ] Ensure that only trusted users with 2FA have admin access to the
+  repository, since they will be able to trigger releases.
 - [ ] Switch to Markdown Changelog
   - We recommend [MyST](https://myst-parser.readthedocs.io/en/latest/?badge=latest), especially if some of your docs are in reStructuredText.
   - Can use `pandoc -s changelog.rst -o changelog.md` and some hand edits as needed.
   - Note that [directives](https://myst-parser.readthedocs.io/en/latest/using/syntax.html#syntax-directives) can still be used
 - [ ] Add HTML start and end comment markers to Changelog file - see example in [CHANGELOG.md](https://github.com/jupyter-server/jupyter_releaser/blob/main/CHANGELOG.md) (view in raw mode)
 - [ ] We recommend using [hatch](https://hatch.pypa.io/latest/) for your
   build system and for version handling.
@@ -85,30 +91,34 @@
 
 - [ ] If you would like the release assets to be uploaded as artifacts, add the following step after the `check_release` action:
 
 ```yaml
 - name: Upload Distributions
   uses: actions/upload-artifact@v2
   with:
-    name: jupyter-releaser-dist-${{ github.run_number }}
+    name: dist-${{ github.run_number }}
     path: .jupyter_releaser_checkout/dist
 ```
 
 - [ ] Add a workflow that uses the [`enforce-label`](https://github.com/jupyterlab/maintainer-tools#enforce-labels) action from `jupyterlab/maintainer-tools` to ensure that all PRs have on of the triage labels used to
   categorize the changelog.
 
 - [ ] Update or add `RELEASE.md` that describes the onboarding and release process, e.g. [jupyter_server](https://github.com/jupyter-server/jupyter_server/blob/main/RELEASE.md).
 
-## Release Workflow
+- [ ] Copy `prep-release.yml` and `publish-release.yml` from the `example-workflows` folder in this repository.
+
+- [ ] Optionally add configuration to the repository if non-standard options or hooks are needed.
+
+- [ ] If desired, add `check_release` job, changelog, and `hatch` support to other active release branches
+
+## Initial Release Workflow
+
+- [ ] Try out the `Prep Release` and `Publish Release` process against a fork of the target repo first so you don't accidentally push tags and GitHub releases to the source repository. Set the `TWINE_REPOSITORY_URL` environment variable to `https://test.pypi.org/legacy/` in the "Finalize Release" action part of the workflow
 
-- [ ] Set up a fork of `jupyter-releaser` if you have not yet done so.
-- [ ] Run through the release process, targeting this repo and the appropriate branch
-- [ ] Optionally add configuration to the target repository if non-standard options or hooks are needed.
-- [ ] If desired, add `check_release` job, changelog, and `tbump` support to other active release branches
-- [ ] Try out the `Draft Changelog` and `Draft Release` process against a fork of the target repo first so you don't accidentally push tags and GitHub releases to the source repository.
-- [ ] Try the `Publish Release` process using a prerelease version before publishing a final version.
+- [ ] Try the `Publish Release` process using a prerelease version on the main
+  repository before publishing a final version.
 
 ## Backport Branches
 
 - Create backport branches the usual way, e.g. `git checkout -b 3.0.x v3.0.1; git push origin 3.0.x`
 - When running the `Publish Release` Workflow, an automatic PR is generated for the default branch
   in the target repo, positioned in the appropriate place in the changelog.
```

### Comparing `jupyter_releaser-1.1.6/docs/source/how_to_guides/convert_repo_from_repo.md` & `jupyter_releaser-1.2.0/docs/source/how_to_guides/convert_repo_from_releaser.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,69 @@
-# Convert a Repo to Use Releaser from Repo
+# Convert a Repo to Use Releaser from Releaser
 
-Follow the steps below to convert a repository to use Jupyter Releaser for releases, where maintainers make releases from the repository itself.
+Follow the steps below to convert a repository to use Jupyter Releaser for releases, where maintainers make releases from a fork of Jupyter Releaser.
 
 ## Prerequisites
 
 See checklist below for details:
 
 - Markdown changelog
-- Bump version configuration (if using Python), for example [hatch](https://hatch.pypa.io/latest/)
+- Bump version configuration (if using Python), for example [tbump](https://github.com/dmerejkowsky/tbump)
 - [Access token](https://docs.github.com/en/github/authenticating-to-github/creating-a-personal-access-token) with access to target GitHub repo to run GitHub Actions.
 - Access token for the [PyPI registry](https://packaging.python.org/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/#saving-credentials-on-github)
 - If needed, access token for [npm](https://docs.npmjs.com/creating-and-viewing-access-tokens).
 
 ## Checklist for Adoption
 
-- [ ] Add a GitHub [personal access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token), preferably from a "machine user" GitHub
-  account that has admin access to the repository. The token itself will
-  need "public_repo", and "repo:status" permissions. Save the token as
-  `ADMIN_GITHUB_TOKEN`
-  in the [repository secrets](https://docs.github.com/en/actions/reference/encrypted-secrets#creating-encrypted-secrets-for-a-repository). We need this
-  access token to allow for branch protection rules, which block the pushing
-  of commits when using the `GITHUB_TOKEN`, even when run from an admin user
-  account.
-- [ ] Add access token for the [PyPI registry](https://packaging.python.org/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/#saving-credentials-on-github) stored as `PYPI_TOKEN`.
+A. Prep the `jupyter_releaser` fork:
+
+- [ ] Clone this repository onto your GitHub user account.
+
+- [ ] Add a GitHub [personal access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) with access to target GitHub repo to run
+  GitHub Actions, saved as `ADMIN_GITHUB_TOKEN` in the
+  [repository secrets](https://docs.github.com/en/actions/reference/encrypted-secrets#creating-encrypted-secrets-for-a-repository).
+  The token will need "public_repo", and "repo:status" permissions.
+
+- [ ] Set up PyPI:
+
+<details><summary>Using PyPI token (legacy way)</summary>
+
+- Add access token for the [PyPI registry](https://packaging.python.org/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/#saving-credentials-on-github) stored as `PYPI_TOKEN`.
   _Note_ For security reasons, it is recommended that you scope the access
-  to a single repository. Additionally, this token should belong to a
-  machine account and not a user account.
-- [ ] If needed, add access token for [npm](https://docs.npmjs.com/creating-and-viewing-access-tokens), saved as `NPM_TOKEN`. Again this should
-  be created using a machine account that only has publish access.
-- [ ] Ensure that only trusted users with 2FA have admin access to the
-  repository, since they will be able to trigger releases.
+  to a single repository, and use a variable called `PYPI_TOKEN_MAP` that is formatted as follows:
+
+  ```text
+  owner1/repo1,token1
+  owner2/repo2,token2
+  ```
+
+  If you have multiple Python packages in the same repository, you can point to them as follows:
+
+  ```text
+  owner1/repo1/path/to/package1,token1
+  owner1/repo1/path/to/package2,token2
+  ```
+
+</details>
+
+<details><summary>Using PyPI trusted publisher (modern way)</summary>
+
+- Set up your PyPI project by [adding a trusted publisher](https://docs.pypi.org/trusted-publishers/adding-a-publisher/)
+  - if you use the example workflows, the _workflow name_ is `publish-release.yml` (or `full-release.yml`) and the
+    _environment_ should be left blank.
+- Ensure the publish release job as `permissions`: `id-token : write` (see the [documentation](https://docs.pypi.org/trusted-publishers/using-a-publisher/))
+
+</details>
+
+- [ ] If needed, add access token for [npm](https://docs.npmjs.com/creating-and-viewing-access-tokens), saved as `NPM_TOKEN`.
+
+> If you want to set _provenance_ on your package, you need to ensure the publish release job as `permissions`: `id-token : write` (see the [documentation](https://docs.npmjs.com/generating-provenance-statements#publishing-packages-with-provenance-via-github-actions)).
+
+B. Prep target repository:
+
 - [ ] Switch to Markdown Changelog
   - We recommend [MyST](https://myst-parser.readthedocs.io/en/latest/?badge=latest), especially if some of your docs are in reStructuredText.
   - Can use `pandoc -s changelog.rst -o changelog.md` and some hand edits as needed.
   - Note that [directives](https://myst-parser.readthedocs.io/en/latest/using/syntax.html#syntax-directives) can still be used
 - [ ] Add HTML start and end comment markers to Changelog file - see example in [CHANGELOG.md](https://github.com/jupyter-server/jupyter_releaser/blob/main/CHANGELOG.md) (view in raw mode)
 - [ ] We recommend using [hatch](https://hatch.pypa.io/latest/) for your
   build system and for version handling.
@@ -72,34 +102,30 @@
 
 - [ ] If you would like the release assets to be uploaded as artifacts, add the following step after the `check_release` action:
 
 ```yaml
 - name: Upload Distributions
   uses: actions/upload-artifact@v2
   with:
-    name: dist-${{ github.run_number }}
+    name: jupyter-releaser-dist-${{ github.run_number }}
     path: .jupyter_releaser_checkout/dist
 ```
 
 - [ ] Add a workflow that uses the [`enforce-label`](https://github.com/jupyterlab/maintainer-tools#enforce-labels) action from `jupyterlab/maintainer-tools` to ensure that all PRs have on of the triage labels used to
   categorize the changelog.
 
 - [ ] Update or add `RELEASE.md` that describes the onboarding and release process, e.g. [jupyter_server](https://github.com/jupyter-server/jupyter_server/blob/main/RELEASE.md).
 
-- [ ] Copy `prep-release.yml` and `publish-release.yml` from the `example-workflows` folder in this repository.
-
-- [ ] Optionally add configuration to the repository if non-standard options or hooks are needed.
-
-- [ ] If desired, add `check_release` job, changelog, and `hatch` support to other active release branches
-
-## Initial Release Workflow
-
-- [ ] Try out the `Prep Release` and `Publish Release` process against a fork of the target repo first so you don't accidentally push tags and GitHub releases to the source repository. Set the `TWINE_REPOSITORY_URL` environment variable to `https://test.pypi.org/legacy/` in the "Finalize Release" action part of the workflow
+## Release Workflow
 
-- [ ] Try the `Publish Release` process using a prerelease version on the main
-  repository before publishing a final version.
+- [ ] Set up a fork of `jupyter-releaser` if you have not yet done so.
+- [ ] Run through the release process, targeting this repo and the appropriate branch
+- [ ] Optionally add configuration to the target repository if non-standard options or hooks are needed.
+- [ ] If desired, add `check_release` job, changelog, and `tbump` support to other active release branches
+- [ ] Try out the `Draft Changelog` and `Draft Release` process against a fork of the target repo first so you don't accidentally push tags and GitHub releases to the source repository.
+- [ ] Try the `Publish Release` process using a prerelease version before publishing a final version.
 
 ## Backport Branches
 
 - Create backport branches the usual way, e.g. `git checkout -b 3.0.x v3.0.1; git push origin 3.0.x`
 - When running the `Publish Release` Workflow, an automatic PR is generated for the default branch
   in the target repo, positioned in the appropriate place in the changelog.
```

### Comparing `jupyter_releaser-1.1.6/docs/source/how_to_guides/write_config.md` & `jupyter_releaser-1.2.0/docs/source/how_to_guides/write_config.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/docs/source/images/draft_github_release.png` & `jupyter_releaser-1.2.0/docs/source/images/draft_github_release.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/docs/source/images/final_github_release.png` & `jupyter_releaser-1.2.0/docs/source/images/final_github_release.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/docs/source/images/fork_fetch.png` & `jupyter_releaser-1.2.0/docs/source/images/fork_fetch.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/docs/source/images/generate_changelog.png` & `jupyter_releaser-1.2.0/docs/source/images/generate_changelog.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/docs/source/images/prep_release.png` & `jupyter_releaser-1.2.0/docs/source/images/prep_release.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/docs/source/images/prep_release_next_step.png` & `jupyter_releaser-1.2.0/docs/source/images/prep_release_next_step.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/docs/source/images/prep_release_repo.png` & `jupyter_releaser-1.2.0/docs/source/images/prep_release_repo.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/docs/source/images/publish_release.png` & `jupyter_releaser-1.2.0/docs/source/images/publish_release.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/docs/source/images/publish_release_next_step.png` & `jupyter_releaser-1.2.0/docs/source/images/publish_release_next_step.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/docs/source/images/publish_release_repo.png` & `jupyter_releaser-1.2.0/docs/source/images/publish_release_repo.png`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/docs/source/reference/api_docs.rst` & `jupyter_releaser-1.2.0/docs/source/reference/api_docs.rst`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/docs/source/reference/faq.md` & `jupyter_releaser-1.2.0/docs/source/reference/faq.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/example-workflows/full-release.yml` & `jupyter_releaser-1.2.0/example-workflows/full-release.yml`

 * *Files 13% similar despite different names*

```diff
@@ -21,14 +21,18 @@
         type: boolean
       steps_to_skip:
         description: "Comma separated list of steps to skip during Populate Release"
         required: false
 jobs:
   full_release:
     runs-on: ubuntu-latest
+    permissions:
+      # This is useful if you want to use PyPI trusted publisher
+      # and NPM provenance
+      id-token: write
     steps:
       - uses: jupyterlab/maintainer-tools/.github/actions/base-setup@v1
 
       - name: Prep Release
         id: prep-release
         uses: jupyter-server/jupyter_releaser/.github/actions/prep-release@v2
         with:
@@ -47,17 +51,18 @@
           branch: ${{ github.event.inputs.branch }}
           release_url: ${{ steps.prep-release.outputs.release_url }}
           steps_to_skip: ${{ github.event.inputs.steps_to_skip }}
 
       - name: Finalize Release
         id: finalize-release
         env:
-          PYPI_TOKEN: ${{ secrets.PYPI_TOKEN }}
-          PYPI_TOKEN_MAP: ${{ secrets.PYPI_TOKEN_MAP }}
-          TWINE_USERNAME: __token__
+          # The following are needed if you use legacy PyPI set up
+          # PYPI_TOKEN: ${{ secrets.PYPI_TOKEN }}
+          # PYPI_TOKEN_MAP: ${{ secrets.PYPI_TOKEN_MAP }}
+          # TWINE_USERNAME: __token__
           NPM_TOKEN: ${{ secrets.NPM_TOKEN }}
         uses: jupyter-server/jupyter-releaser/.github/actions/finalize-release@v2
         with:
           token: ${{ secrets.ADMIN_GITHUB_TOKEN }}
           release_url: ${{ steps.populate-release.outputs.release_url }}
 
       - name: "** Next Step **"
```

### Comparing `jupyter_releaser-1.1.6/example-workflows/prep-release.yml` & `jupyter_releaser-1.2.0/example-workflows/prep-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/example-workflows/publish-release.yml` & `jupyter_releaser-1.2.0/example-workflows/publish-release.yml`

 * *Files 11% similar despite different names*

```diff
@@ -11,14 +11,18 @@
       steps_to_skip:
         description: "Comma separated list of steps to skip"
         required: false
 
 jobs:
   publish_release:
     runs-on: ubuntu-latest
+    permissions:
+      # This is useful if you want to use PyPI trusted publisher
+      # and NPM provenance
+      id-token: write
     steps:
       - uses: jupyterlab/maintainer-tools/.github/actions/base-setup@v1
 
       - name: Populate Release
         id: populate-release
         uses: jupyter-server/jupyter_releaser/.github/actions/populate-release@v2
         with:
@@ -26,17 +30,18 @@
           branch: ${{ github.event.inputs.branch }}
           release_url: ${{ github.event.inputs.release_url }}
           steps_to_skip: ${{ github.event.inputs.steps_to_skip }}
 
       - name: Finalize Release
         id: finalize-release
         env:
-          PYPI_TOKEN: ${{ secrets.PYPI_TOKEN }}
-          PYPI_TOKEN_MAP: ${{ secrets.PYPI_TOKEN_MAP }}
-          TWINE_USERNAME: __token__
+          # The following are needed if you use legacy PyPI set up
+          # PYPI_TOKEN: ${{ secrets.PYPI_TOKEN }}
+          # PYPI_TOKEN_MAP: ${{ secrets.PYPI_TOKEN_MAP }}
+          # TWINE_USERNAME: __token__
           NPM_TOKEN: ${{ secrets.NPM_TOKEN }}
         uses: jupyter-server/jupyter-releaser/.github/actions/finalize-release@v2
         with:
           token: ${{ secrets.ADMIN_GITHUB_TOKEN }}
           release_url: ${{ steps.populate-release.outputs.release_url }}
 
       - name: "** Next Step **"
```

### Comparing `jupyter_releaser-1.1.6/jupyter_releaser/changelog.py` & `jupyter_releaser-1.2.0/jupyter_releaser/changelog.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/jupyter_releaser/cli.py` & `jupyter_releaser-1.2.0/jupyter_releaser/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -596,14 +596,15 @@
         dist_dir,
         dry_run,
         release_url,
     )
 
 
 @main.command()
+@add_options(auth_options)
 @add_options(dist_dir_options)
 @click.option("--npm-token", help="A token for the npm release", envvar="NPM_TOKEN")
 @click.option(
     "--npm-cmd",
     help="The command to run for npm release",
     envvar="RH_NPM_COMMAND",
     default="npm publish",
@@ -622,38 +623,48 @@
 )
 @click.option(
     "--twine-repository-url",
     help="The pypi registry to target for publishing",
     envvar="TWINE_REPOSITORY_URL",
     default="https://upload.pypi.org/legacy/",
 )
+@click.option(
+    "--npm-tag",
+    help="The npm tag. It defaults to 'next' if it is a prerelease otherwise to 'latest'.",
+    envvar="NPM_TAG",
+    default="",
+)
 @add_options(dry_run_options)
 @add_options(python_packages_options)
 @add_options(release_url_options)
 @use_checkout_dir()
 def publish_assets(
+    auth,
     dist_dir,
     npm_token,
     npm_cmd,
     twine_cmd,
     npm_registry,
     twine_repository_url,
+    npm_tag,
     dry_run,
     release_url,
     python_packages,
 ):
     """Publish release asset(s)"""
     for python_package in python_packages:
         lib.publish_assets(
+            auth,
             dist_dir,
             npm_token,
             npm_cmd,
             twine_cmd,
             npm_registry,
             twine_repository_url,
+            npm_tag,
             dry_run,
             release_url,
             python_package,
         )
 
 
 @main.command()
```

### Comparing `jupyter_releaser-1.1.6/jupyter_releaser/lib.py` & `jupyter_releaser-1.2.0/jupyter_releaser/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import json
 import os
 import os.path as osp
 import re
 import shutil
 import tempfile
 import uuid
+import warnings
 from datetime import datetime, timezone
 from glob import glob
 from pathlib import Path
 from subprocess import CalledProcessError
 from typing import Type, Union
 
 import mdformat
@@ -311,41 +312,64 @@
             msg = f"sha for {asset.name} does not match asset_shas file"
             raise ValueError(msg)
 
     os.chdir(orig_dir)
 
 
 def publish_assets(  # noqa
+    auth,
     dist_dir,
     npm_token,
     npm_cmd,
     twine_cmd,
     npm_registry,
     twine_repository_url,
+    npm_tag,
     dry_run,
     release_url,
     python_package,
 ):
     """Publish release asset(s)"""
     os.environ["NPM_REGISTRY"] = npm_registry
     os.environ["TWINE_REPOSITORY_URL"] = twine_repository_url
     twine_token = ""
 
     if len(glob(f"{dist_dir}/*.tgz")):
         npm.handle_npm_config(npm_token)
         if npm_token:
             util.run("npm whoami")
+        # check if this is a prerelease
+        match = util.parse_release_url(release_url)
+        owner, repo = match["owner"], match["repo"]
+
+        gh = util.get_gh_object(dry_run=dry_run, owner=owner, repo=repo, token=auth)
+        release = util.release_for_url(gh, release_url)
+        is_prerelease = release.prerelease
+
+        if " --tag " not in npm_cmd:
+            npm_tag = npm_tag or ("next" if is_prerelease else "latest")
+            npm_cmd = f"{npm_cmd} --tag {npm_tag}"
+        elif npm_tag:
+            warnings.warn(
+                f"The NPM tag '{npm_tag}' will be ignored as at tag option is set in NPM command; '{npm_cmd}'.",
+                stacklevel=2,
+            )
 
     res = python_package.split(":")
     python_package_path = res[0]
     python_package_name = res[1].replace("-", "_") if len(res) == 2 else ""  # noqa
 
     if release_url and len(glob(f"{dist_dir}/*.whl")):
         twine_token = python.get_pypi_token(release_url, python_package_path)
 
+        if twine_token:
+            # tell GitHub Actions to mask the token in any console logs,
+            # to avoid leaking it
+            util.run(f'echo "::add-mask::{twine_token}"')
+
     if dry_run:
         # Start local pypi server with no auth, allowing overwrites,
         # in a temporary directory
         if len(glob(f"{dist_dir}/*.whl")):
             python.start_local_pypi()
             twine_cmd = "pipx run twine upload --repository-url=http://0.0.0.0:8081"
             os.environ["TWINE_USERNAME"] = "foo"
```

### Comparing `jupyter_releaser-1.1.6/jupyter_releaser/mock_github.py` & `jupyter_releaser-1.2.0/jupyter_releaser/mock_github.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/jupyter_releaser/npm.py` & `jupyter_releaser-1.2.0/jupyter_releaser/npm.py`

 * *Files 5% similar despite different names*

```diff
@@ -131,14 +131,21 @@
         text = npmrc.read_text(encoding="utf-8")
         if reg_entry in text:
             reg_entry = ""
         if auth_entry in text:
             auth_entry = ""
 
     text += f"\n{reg_entry}\n{auth_entry}"
+
+    if os.environ.get(util.GH_ID_TOKEN_TOKEN_VAR, ""):
+        util.log("Turning on NPM provenance as id-token permission is set.")
+        # See documentation https://docs.npmjs.com/generating-provenance-statements
+        # Also https://github.blog/2023-04-19-introducing-npm-package-provenance/
+        text += "\nprovenance=true"
+
     text = text.strip() + "\n"
     util.log(f"writing npm config to {npmrc}")
     npmrc.write_text(text, encoding="utf-8")
 
 
 def get_package_versions(version):
     """Get the formatted list of npm package names and versions"""
```

### Comparing `jupyter_releaser-1.1.6/jupyter_releaser/schema.json` & `jupyter_releaser-1.2.0/jupyter_releaser/schema.json`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/jupyter_releaser/tee.py` & `jupyter_releaser-1.2.0/jupyter_releaser/tee.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/jupyter_releaser/util.py` & `jupyter_releaser-1.2.0/jupyter_releaser/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,17 @@
 )
 
 SCHEMA = files("jupyter_releaser").joinpath("schema.json").read_text()
 SCHEMA = json.loads(SCHEMA)
 
 GIT_FETCH_CMD = "git fetch origin --filter=blob:none --quiet"
 
+GH_ID_TOKEN_URL_VAR = "ACTIONS_ID_TOKEN_REQUEST_URL"  # noqa
+GH_ID_TOKEN_TOKEN_VAR = "ACTIONS_ID_TOKEN_REQUEST_TOKEN"  # noqa
+
 
 def run(cmd, **kwargs):
     """Run a command as a subprocess and get the output as a string"""
     quiet_error = kwargs.pop("quiet_error", False)
     show_cwd = kwargs.pop("show_cwd", False)
     quiet = kwargs.get("quiet", False)
     echo = kwargs.pop("echo", False)
```

### Comparing `jupyter_releaser-1.1.6/jupyter_releaser/actions/common.py` & `jupyter_releaser-1.2.0/jupyter_releaser/actions/common.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/jupyter_releaser/actions/generate_changelog.py` & `jupyter_releaser-1.2.0/jupyter_releaser/actions/generate_changelog.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/jupyter_releaser/actions/populate_release.py` & `jupyter_releaser-1.2.0/jupyter_releaser/actions/populate_release.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/jupyter_releaser/actions/prep_release.py` & `jupyter_releaser-1.2.0/jupyter_releaser/actions/prep_release.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/jupyter_releaser/tests/conftest.py` & `jupyter_releaser-1.2.0/jupyter_releaser/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/jupyter_releaser/tests/test_cli.py` & `jupyter_releaser-1.2.0/jupyter_releaser/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,14 +148,15 @@
 check-imports: RH_CHECK_IMPORTS
 dist-dir: RH_DIST_DIR
 dry-run: RH_DRY_RUN
 expected-sha: RH_EXPECTED_SHA
 npm-cmd: RH_NPM_COMMAND
 npm-install-options: RH_NPM_INSTALL_OPTIONS
 npm-registry: NPM_REGISTRY
+npm-tag: NPM_TAG
 npm-token: NPM_TOKEN
 post-version-message: RH_POST_VERSION_MESSAGE
 post-version-spec: RH_POST_VERSION_SPEC
 pydist-check-cmd: RH_PYDIST_CHECK_CMD
 pydist-extra-check-cmds: RH_EXTRA_PYDIST_CHECK_CMDS
 pydist-resource-paths: RH_PYDIST_RESOURCE_PATHS
 python-packages: RH_PYTHON_PACKAGES
@@ -589,29 +590,33 @@
     assert called == 2, called
 
     log = get_log()
     assert "before-publish-assets" in log
     assert "after-publish-assets" in log
 
 
-def test_publish_assets_npm(npm_dist, runner, mocker):
+def test_publish_assets_npm(npm_dist, runner, mocker, mock_github):
+    # Create the release.
     dist_dir = npm_dist / util.CHECKOUT_NAME / "dist"
+    release = create_draft_release("bar", glob(f"{dist_dir!s}/*.*"))
+
+    os.environ["RH_RELEASE_URL"] = release.html_url
+
     orig_run = util.run
     called = 0
 
     def wrapped(cmd, **kwargs):
         nonlocal called
-        if cmd.startswith("npm publish --dry-run"):
+        if cmd.startswith("npm publish --dry-run --tag next"):
             called += 1
         return orig_run(cmd, **kwargs)
 
     mock_run = mocker.patch("jupyter_releaser.util.run", wraps=wrapped)
 
     runner(["publish-assets", "--npm-cmd", "npm publish --dry-run", "--dist-dir", dist_dir])
-
     assert called == 3, called
 
 
 def test_publish_assets_npm_exists(npm_dist, runner, mocker, mock_github, draft_release):
     os.environ["RH_RELEASE_URL"] = draft_release
     dist_dir = npm_dist / util.CHECKOUT_NAME / "dist"
     called = 0
```

### Comparing `jupyter_releaser-1.1.6/jupyter_releaser/tests/test_functions.py` & `jupyter_releaser-1.2.0/jupyter_releaser/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/jupyter_releaser/tests/test_mock_github.py` & `jupyter_releaser-1.2.0/jupyter_releaser/tests/test_mock_github.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/jupyter_releaser/tests/util.py` & `jupyter_releaser-1.2.0/jupyter_releaser/tests/util.py`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/.gitignore` & `jupyter_releaser-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/LICENSE` & `jupyter_releaser-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/README.md` & `jupyter_releaser-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/pyproject.toml` & `jupyter_releaser-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyter_releaser-1.1.6/PKG-INFO` & `jupyter_releaser-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_releaser
-Version: 1.1.6
+Version: 1.2.0
 Summary: Jupyter Releaser for Python and/or npm packages.
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: Copyright (c) 2021 Project Jupyter Contributors
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

