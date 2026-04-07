---
name: PDF Ingestion — Do It Directly, Not in Background Agents
description: Pedro wants PDF ingestion done directly in the main conversation so he can verify correctness, not via background agents
type: feedback
---

Do not launch background agents for PDF book ingestion.

**Why:** Pedro stopped background agents mid-session because he couldn't verify the correctness and quality of what was being written. He wants to see progress directly and confirm it's being ingested accurately.

**How to apply:** When ingesting a reference book chapter by chapter:
- Read PDF pages directly in the main conversation (or accept screenshots from user when PDF tool returns cached results)
- Write content to knowledge files immediately after reading each chapter
- The PDF Read tool often returns cached results after the first call — if that happens, ask the user to share screenshots instead

**Note:** Background agents are acceptable for truly independent work (e.g. modal particles Ch 10, which was a self-contained chapter Pedro wasn't actively reading). The problem was running multiple parallel agents on chapters Pedro was also trying to read and verify.
