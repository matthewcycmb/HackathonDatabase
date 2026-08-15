---
description: Research a hackathon's judges with BrowserOS Neo and generate ranked hardware×emotion angles
argument-hint: <hackathon-url>
---

Build a judge dossier for the hackathon at: $ARGUMENTS

Rules: public professional info only (LinkedIn bios, talks, Devpost history, company pages — no personal digging). Every fact must come from a page you actually opened; cite the URL. No fabrication — mark unknowns as unknown.

1. Load BrowserOS Neo tools via ToolSearch ("select:mcp__browseros-neo__navigate,mcp__browseros-neo__read,mcp__browseros-neo__grep,mcp__browseros-neo__tabs,mcp__browseros-neo__name_session"). name_session "dossier <event>". Open your own tabs.
2. From the event site: theme, tracks, prizes, sponsors, and the judges/mentors list. Judges often appear late — if none are listed yet, dossier what exists (sponsors + past-year judges) and mark it PRELIMINARY.
3. Per judge: past companies, what they built, where they're from/based, causes and interests they publicly champion, and infer their likely judging lens.
4. Read `inventory/parts.md` (what we can build) and every `events/*/retro.md` (what we've learned).
5. Write `events/<slug>/dossier.md` using `events/_templates/dossier.md`: end with 3 ranked hardware×emotion angles, each scored against the SPECIFIC judges by name, feasible in 24h with owned parts.
6. Commit ("dossier: <slug>").
