# 7x · se7enxweb

**We keep Exponential shipping: the open-source PHP CMS behind sites that have run for 25 years, on today's PHP.**

[se7enx.com](https://se7enx.com) · [exponential.earth](https://exponential.earth) · [Docs](https://doc.exponential.earth) · [API reference](https://api.exponential.earth) · [Share](https://share.exponential.earth) · [Sponsor 7x](https://github.com/sponsors/se7enxweb)

Exponential is the free, GPL continuation of the eZ Publish line. 7x (formerly Brookins Consulting) has worked on it for
24+ years and has led the open-source project since 2023. Your existing content, templates and extensions keep running
on PHP 8.0 through 8.5.

**Try it:** [live demo](https://exponential.earth/about/demo) · [latest release](https://github.com/se7enxweb/exponential/releases/latest) · [Packagist](https://packagist.org/packages/se7enxweb/exponential)

---

## Why teams stay on Exponential

- **Content that lasts.** A typed content model, versions, translations and multi-site from one install. Sites
  launched in the 2000s still publish every day.
- **Upgrades without rewrites.** Templates, extensions and content carry across PHP and platform upgrades. We do the
  compatibility work so you don't have to rebuild.
- **Your choice of stack.** The classic kernel, the Symfony-based Platform, or both side by side. Apache, nginx,
  FrankenPHP or our own Velocity server.
- **Free for good.** GPL, no license fees, no vendor lock-in. Fork it whenever you want.

---

## Start here

| You want to | Go to |
|---|---|
| Run the CMS | [**exponential**](https://github.com/se7enxweb/exponential): Exponential 6, PHP 8.0–8.5, monthly releases · `composer require se7enxweb/exponential` |
| Run the modern stack and the legacy one together | [**exponential-platform-nexus**](https://github.com/se7enxweb/exponential-platform-nexus): Platform v2–v5 + Exponential 6 in one install |
| Run the modern stack only | [**exponential-platform-dxp**](https://github.com/se7enxweb/exponential-platform-dxp) · [**exponential-platform-legacy**](https://github.com/se7enxweb/exponential-platform-legacy) |
| Serve PHP faster, without Apache or FPM | [**exponential-velocity**](https://github.com/se7enxweb/exponential-velocity): a pure-PHP web server with persistent workers and static binaries |
| Let AI assistants work on a site safely | [**tron**](https://github.com/se7enxweb/tron): the open MCP server layer of Exponential. Agents act as real users, with tokens, policies and an audit log · `composer require se7enxweb/tron` · [product page](https://se7enx.com/products/tron) |
| Stop bots and scanners before PHP runs | [**exp_request_shield**](https://github.com/se7enxweb/exp_request_shield): a small web application firewall that decides every request |
| Move an old eZ Publish site forward | [**LegacyBridge**](https://github.com/se7enxweb/LegacyBridge) · [hire us](https://se7enx.com) |
| Learn the platform | [Docs](https://doc.exponential.earth) · [free training books](#free-training-books) |

---

## What we maintain

**Core**
- [exponential](https://github.com/se7enxweb/exponential): the CMS kernel, admin and installers. Monthly releases, each
  tested on every supported PHP version.
- [exponential-velocity](https://github.com/se7enxweb/exponential-velocity): the application server. Workers stay warm
  between requests, it ships as a single static binary, and it runs Exponential without Apache or PHP-FPM. [Product page](https://se7enx.com/products/exponential-velocity).
- [symfony](https://github.com/se7enxweb/symfony): our Symfony fork. The 3.x and 5.x branches are maintained here for
  current PHP, after upstream moved on.
- [LegacyBridge](https://github.com/se7enxweb/LegacyBridge): runs legacy extensions and templates next to the Symfony
  kernel, so a mixed site keeps working.

**Building sites**
- [explayouts](https://github.com/se7enxweb/explayouts) (Exponential Layouts): layouts, zones, blocks and rules, edited
  visually by editors instead of in templates. [Product page](https://se7enx.com/products/exponential-layouts).
- [expai](https://github.com/se7enxweb/expai) (Exponential Intelligence): AI-assisted writing and content creation
  inside the editor, with the provider you choose. [Product page](https://se7enx.com/products/exponential-intelligence).
- [tron](https://github.com/se7enxweb/tron): the open MCP server layer of Exponential. An AI agent works in your
  installation as one of its real users, under that user's roles and policies, with its own token, an audit log and an
  activity journal. [Product page](https://se7enx.com/products/tron).
- [media-site](https://github.com/se7enxweb/media-site) · [media-site-legacy](https://github.com/se7enxweb/media-site-legacy):
  a complete reference site, with content model, theme and layouts, to start from.

**Extensions**
- [cjw_newsletter](https://github.com/se7enxweb/cjw_newsletter): newsletters with lists, subscriptions and bounce
  handling, built into the admin.
- [ezjscore](https://github.com/se7enxweb/ezjscore): packs and caches CSS and JavaScript, now on jQuery 4.
- [ezoe](https://github.com/se7enxweb/ezoe): the online rich text editor.
- [NetgenInformationCollectionBundle](https://github.com/se7enxweb/NetgenInformationCollectionBundle): forms, surveys
  and collected data in the content model.

**Operations**
- [exp_request_shield](https://github.com/se7enxweb/exp_request_shield): rate limits, browser checks and scanner bans,
  with a dashboard in the admin.
- [ezmigrationbundle](https://github.com/se7enxweb/ezmigrationbundle): content and schema migrations as versioned
  YAML, run on every deploy.
- [metadata-bundle](https://github.com/se7enxweb/metadata-bundle): SEO titles, descriptions, Open Graph and Twitter
  cards per content type.
- [database translator](https://github.com/se7enxweb/sevenx_exponential_platform_v5_database_translator): rewrites
  MySQL queries to PostgreSQL in flight, so a site can move databases without code changes.

Everything else: [all repositories](https://github.com/se7enxweb?tab=repositories).

---

## Work with us

| Need | |
|---|---|
| A new site on Exponential | [se7enx.com](https://se7enx.com) |
| Migrate from eZ Publish or another CMS | [se7enx.com](https://se7enx.com) |
| Upgrade PHP, the platform or bundles | [se7enx.com](https://se7enx.com) |
| Support, maintenance, a redesign | [se7enx.com](https://se7enx.com) |
| Become a partner | [exponential.earth](https://exponential.earth) |

## Sponsor

Every release, security fix and PHP update is paid for by sponsors and client work. If your business runs on this
platform, sponsoring it is maintenance budget, not charity.

- **[Sponsor 7x](https://github.com/sponsors/se7enxweb)**: pays for the releases, the PHP work and the support.
- **[Sponsor the Exponential project](https://github.com/sponsors/exponentialcms)**: pays for the core libraries, the docs and community infrastructure.

## Free training books

700+ pages; everything in them still applies to Exponential today.

- [Basics](https://github.com/se7enxweb/mirror.exponential.se7enx.com/blob/master/books/ez_publish_basics_english.pdf)
- [Content management basics](https://github.com/se7enxweb/mirror.exponential.se7enx.com/blob/master/books/ez_publish_content_management_basics.pdf)
- [Advanced content management](https://github.com/se7enxweb/mirror.exponential.se7enx.com/blob/master/books/ez_publish_advanced_content_management.pdf)

## Contact

[se7enx.com](https://se7enx.com) · [Community Slack](https://ezcommunity.slack.com) · Security reports: security@se7enx.com

<sub>Exponential is not affiliated with eZ Systems or Ibexa. All software here is GPL-licensed and free.</sub>
