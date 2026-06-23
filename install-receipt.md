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
- Hermes: installed and configured; OpenAI Codex authentication active
- Telegram: real credential stored only in private profile-local configuration
- Gateways: Cerberus/Kublai gateway installed as a macOS LaunchAgent and running
- Telegram runtime: `python-telegram-bot` 22.6; identity validation, polling connection, outbound delivery, allowlisted inbound `/status`, and response passed
- QMD: v2.5.3 installed; Brain collection update/embed/search passed
- Kanban: initialized and smoke-tested
- Local model: direct inference and Hermes/Tolui one-shot passed at 65,536 context; tool-bearing work remains intentionally unverified

## Security boundary

This public receipt contains only sanitized paths, generated non-secret identity data, command summaries, and reconciliation metadata. It excludes `.env` files, credentials, chat IDs, OAuth state, sessions, private Brain content, and runtime databases.

The active Cerberus credential should be rotated because it was shared through a chat channel. The replacement must remain in private local configuration only.
