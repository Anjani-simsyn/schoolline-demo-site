# SchoolLine AI · Connected Learning Communities

Website for the SIPL x Uniconnect AI Hackathon 2026 finale (Team Data Dragons).

- `index.html` is the judge-facing page: problem, solution, the 10-minute live demo, build status, the full solution blueprint (data model, roles and access, channels, AI agents, 24 workflows, campaigns, integrations, dashboards), build plan, go-to-market and FAQ.
- `runbook.html` is for the team only (run sheet, fallbacks, who plays whom, pre-show checklist). It is not linked from `index.html`.
- `styles.css` is shared by both pages.

## Run locally

No build step. Serve the folder and open http://localhost:8000:

    python -m http.server 8000

Blueprint tabs can be linked directly, e.g. `index.html#p-wf` (workflows), `#p-access`, `#p-agents`.

## Edit

All in the `<script>` block at the bottom of `index.html`:

- Build status cards: `ITEMS` (`s` is `live`, `testing`, `build` or `roadmap`).
- Demo scenes: `SCENES`.
- CRM modules and fields: `MODULES`. Permission matrix: `MATRIX`.
- WhatsApp templates: `TEMPLATES`. AI agents: `AGENTS`. Workflows: `WF`.
- FAQ: `QA`.
- Pre-show checklist: `CHECKS` in `runbook.html`.
- Colours: the `:root` tokens at the top of `styles.css` (navy `#0B1E30`, yellow `#F6C451`).
