# SWG Remastered

SWG Remastered is a free, fan-run revival of Star Wars Galaxies (NGE era) built on the SWG-Source server codebase. The goal is a living, evolving galaxy -- hand-crafted questing and exploration, balanced solo and small-group combat, and a working player economy -- built right, not rushed. No pay-to-win, no wipe threats, no corporate timeline.

---

## Repositories

| Repo | What it is |
|---|---|
| [swgr-server](https://github.com/swgremastered/swgr-server) | Game server (SWG-Source fork). Containerized, Ubuntu 24.04, Oracle Free 23ai. CI builds the cluster image on every push to main. |
| [swgr-launcher](https://github.com/swgremastered/swgr-launcher) | Rust launcher. Handles patch delivery, channel switching (stable/beta), and client launch. |
| [swgr-auth](https://github.com/swgremastered/swgr-auth) | Authentication service. Cloudflare Workers + D1 + KV. Argon2id, device-bound sessions, MFA-ready. |
| [swgr-website](https://github.com/swgremastered/swgr-website) | swgremastered.com. Cloudflare Workers static site. |
| [swgr-ops](https://github.com/swgremastered/swgr-ops) | Infrastructure, CI/CD pipelines, planning docs, runbooks, monitoring config. |
| [swgr-client-tools](https://github.com/swgremastered/swgr-client-tools) | SWG client source fork (VS2022, win32). Builds SWGRemasteredClient.exe. |

---

## Play

- **Download:** grab the launcher from [swgr-launcher releases](https://github.com/swgremastered/swgr-launcher/releases)
- **Status:** [status.swgremastered.com](https://status.swgremastered.com)
- **Website:** [swgremastered.com](https://swgremastered.com)

---

## Dev Setup

See [swgr-ops wiki](https://github.com/swgremastered/swgr-ops/blob/main/wiki/README.md) for the full docs. Start with [RUNBOOK](https://github.com/swgremastered/swgr-ops/blob/main/wiki/ops/RUNBOOK.md) for provisioning and [ROADMAP](https://github.com/swgremastered/swgr-ops/blob/main/wiki/strategy/ROADMAP.md) for where we're headed.

Two galaxies are live: **Eclipse** (prod) and **Starsider-PTR** (staging). All content changes go through staging first before promotion to prod.
