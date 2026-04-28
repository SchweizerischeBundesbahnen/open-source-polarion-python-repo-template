# Changelog

## 0.1.0 (2026-04-28)


### Features

* add manual workflow trigger ([41415d0](https://github.com/SchweizerischeBundesbahnen/open-source-polarion-python-repo-template/commit/41415d09011db74a934c016f25db80b92ae32441))
* add pre-commit and workflow to check github workflows ([2a95018](https://github.com/SchweizerischeBundesbahnen/open-source-polarion-python-repo-template/commit/2a95018b7ac42ce9cd436f8850414c1876d143c0))
* enhance commit message checks and add sensitive data leak detection ([a241fba](https://github.com/SchweizerischeBundesbahnen/open-source-polarion-python-repo-template/commit/a241fba68577e8648248ab3a0cb0ad2dd6403333))
* migrate to poetry 2.0.0 and python 3.13 ([652f951](https://github.com/SchweizerischeBundesbahnen/open-source-polarion-python-repo-template/commit/652f95149c75dc1a66b49dcc3172eacd89f15c9f))
* migrate to poetry 2.0.0 and python 3.13 ([f3aa072](https://github.com/SchweizerischeBundesbahnen/open-source-polarion-python-repo-template/commit/f3aa07253cececdc0d5f967471dace04493cfe29))
* migrate workflows to reusable workflows from github-workflows-polarion ([#113](https://github.com/SchweizerischeBundesbahnen/open-source-polarion-python-repo-template/issues/113)) ([666ab26](https://github.com/SchweizerischeBundesbahnen/open-source-polarion-python-repo-template/commit/666ab264041b6cb2f60c42a32dfdd95177584cc4)), closes [#112](https://github.com/SchweizerischeBundesbahnen/open-source-polarion-python-repo-template/issues/112)
* replace commitizen with cocogitto/cocogitto-action ([c8a2ec4](https://github.com/SchweizerischeBundesbahnen/open-source-polarion-python-repo-template/commit/c8a2ec414bfa9e60be708c60baf72e8eec7ec4a5))


### Bug Fixes

* **ci:** fix release-please tag config and use frozen lockfile ([#122](https://github.com/SchweizerischeBundesbahnen/open-source-polarion-python-repo-template/issues/122)) ([a53cfff](https://github.com/SchweizerischeBundesbahnen/open-source-polarion-python-repo-template/commit/a53cffff39f2d14d6efc4137788e3936bc95046e)), closes [#116](https://github.com/SchweizerischeBundesbahnen/open-source-polarion-python-repo-template/issues/116)
* **ci:** use github.ref_name for SonarCloud push scan branch name ([#123](https://github.com/SchweizerischeBundesbahnen/open-source-polarion-python-repo-template/issues/123)) ([753b1a0](https://github.com/SchweizerischeBundesbahnen/open-source-polarion-python-repo-template/commit/753b1a0349547224ff77d2914fae4b6ba33b6097)), closes [#114](https://github.com/SchweizerischeBundesbahnen/open-source-polarion-python-repo-template/issues/114)
* sensitive data leaks regexp refactored ([#14](https://github.com/SchweizerischeBundesbahnen/open-source-polarion-python-repo-template/issues/14)) ([128b866](https://github.com/SchweizerischeBundesbahnen/open-source-polarion-python-repo-template/commit/128b866c2aee85f043a71890aa1022ac5b1bd8bb))
* sensitive data leaks regexp refactored ([#15](https://github.com/SchweizerischeBundesbahnen/open-source-polarion-python-repo-template/issues/15)) ([471c939](https://github.com/SchweizerischeBundesbahnen/open-source-polarion-python-repo-template/commit/471c939321e68cb0df993f29325c1290fcbf987b))
* trigger for all branches ([2f1e775](https://github.com/SchweizerischeBundesbahnen/open-source-polarion-python-repo-template/commit/2f1e775f1702bd2507ad2044c39cb298bab555e0))


### Performance Improvements

* switch tox to uv-venv-lock-runner for faster CI ([#109](https://github.com/SchweizerischeBundesbahnen/open-source-polarion-python-repo-template/issues/109)) ([da619d4](https://github.com/SchweizerischeBundesbahnen/open-source-polarion-python-repo-template/commit/da619d4fa59539d3b1fb4cde97ef7ae57da266ce))
* switch tox to uv-venv-lock-runner for faster CI ([#110](https://github.com/SchweizerischeBundesbahnen/open-source-polarion-python-repo-template/issues/110)) ([da619d4](https://github.com/SchweizerischeBundesbahnen/open-source-polarion-python-repo-template/commit/da619d4fa59539d3b1fb4cde97ef7ae57da266ce))


### Documentation

* remove workflow pinning rule from CLAUDE.md (moved to core plugin) ([9bb7c99](https://github.com/SchweizerischeBundesbahnen/open-source-polarion-python-repo-template/commit/9bb7c992498da0cac67649da3a10f968942e3dc8))
* update CLAUDE.md for uv migration and new tox envs ([a1b3192](https://github.com/SchweizerischeBundesbahnen/open-source-polarion-python-repo-template/commit/a1b31927a6f141e60dfba48603696ff0f31a0322))
* update CONTRIBUTING.md ([7510847](https://github.com/SchweizerischeBundesbahnen/open-source-polarion-python-repo-template/commit/7510847a52e945aef2c190eefd03639fd6c06cc2))
* update RELESE.md ([eced570](https://github.com/SchweizerischeBundesbahnen/open-source-polarion-python-repo-template/commit/eced570f77568675349e47e32a3b2e8bb347bc9d))
