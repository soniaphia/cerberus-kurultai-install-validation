# Cerberus Kurultai installation validation

Sanitized validation receipts for a local installation of [Kurultai](https://github.com/Danservfinn/kurultai).

- Kurultai commit: `ae4eda273e2a1a5d797afc258f97f9b726bab375`
- Platform: macOS 26.4, Apple Silicon (`arm64`)
- System Python used by Kurultai installer: Python 3.9.6
- Hermes: v0.17.0 (2026.6.19), managed Python 3.11.15
- Brain root: `~/brain`
- User-visible chair name: `Cerberus`
- User-visible bot name: `Cerberus Bot`
- Internal Hermes chair profile ID: `kublai` (retained for compatibility)

## Validated state

- Hermes installed and its config migrated to schema v30.
- Frontier settings staged as `openai-codex` / `gpt-5.5`, 1,000,000 context, compression enabled at `0.25`.
- Eleven Kurultai profiles created: `kublai`, `batu`, `chagatai`, `jochi`, `temujin`, `coder`, `mongke`, `ogedei`, `subc`, `tolui`, and `codex`.
- Brain Markdown/receipt tree created successfully.
- Native Hermes Kanban initialized; a harmless create/complete smoke task passed.
- 71 bundled Hermes skills are installed. Kurultai's private/external skill manifest remains a reconciliation follow-up.
- llama.cpp and the specified 9B Q4_K_M local model are installed. Direct inference and a Hermes Tolui one-shot both passed at 65,536 context using Q8 KV cache and one server slot on the 16 GB host.
- QMD v2.5.3 is installed. The `brain` collection contains 6 indexed Markdown files and 8 embedded chunks; a collection-scoped search passed.
- Hermes's Telegram dependency (`python-telegram-bot` 22.6) is installed and the adapter/configuration preflight passes with secure DM pairing.
- No cron jobs were created from missing private scripts.

## Human-gated or pending

- OpenAI Codex OAuth/login.
- Replace the local Telegram placeholders with the real credential, then run gateway setup and foreground smoke tests.
- A separate Ogedei bot credential, if the operations gateway is wanted.
- Start the local llama.cpp endpoint with at least 65,536 context when Tolui is needed.
- Review/install missing private or external Kurultai skills and cron scripts.

No secrets, real tokens, chat IDs, OAuth files, cookies, private Brain contents, Hermes sessions, or runtime databases are included in this repository.
