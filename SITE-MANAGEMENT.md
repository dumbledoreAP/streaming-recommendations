# SITE-MANAGEMENT.md — Streaming Recommendations

## Site
- Live: https://dumbledoreap.github.io/streaming-recommendations/
- Repo: https://github.com/dumbledoreAP/streaming-recommendations
- Clone: /root/.openclaw/workspace/streaming-recommendations

## When Jeff says "I watched X"
Follow this procedure exactly:

1. **Identify the show** in the site data (index.html or data.json) — note which service it belongs to
2. **Remove it** from the active list
3. **Research a replacement** — same service, same criteria (no horror, no reality). Do a quick web search to confirm IMDb rating and that it's available on that service in Australia
4. **Add the new show** to the same service section
5. **Add the watched show** to the "Recently Watched" section at the bottom of the page
6. **Commit and push** to main — GitHub Pages redeploys automatically
7. **Confirm to Jeff** — tell him what was removed and what replaced it

## Content Rules
- No horror, no reality TV
- Verify IMDb rating via web search or IMDb page
- Confirm the show is actually available on that Australian streaming service
- Keep per-service count consistent (currently 8 per service, 10 for Apple TV+)
- Genre icon + genre label + IMDb badge + season count for every entry

## Updating the Data
After Phase 1 refactor, data lives in `data.json` and is rendered by JS in `index.html`. Edit the JSON, push, done.
