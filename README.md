# STS / CORA — CustomGPT.ai Betty-displacement demo

Sales demo replica for **The Society of Thoracic Surgeons**. Not affiliated with or endorsed by STS.

## Three surfaces (required)

1. **Floating live chat** — `js/main.js` loads `chat.js` using `DEMO_CONFIG.p_id` / `p_key`
2. **Full-page assistant** — hero button **"Try CORA AI assistant"** → `assistant.html` (embed.js)
3. **Header SGE search** — AI search bar → dropdown `#customgpt_search` via `sge.js`

## Open locally

```bash
cd /workspace/betty-demos/sts/demo-site
python3 -m http.server 8080
```

Then open http://localhost:8080/ (and http://localhost:8080/assistant.html).

## Wire agents

Edit `config.js` and replace `PENDING` with public embed keys:

- `p_id` / `p_key` — chat agent (floating bubble + assistant.html)
- `search_p_id` / `search_p_key` — search/SGE agent

Or pass query overrides: `?p_id=...&p_key=...&search_p_id=...&search_p_key=...`

## CTA URL notes

- Provisional: https://www.sts.org/membership
- Provisional: https://www.sts.org/meetings
- Provisional: https://www.sts.org/education
- Research path: https://www.sts.org/education/education/cora-your-cardiothoracic-online-resource-assistant
- Homepage seed: https://www.sts.org/

## Brand

Primary: `#005C8A` · Accent: `#00A3A1` · Seed: https://www.sts.org/
