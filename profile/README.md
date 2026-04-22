<div align="center">

<img src="https://cdn.prod.website-files.com/69c979c409e61c86a94c4f33/69c9859794db0e9297cc3fe0_cyguin3.png" width="110" alt="cyguin mascot" />

# cyguin.

**Drop-in developer tools. Open-core, self-hosted, no lock-in.**

unrelated to https://cygwin.com/. we're not that cool.

[![npm packages](https://img.shields.io/badge/npm-%40cyguin-FFD700?style=flat-square&logo=npm&logoColor=000)](https://www.npmjs.com/org/cyguin)
[![License](https://img.shields.io/badge/license-MIT-FFD700?style=flat-square)](https://github.com/cyguin)
[![Website](https://img.shields.io/badge/website-cyguin.com-FFD700?style=flat-square)](https://cyguin.com)
[![Demo](https://img.shields.io/badge/demo-npm%20suite-FFD700?style=flat-square)](https://github.com/cyguin/npm-suite-demo)

</div>

---

cyguin LLC builds small, practical software for teams that want useful product surfaces without renting their whole workflow from a vendor.

Most of the current work is the **cyguin npm suite**: self-hosted Next.js and React packages for common SaaS jobs like waitlists, notifications, changelogs, docs, feedback, surveys, consent banners, announcements, and snippet sharing. Each package ships the UI, API handler layer, storage adapters where needed, and MIT license.

---

## npm suite

The suite is being shaped as one coherent set of packages: shared cyguin styling, dark-by-default React components, self-hosted data ownership, and consistent package/repo conventions.

| Package | Current | Repo | What it does |
|---|---:|---|---|
| [`@cyguin/waitlist`](https://www.npmjs.com/package/@cyguin/waitlist) | `0.1.6` | [`cyguin/waitlist`](https://github.com/cyguin/waitlist) | Email waitlist with position tracking and referral tokens. |
| [`@cyguin/notify`](https://www.npmjs.com/package/@cyguin/notify) | `0.1.6` | [`cyguin/notify`](https://github.com/cyguin/notify) | Server-triggered in-app notification bell with unread state. |
| [`@cyguin/announce`](https://www.npmjs.com/package/@cyguin/announce) | `0.1.6` | [`cyguin/announce`](https://github.com/cyguin/announce) | Dismissible in-app announcement banners. |
| [`@cyguin/banner`](https://www.npmjs.com/package/@cyguin/banner) | `0.1.6` | [`cyguin/banner`](https://github.com/cyguin/banner) | Drop-in consent banner with accept/reject recording. |
| [`@cyguin/feedback`](https://www.npmjs.com/package/@cyguin/feedback) | `0.1.6` | [`cyguin/feedback`](https://github.com/cyguin/feedback) | Thumbs, rating, and free-text feedback widgets. |
| [`@cyguin/survey`](https://www.npmjs.com/package/@cyguin/survey) | `0.1.4` | [`cyguin/survey`](https://github.com/cyguin/survey) | Post-action micro-survey modal for 1-3 question prompts. |
| [`@cyguin/docs`](https://www.npmjs.com/package/@cyguin/docs) | `0.1.5` | [`cyguin/docs`](https://github.com/cyguin/docs) | Searchable docs widget plus self-hosted docs API/admin layer. |
| [`@cyguin/sniplet`](https://www.npmjs.com/package/@cyguin/sniplet) | `0.2.6` | [`cyguin/sniplet`](https://github.com/cyguin/sniplet) | Pastebin-style code snippets with expiry and burn-on-read. |
| [`@cyguin/changelog-react`](https://www.npmjs.com/package/@cyguin/changelog-react) | `0.1.10` | [`cyguin/changelog`](https://github.com/cyguin/changelog) | React changelog feed and unread badge. |
| [`@cyguin/changelog-core`](https://www.npmjs.com/package/@cyguin/changelog-core) | `0.1.10` | [`cyguin/changelog`](https://github.com/cyguin/changelog) | Changelog types and adapter interface. |
| [`@cyguin/changelog-cli`](https://www.npmjs.com/package/@cyguin/changelog-cli) | `0.1.10` | [`cyguin/changelog`](https://github.com/cyguin/changelog) | CLI scaffolder for changelog API routes. |
| [`@cyguin/changelog-adapter-sqlite`](https://www.npmjs.com/package/@cyguin/changelog-adapter-sqlite) | `0.1.10` | [`cyguin/changelog`](https://github.com/cyguin/changelog) | SQLite adapter for changelog storage. |
| [`@cyguin/changelog-adapter-postgres`](https://www.npmjs.com/package/@cyguin/changelog-adapter-postgres) | `0.1.10` | [`cyguin/changelog`](https://github.com/cyguin/changelog) | Postgres adapter for changelog storage. |

### Showcase

[`cyguin/npm-suite-demo`](https://github.com/cyguin/npm-suite-demo) is the standalone demo site for the suite. It mounts the published React packages into one cyguin-branded Vite app and uses browser-side mock API endpoints so every widget can be exercised without provisioning a database.

The demo currently covers:

- waitlist form and demo count
- notification bell and unread state
- announcement banner
- consent banner
- feedback widgets
- survey modal
- docs widget
- sniplet create/view flow
- changelog badge and release feed
- `@cyguin/claude-context-gen` CLI preview

---

## AI/dev tooling

| Package | Current | Repo | What it does |
|---|---:|---|---|
| [`@cyguin/claude-context-gen`](https://www.npmjs.com/package/@cyguin/claude-context-gen) | `2.0.1` | [`cyguin/claude-context-gen`](https://github.com/cyguin/claude-context-gen) | Interactive CLI that generates `CLAUDE.md` and `AGENTS.md` context files for AI coding assistants. |

---

## Other repos

| Repo | Notes |
|---|---|
| [`cyguin/marginkit-landing`](https://github.com/cyguin/marginkit-landing) | Landing page work. |
| [`cyguin/PlugScope`](https://github.com/cyguin/PlugScope) | Product repo. |
| [`cyguin/cronguardian`](https://github.com/cyguin/cronguardian) | Cron monitoring work. |
| [`cyguin/test-pipeline`](https://github.com/cyguin/test-pipeline) | Pipeline test repo. |

---

## Direction

The near-term focus is making the npm suite feel like one product:

- consistent `@cyguin/*` package metadata, README structure, licensing, and GitHub repo conventions
- dark-by-default cyguin UI skins with explicit light-mode opt-in
- self-hosted Next.js handlers and adapters where data is involved
- a single demo site that stays current with the latest published npm versions
- clearer install paths for teams that want to own their data first and consider managed services later

---

<div align="center">

[![npm](https://img.shields.io/badge/npm-%40cyguin-FFD700?style=for-the-badge&logo=npm&logoColor=000)](https://www.npmjs.com/org/cyguin)&nbsp;
[![Website](https://img.shields.io/badge/cyguin.com-FFD700?style=for-the-badge)](https://cyguin.com)&nbsp;
[![Demo repo](https://img.shields.io/badge/npm%20suite%20demo-FFD700?style=for-the-badge)](https://github.com/cyguin/npm-suite-demo)

</div>
