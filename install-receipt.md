# Installation receipt

Date: 2026-06-22

Kurultai was installed locally from commit `ae4eda273e2a1a5d797afc258f97f9b726bab375`.

## Result

- Chair display name: `Cerberus`
- Chair bot display name: `Cerberus Bot`
- Operator: `Sophia`
- System: `Sophia Kurultai`
- Internal chair profile: `kublai` (not renamed)
- Brain: created successfully at `~/brain`
- Hermes: installed and configured; provider authentication remains human-gated
- Telegram: placeholder-only private profile config; no live credential used
- Gateways: not started or installed as services
- Telegram runtime: `python-telegram-bot` 22.6 installed; offline adapter/configuration preflight passed
- QMD: v2.5.3 installed; Brain collection update/embed/search passed
- Kanban: initialized and smoke-tested
- Local model: direct inference and Hermes/Tolui one-shot passed at 65,536 context; tool-bearing work remains intentionally unverified

## Security boundary

This public receipt contains only sanitized paths, generated non-secret identity data, command summaries, and reconciliation metadata. It excludes `.env` files, credentials, chat IDs, OAuth state, sessions, private Brain content, and runtime databases.
