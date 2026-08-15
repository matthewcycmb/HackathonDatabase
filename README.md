# HackathonDatabase

One place for the whole hackathon pipeline: find events → research judges → pick a hardware×emotion angle → win → retro → repeat.

## The three systems

1. **Radar** (`radar/`) — a scheduled cloud agent scans Devpost, Luma, MLH, and UBC/SFU/BCIT pages twice daily for Metro Vancouver hackathons, flags high-school eligibility (✅/⚠️/❓), and pushes to Telegram **only when something changed** (new event, registration opens, deadline <7 days) plus a Sunday heartbeat. State lives in `radar/state.json`.
2. **Judge dossiers** (`events/`) — run `/dossier <hackathon-url>` on the laptop (uses BrowserOS Neo). Produces `events/<slug>/dossier.md`: judges' public backgrounds → 3 ranked hardware×emotion project angles. After each event run `/retro <slug>`; future dossiers read all past retros.
3. **Hardware** (`hardware/`) — analysis of verified prize-winning hardware projects (Aug 2025–Aug 2026) and the tiered Apliu Street shopping checklist. `inventory/parts.md` maps owned parts → buildable archetypes.

## Status / TODO

- [ ] Telegram bot token not yet wired (paste token → goes into radar routine env)
- [ ] Radar cloud schedule not yet created (blocked on token)
- [ ] Hardware winners analysis in progress
