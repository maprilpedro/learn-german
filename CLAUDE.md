# learn-german — Project Rules

## Purpose

This repo is Pedro's structured German language knowledge base, ingested from **Hammer's German Grammar and Usage, 5th Ed.** (Martin Durrell, Routledge 2011).

**PDF path:** `/Users/pedrofer/Library/CloudStorage/GoogleDrive-maprilpedro@gmail.com/My Drive/CalibreLibraryMain/5th Ed ( PDFDrive )/Hammer's GERMAN Grammar and Usage (2257)/Hammer's GERMAN Grammar and Usage - 5th Ed ( PDFDrive ).pdf`

---

## Domain Structure

| Domain | Folder | Book chapters |
|---|---|---|
| Grammar | `german/grammar/` | Ch. 1–9, 11, 15–16, 19–21, 23 |
| Verbs | `german/verbs/` | Ch. 12–14, 17–18 |
| Vocabulary | `german/vocabulary/` | Scattered throughout |
| Modal Particles | `german/modal-particles/` | Ch. 10 |

---

## When Helping Pedro with German

1. **Before answering**, check the relevant domain `rules.md` for existing rules
2. **Apply `rules.md` entries by default** — don't re-explain confirmed rules, just apply them
3. **After any German task or ingestion**, extract new insights into the appropriate domain file and commit
4. **Flag contradictions** to existing rules immediately — demote the rule to `hypotheses.md`

---

## When Ingesting a New Chapter

- Read PDF pages directly in the main conversation (do NOT use background agents — Pedro needs to verify quality)
- If the PDF tool returns cached results, ask Pedro to share screenshots
- Map each chapter to a domain (grammar / verbs / vocabulary / modal-particles)
- Extract into `knowledge.md` first; promote to `rules.md` only what is clearly prescriptive
- Note register labels from the source (formal, colloquial, archaic, regional)

---

## Knowledge Architecture Rules

Each domain follows the same pattern:
- `knowledge.md` — facts, patterns, examples from the source
- `rules.md` — confirmed prescriptive rules to apply by default
- `hypotheses.md` — nuances needing more exposure before promotion

Promote a hypothesis to rule after 3+ confirmations.
Demote a rule to hypothesis if contradicted by new data.

---

## Git Workflow

- Remote: `https://github.com/maprilpedro/learn-german.git`
- Always push after significant ingestion sessions
- Use `gh auth switch --user maprilpedro` before any `gh` commands; switch back to `pedrofer_adobe` after
