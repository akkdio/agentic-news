# Agentic Commerce Tracker

A Cursor-native knowledge base for staying current on **agentic commerce**. Paste sources into chat; the agent saves, indexes, and answers with cited analysis from this corpus.

## How to use

1. Open this project in Cursor.
2. Paste an article, email digest, or notes into chat and say **“add this to the tracker”** (or “index this”).
3. Ask analysis questions, e.g.:
   - “What’s the latest on agentic commerce?”
   - “How do Visa and Mastercard compare on agent pay?”
   - “Refresh the brief”

## Layout

| Path | Role |
|------|------|
| `sources/` | Dated markdown intakes (one file per paste or digest) |
| `index/corpus.json` | Searchable metadata, summaries, and signals |
| `briefs/latest.md` | Rolling synthesis of the state of agentic commerce |
| `.cursor/rules/agentic-tracker.mdc` | Always-on ingest + query behavior |

## Source frontmatter

Each file under `sources/` should include:

- `id`, `title`, `date` (ISO), `added_at`, `source_type` (`email_digest` \| `article` \| `note` \| `url_paste`)
- `topics`, `entities`, optional `url`

Filename pattern: `YYYY-MM-DD-short-slug.md`

## Design note

v1 has no embeddings or separate chat UI. Retrieval is: read `index/corpus.json` → open matching `sources/` files → answer with citations. The corpus starts with the Nov 14, 2026 CRC Fintech Weekend Reads digest.
