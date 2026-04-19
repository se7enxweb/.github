# 7x · se7enxweb

**North American stewards of Exponential Platform — the PHP CMS that refused to die.**

[se7enx.com](https://se7enx.com) · [exponential.earth](https://exponential.earth) · [mirror.ezpublish.se7enx.com](https://mirror.ezpublish.se7enx.com)

---

## What we're doing right now

### Keeping Exponential Platform alive — past its EOL and into the PHP 9 era

The platform originally known as eZ Publish reached end-of-life in 2021. We kept going. We maintain **Exponential Platform** — 100% source-compatible with the original eZ Publish stack (trademark usage removed) — through PHP 8.2, 8.3, 8.4, 8.5 and actively preparing for PHP 9.

**Active work in progress:**
- 🔒 **Security hardening across the full Zeta Components library** — 14 security PRs submitted upstream to [zetacomponents](https://github.com/zetacomponents) covering session fixation, SSRF, SQL injection, path traversal, predictable lock tokens, shell injection, and RCE via `eval()`. All changes verified against live source before any PR was opened.
- 🐘 **PHP 8.5+ compatibility** — active fork of Symfony maintained at [se7enxweb/symfony](https://github.com/se7enxweb/symfony) for General Public Use (GPL)
- 🔁 **Database translator** — [sevenx_exponential_platform_v5_database_translator](https://github.com/se7enxweb/sevenx_exponential_platform_v5_database_translator) intercepts every SQL query before it hits the wire and translates MySQL syntax to PostgreSQL in real-time, giving users a genuine choice of database
- 📦 **Distribution packages** — [Exponential Platform DXP](https://github.com/se7enxweb/exponential-platform-dxp) and [Exponential Platform Nexus](https://github.com/se7enxweb/exponential-platform-nexus) deliver the full stack (modern Platform + Legacy Bridge) as ready-to-install Composer packages
- 📚 **Free training book mirror** — three original developer training books (700+ pages combined) mirrored at [mirror.exponential.se7enx.com](https://github.com/se7enxweb/mirror.exponential.se7enx.com) so they are never lost

---

## What we've built for the freedom of everyone

> 7x has been in business supporting this platform and its community for **24+ years**. Previously known as Brookins Consulting, we took over leadership of the open-source project in 2023. Everything we do is GPL-licensed and freely available.

### Keeping a world-class CMS free and functional

| Achievement | What it means for you |
|---|---|
| Maintained PHP 7.4 → 8.4 compatibility | Your existing eZ Publish / Exponential Platform site still runs on current PHP |
| Forked and patched 47+ Zeta Components repos | The core PHP libraries powering the platform have security fixes and PHP 8 compatibility |
| Maintained the Legacy Bridge | Use the modern Symfony/DXP stack **and** keep your eZ Publish legacy extensions working |
| Kept the training books available | Three out-of-print developer books, free, always online |
| Built the Exponential Platform Nexus distribution | One Composer install gets you the complete integrated stack |
| PHP 8.5+ Symfony fork | The underlying framework works with the latest PHP before upstream catches up |
| Postgres database translator | First-class PostgreSQL support without rewriting a single query |
| GraphQL, REST, Solr search — all maintained | Modern integration options for headless and API-first architectures |

---

## 🧰 Most Powerful Bundles & Extensions

### Core Infrastructure

#### 🔗 [LegacyBridge](https://github.com/se7enxweb/LegacyBridge)
The bridge between the modern Symfony/DXP stack and Exponential Platform Legacy. Without this, legacy extensions and templates cannot co-exist with the new kernel. Co-maintained with the community. **If you run a mixed stack, this is not optional.**

#### 📦 [Exponential Platform Nexus](https://github.com/se7enxweb/exponential-platform-nexus)
The complete integrated distribution: Platform (Ibexa v2/3/4/5 OSS) + Exponential Legacy — in one Composer meta-package. The fastest path from zero to a running full-stack installation.

#### 🔄 [Database Translator — v5](https://github.com/se7enxweb/sevenx_exponential_platform_v5_database_translator)
Intercepts every SQL query before execution and transparently rewrites MySQL syntax to PostgreSQL. Run a MySQL-written CMS on Postgres with no query changes. Underserved and genuinely unique.

---

### Content & Editorial

#### 📋 [NetgenInformationCollectionBundle](https://github.com/se7enxweb/NetgenInformationCollectionBundle)
Forms, data collection, submissions — the feature that's always missing from CMS platforms. Build contact forms, surveys, and data capture workflows directly inside the content model.

#### 🔍 [ezplatform-query-fieldtype](https://github.com/se7enxweb/ezplatform-query-fieldtype)
A field type that builds dynamic content listings by querying the repository — no custom PHP required. Define a query in the content model and get a rendered list. Massively underused.

#### 📝 [ezmigrationbundle](https://github.com/se7enxweb/ezmigrationbundle)
Content and schema migrations as version-controlled YAML files. Run `migrate` on deploy the same way you run database migrations. Essential for any professional deployment pipeline.

#### 🌳 [SevenxExpPlatformNGSubtreeCopyWithLayouts](https://github.com/se7enxweb/SevenxExpPlatformNGSubtreeCopyWithLayouts)
Copy entire content subtrees (including NG Layouts page configuration and section assignments) in one operation. Solves a genuinely hard problem for multi-site and content staging workflows.

---

### Frontend & Administration

#### 🎨 [NetgenAdminUIBundle](https://github.com/se7enxweb/NetgenAdminUIBundle)
An alternative administration UI that implements a cleaner, more modern editorial experience on top of the Platform kernel. If the default admin UI doesn't fit your editorial workflow, this does.

#### 📐 [ezplatform-alloyeditor-element-width](https://github.com/se7enxweb/ezplatform-alloyeditor-element-width)
Adds a UI control to the Online Editor (AlloyEditor) for setting element width directly — a small but constantly-requested editorial capability that the base editor omits.

#### 🌿 [Twig (maintained fork)](https://github.com/se7enxweb/Twig)
The Twig template engine, maintained for use with Exponential Platform. Kept current with PHP compatibility fixes.

---

### SEO & Metadata

#### 🏷️ [metadata-bundle](https://github.com/se7enxweb/metadata-bundle)
Full metadata management for Exponential / eZ Platform content — titles, descriptions, Open Graph, Twitter Cards. Based on xrowmetadata. The most complete SEO metadata solution available for this stack.

#### 🔎 [ezseobundle](https://github.com/se7enxweb/ezseobundle)
SEO bundle for Exponential / eZ Platform. Handles sitemap generation, robots.txt, canonical URLs, and SEO field configuration per content type. Based on Novactive's work, maintained by 7x.

---

### Media & Rich Content

#### 🎬 [xrowvideo](https://github.com/se7enxweb/xrowvideo)
A video datatype with automatic transcoding into multiple formats and bitrates, plus a built-in video player. Handles upload → encode → serve without leaving the CMS.

#### 🖼️ [xrowsvg](https://github.com/se7enxweb/xrowsvg)
SVG editor and datatype for Exponential Platform Legacy. Edit SVG content inline in the CMS.

---

### Developer Tools

#### 🔧 [ngsymfonytools](https://github.com/se7enxweb/ngsymfonytools)
A Legacy extension that provides a way to include Twig templates inside eZ Publish Legacy template code. Bridges the template worlds so you don't have to maintain two separate UI stacks.

#### ↔️ [ezplatform-search-extra](https://github.com/se7enxweb/ezplatform-search-extra)
Extra search capabilities for Exponential / eZ Platform — additional criteria, sort clauses, and field-level search features not available in the standard search layer.

#### 🛠️ [system-info](https://github.com/se7enxweb/system-info)
System information and diagnostics bundle. Shows PHP version, extension status, database connectivity, and configuration health at a glance. Essential for auditing deployments.

#### 🍱 [sevenx-recipes](https://github.com/se7enxweb/sevenx-recipes)
Symfony Flex recipes for Exponential Platform DXP. Automate configuration file setup and bundle registration when installing packages. Pairs with `exponential-platform-dxp`.

---

### Workflows & Publishing

#### ⚙️ [xrowworkflow](https://github.com/se7enxweb/xrowworkflow)
A standard editorial publishing workflow for Exponential Platform Legacy — draft, review, approve, publish. The most complete open-source workflow solution for this stack.

#### 📊 [xrowquestionnaire](https://github.com/se7enxweb/xrowquestionnaire)
Questionnaires, polls, and quizzes built directly into the content model. Collect structured responses from visitors without a third-party tool.

---

### Media Site — Full Reference Implementation

#### 🖥️ [media-site](https://github.com/se7enxweb/media-site)
A complete, production-grade media website built on Exponential Platform + Netgen Layouts. This is the reference implementation that shows best practices for content modelling, theming, and layout management. Start here if you're building a content-heavy site.

#### 🗄️ [media-site-legacy](https://github.com/se7enxweb/media-site-legacy)
The Legacy variant of the media site — Ibexa v4 OSS + Exponential Legacy together. A working reference for mixed-stack deployments.

---

## 📚 Free Training Books

Three original developer training books — 700+ pages — free to download:

| Book | Get it |
|---|---|
| **Exponential Platform Basics** | [📄 Download PDF](https://github.com/se7enxweb/mirror.exponential.se7enx.com/blob/master/books/ez_publish_basics_english.pdf) |
| **Content Management Basics** | [📄 Download PDF](https://github.com/se7enxweb/mirror.ezpublish.se7enx.com/blob/master/books/ez_publish_content_management_basics.pdf) |
| **Advanced Content Management** | [📄 Download PDF](https://github.com/se7enxweb/mirror.ezpublish.se7enx.com/blob/d1c9393d30e8f7de2cbbe25f701960a4ff90d2d6/books/ez_publish_advanced_content_management.pdf) |

> These books describe the architecture that Exponential Platform is built on. Everything in them applies directly to development work on the platform today.

---

## Get involved

- 🌐 **Website:** [se7enx.com](https://se7enx.com)
- 💬 **Community Slack:** [ezcommunity.slack.com](https://ezcommunity.slack.com)
- 🐛 **Issues & PRs:** Browse any repo in [github.com/se7enxweb](https://github.com/se7enxweb)
- 📖 **API Docs:** [api.exponential.earth](https://api.exponential.earth)
- 📖 **Core Docs:** [doc.core.exponential.earth](https://doc.core.exponential.earth)
- 🔒 **Security:** security@se7enx.com

> Exponential Platform is not affiliated with eZ Systems or Ibexa. All software is GPL-licensed and free.
