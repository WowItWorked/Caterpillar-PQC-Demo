# Caterpillar Post-Quantum Cryptography (PQC) Readiness Dashboard

An interactive, single-page dashboard assessing Caterpillar Inc.'s readiness for the
transition to post-quantum cryptography — covering the company's own readiness profile,
a heavy-equipment peer benchmark, third-party / supply-chain exposure, the PQC regulatory
timeline, and a set of executive decision questions.

**▶ Live site:** _enable GitHub Pages to populate this link_ — `https://<user>.github.io/Caterpillar-PQC-Demo/`

## Views

- **Start here** — plain-language explainer of the quantum threat for executives
- **Overview** — KPIs, readiness gauge, peer benchmark and third-party exposure at a glance
- **Caterpillar profile** — readiness scored across six dimensions, with a migration roadmap
- **Peer benchmark** — estimated readiness vs. Komatsu, John Deere, Hitachi, Volvo CE, Liebherr
- **Third parties** — interactive exposure quadrant + filterable/sortable vendor register
- **PQC timeline** — milestones from the first NSA warnings to the 2030–2035 deadlines
- **Executive questions** — board-level prompts grouped by risk area

## How it works

This is a zero-build static site. `index.html` contains the design as a declarative
template; `support.js` is a small runtime that loads React from a CDN, compiles the
template, and renders it. There is nothing to install or build — open `index.html` over
HTTP and it runs.

Run locally:

```bash
python -m http.server 8000
# then open http://localhost:8000/index.html
```

> The fonts (Google Fonts), icons (Lucide), and React are loaded from public CDNs, so an
> internet connection is required to render.

## Important disclaimer

Post-quantum readiness is **not publicly disclosed** by the organizations shown here. All
scores are **analyst estimates** inferred from observable signals (public crypto posture,
NIST / CNSA alignment, cloud platforms, certifications, disclosures) and each carries a
stated confidence level. Use them as a directional planning aid — **not as audited fact**.
Nothing in this dashboard uses confidential or organization-supplied data.

## Files

- `index.html` — the dashboard (the live entry point)
- `Caterpillar PQC Readiness.dc.html` — original design source (identical to `index.html`)
- `support.js` — the rendering runtime
- `screenshots/` — reference captures of each view

---

Originally mocked up in [Claude Design](https://claude.ai/design) and exported as a handoff bundle.
