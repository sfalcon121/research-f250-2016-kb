# Instructions for AI agents working in this repo

This is a **research area** for future AI agents: a curated knowledge base for repairing a 2016 Ford F-250 Super Duty (6.2L gas, 6R140).

## Start here
1. Read `README.md` (file map and confidence tags: [OM] [TSB] [FIELD] [VERIFY]).
2. Read `AGENT_SYSTEM_PROMPT.md` for the operating rules of the repair agent.
3. Read `99_Sources_Gaps_and_Expansion.md` for known gaps and what to research next.

## Conventions
- Keep every claim tagged with its confidence level. Never upgrade [FIELD]/[VERIFY] to [OM]/[TSB] without a source.
- Torque specs on safety parts must stay [VERIFY] until confirmed in the Ford Workshop Manual.
- Raw source data lives in `sources/nhtsa/` (JSON). Generated files (e.g. `04_*`) should be regenerated, not hand-edited.
- Record new gaps and sources in `99_Sources_Gaps_and_Expansion.md`.

## Not in git
Ford's owner's manual PDFs and text extractions (`sources/ford_official/`) are copyrighted and excluded via `.gitignore`.
Download them from Ford's owner site if you need to re-verify [OM] claims.
