# Changelog — timbogp marketplace

Marketplace-wide and cross-cutting changes only: the catalog itself, repo-level conventions, and general decisions. **Per-plugin changes live in each plugin's own changelog:**

- `agentic-study-environment` → [`plugin/agentic-study-environment/CHANGELOG.md`](plugin/agentic-study-environment/CHANGELOG.md)
- `ux-design` → [`plugin/ux-design/CHANGELOG.md`](plugin/ux-design/CHANGELOG.md)

Format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

## Versioning

Each plugin is versioned and released **independently**, tagged `<plugin>-vX.Y.Z` (e.g. `agentic-study-environment-v0.3.0`, `ux-design-v0.2.0`). The historical repo-wide tags [`v0.1.0`](https://github.com/TimboGP/timbogp-marketplace/releases/tag/v0.1.0) and [`v0.2.0`](https://github.com/TimboGP/timbogp-marketplace/releases/tag/v0.2.0) predate the split and correspond to `agentic-study-environment` releases (the repo's only plugin at the time). The marketplace catalog itself is not separately versioned.

## 2026-06-23

- **Coding-agent parity rule.** Added a *Coding-agent parity* directive to the canonical AI instructions ([`AGENTS.md`](AGENTS.md)) and the human contributor guide ([`CONTRIBUTING.md`](CONTRIBUTING.md)): any capability added for one named coding agent (currently **Claude Code** and **Codex**) must ship for the other in the same change — manifests, marketplace catalogs, capabilities, and docs move together.
- **Migrated to per-plugin changelogs.** Plugin-specific history moved out of this file into `plugin/<name>/CHANGELOG.md`; the root changelog now tracks only marketplace-wide and cross-cutting changes. Adopted per-plugin release tags (`<plugin>-vX.Y.Z`) while keeping the historical repo-wide `v*` tags.
- **Renamed the repository** `agentic-study-environment` → `timbogp-marketplace`; updated changelog links to the new URL.

## 2026-06-22

- **Restructured the repository README into a marketplace overview.** The root [`README.md`](README.md) now introduces the `timbogp` marketplace and both plugins (with install commands and links) rather than documenting the study harness directly. The harness's full content — transcripts, the `.studyenv/` layout, getting-started, FAQ, and limitations — now lives in its own plugin README at [`plugin/agentic-study-environment/README.md`](plugin/agentic-study-environment/README.md).
- **Added the `ux-design` plugin to the catalog** as the marketplace's second plugin. See its changelog for details.
