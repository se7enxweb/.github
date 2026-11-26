# se7enxweb / Exponential Platform — Default Community Health Files

This repository contains the default community health files for all [se7enxweb](https://github.com/se7enxweb) repositories hosting **Exponential Platform** and related open-source projects.

These files apply automatically to every repository in the `se7enxweb` organisation that does not have its own copy.

## What is Exponential Platform?

[Exponential Platform](https://se7enx.com) is a professional PHP application framework with advanced CMS functionality, driven by [7x](https://se7enx.com) — the North American corporation leading the continued development, support, hosting, and community growth of the platform.

7x has been supporting Exponential Platform website customers and projects for over 24 years. Current releases focus on PHP 8.2, 8.3, 8.4 and beyond compatibility.

> **Please note:** This project is not associated with the original eZ Publish software, eZ Systems, or Ibexa.

## Files in this repository

| File | Purpose |
|---|---|
| [CONTRIBUTING.md](CONTRIBUTING.md) | How to contribute code, issues and documentation |
| [SECURITY.md](SECURITY.md) | How to report security vulnerabilities |
| [SUPPORT.md](SUPPORT.md) | Where to get help |
| [.github/workflows/extension-ci.yml](.github/workflows/extension-ci.yml) | Shared CI for extension repositories (reusable workflow) |
| [workflow-templates/extension-ci.yml](workflow-templates/extension-ci.yml) | The caller an extension repository adds as its own `.github/workflows/ci.yml` |

## Shared CI for extension repositories

Every extension repository runs the same checks through one reusable workflow. Its own
`.github/workflows/ci.yml` is the short caller in `workflow-templates/extension-ci.yml`:

```yaml
jobs:
  extension:
    uses: se7enxweb/.github/.github/workflows/extension-ci.yml@main
```

In one job (one runner per repository) it runs `php -l` on every tracked PHP file on each of
PHP 7.4 and 8.0-8.5 that `require.php` in the repository's `composer.json` admits (all of them
when it states none), `xmllint` on `extension.xml`, a parity check of the version in
`ezinfo.php`, `extension.xml` and a `version` in `composer.json`, and PHPUnit when the
repository has a PHPUnit configuration and `phpunit/phpunit` in `require-dev`. Inputs:
`php-versions` (override the list), `test-command` (run after the lint on every version, for
tests that need no kernel) and `lint-exclude` (paths not to lint).

## More information

See the GitHub documentation on default community health files:  
https://docs.github.com/en/github/building-a-strong-community/creating-a-default-community-health-file
