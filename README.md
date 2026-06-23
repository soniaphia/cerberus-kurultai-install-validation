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
- llama.cpp and the specified 9B Q4_K_M local model are installed. Direct local inference passed. Tolui is configured for the local endpoint but Hermes response-structure compatibility still needs follow-up before tool-bearing work.
- No cron jobs were created from missing private scripts.

## Human-gated or pending

- OpenAI Codex OAuth/login.
- Replace the local Telegram placeholders with the real credential, then run gateway setup and foreground smoke tests.
- A separate Ogedei bot credential, if the operations gateway is wanted.
- QMD installation and `qmd update -c brain` / `qmd embed -c brain`.
- Start the local llama.cpp endpoint when Tolui is needed and resolve Hermes `final_response` compatibility.
- Review/install missing private or external Kurultai skills and cron scripts.

No secrets, real tokens, chat IDs, OAuth files, cookies, private Brain contents, Hermes sessions, or runtime databases are included in this repository.

