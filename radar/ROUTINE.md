# Hackathon Radar — cloud routine prompt

Run twice daily (08:00 and 20:00 America/Vancouver). You are scanning for hackathons a Vancouver high-school student can enter. Never invent events — every reported event must come from a page you actually fetched, with its URL.

## Sources to scan (headless: WebFetch / WebSearch / firecrawl)
- https://devpost.com/hackathons — search "Vancouver", also upcoming BC events
- https://lu.ma — search "hackathon Vancouver"
- https://mlh.io/seasons/2026/events and /2027/events — filter British Columbia
- Known recurring events' own sites: nwHacks (UBC), StormHacks (SFU), HackCamp (UBC), cmd-f, Hack the North is NOT local (skip unless asked), BCIT events page
- Eventbrite: search "hackathon" in Vancouver, BC

## Scope rules
- Metro Vancouver, in-person (Vancouver, Burnaby, Surrey, Richmond, UBC, SFU, BCIT)
- Skip online-only and non-BC events
- For each event capture: name, dates, venue, registration URL, registration open/close, eligibility
- Eligibility flag: ✅ high-schoolers explicitly allowed · ⚠️ post-secondary only · ❓ unclear (say what the page said)

## State + alert policy
State file: `radar/state.json` in this repo, keyed `"<event-slug>-<year>"` with `{name, url, dates, reg_deadline, eligibility, first_seen, last_status, alerted}` fields.

Send a Telegram message ONLY when:
1. An event key is new since last scan → "🆕 New hackathon: …"
2. Registration opened since last scan → "🟢 Registration open: …"
3. A registration deadline is <7 days away and no countdown alert was sent yet → "⏰ 5 days left: …"
4. It is Sunday and no heartbeat was sent this week → "📡 Weekly radar: N tracked events" + one-line list

Otherwise send nothing. Update `state.json` and commit+push ("radar: scan YYYY-MM-DD HH:MM") every run, even silent ones.

## Telegram send
```
curl -s "https://api.telegram.org/bot${TELEGRAM_BOT_TOKEN}/sendMessage" \
  -d chat_id="${TELEGRAM_CHAT_ID}" -d parse_mode=Markdown --data-urlencode text="..."
```
TELEGRAM_BOT_TOKEN and TELEGRAM_CHAT_ID come from the routine's environment (not committed to the repo).
