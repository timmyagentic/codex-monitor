# CodexMonitor

A macOS menu-bar app for tracking **Codex** and **Claude Code** usage — live quota meters, rolling spend, session-level drilldown, and burn-rate projections.

> **This is a branded release mirror of [quota-monitor](https://github.com/systemoutprintlnnnn/quota-monitor).**
> All development happens there. This repo only hosts branded releases under the **CodexMonitor** name.

## Download

Grab the latest `CodexMonitor-<version>.dmg` from the [Releases page](https://github.com/systemoutprintlnnnn/codex-monitor/releases).

## Install

1. Open the DMG, drag **QuotaMonitor.app** onto the **Applications** alias.
   *(The .app bundle name stays `QuotaMonitor.app` internally — this is intentional for auto-update continuity.)*
2. **First launch only** — macOS will refuse to open the app directly:
   - **Right-click** `QuotaMonitor.app` → **Open** → click **Open** in the Gatekeeper dialog.
   - Or: `xattr -dr com.apple.quarantine /Applications/QuotaMonitor.app`

## What it does

- **Menu bar popover** — live 5h / 7d quota rows, rolling 30-day spend, session counts.
- **Dashboard** — Forecast (burn rate + projected exhaustion), Trends, Composition.
- **Sessions & History** — searchable per-session and per-day usage breakdowns.
- **Settings** — language (English / 简体中文), Codex poll interval, Claude Keychain policy, CSV export, pricing catalog, and more.

Languages: English (default) and 简体中文, hot-swappable at runtime.

## Why two repos?

- **[quota-monitor](https://github.com/systemoutprintlnnnn/quota-monitor)** — the source repo with all code, issues, and PRs.
- **codex-monitor** — a release-only mirror that publishes the same app under the CodexMonitor brand.

Both are built from identical source code in a single CI pipeline. Features, bug fixes, and contributions all go to [quota-monitor](https://github.com/systemoutprintlnnnn/quota-monitor).

## License

[MIT](LICENSE) © 2026 tjzhou.
