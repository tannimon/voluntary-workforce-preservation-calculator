![Voluntary Workforce Preservation Calculator — voluntary contribution scenarios with pay-equity analysis](assets/banner.png)

# Voluntary Workforce Preservation Calculator

*Voluntary contribution scenarios with pay-equity analysis.*

**Explore voluntary alternatives to workforce reductions through transparent financial modeling and equity analysis.**

A free, browser-based tool that models whether small, broadly shared contributions across a hospital workforce could reduce the need for layoffs, furloughs, or service cuts during periods of financial stress — evaluated by both financial impact and distributional fairness across income levels.

Everything runs client-side in a single HTML file. Nothing is entered, transmitted, or stored on any server.

> **What this is:** decision-support modeling for finance, HR, quality leaders, employees, and the people a program would affect.
> **What this is not:** legal, HR, or payroll advice, or an endorsement of any particular program. Figures are gross payroll estimates only.

---

## Why this tool exists

Hospitals across the U.S. are under sustained financial pressure from declining reimbursement, rising operating costs, and reductions in public funding. Because labor is typically a hospital's largest controllable operating expense, workforce reductions — hiring freezes, layoffs, furloughs, service cuts — often become the default response when revenue declines. Those reductions fall hardest on the people who deliver care.

This calculator explores one alternative. The goal is **not the savings** — it's preserving jobs, care teams, and institutional knowledge. Savings are simply the mechanism. It models whether many people making small, voluntary, transparent contributions could reduce the need to eliminate positions.

The calculator is intentionally designed to evaluate proportional burden-sharing across income levels. Every scenario includes equity measures, so the distribution of contributions is visible rather than assumed.

It advocates for no specific program. **Every modeled dollar should be weighed against the human cost of workforce reductions — this calculator exists to make those tradeoffs transparent, not to decide them.**

## What it does

- **Four contribution models** — percentage of hours (the proportional default), tiered by pay band, PTO donation, or flat minutes — so you can compare *how* the contribution is structured, not just how big it is.
- **A live fairness check.** Every scenario shows each role's contribution as a **share of its own pay**, and the multi-role view returns a plain 🟢 progressive / 🟡 proportional / 🔴 regressive verdict comparing lower-paid vs higher-paid staff. Flat minutes is available but flagged as least proportional.
- **Single-role, multi-role, and higher-earner views.** Model one role, a whole department roster, or the salaried/exempt population separately (where early clock-out legally can't apply).
- **FLSA-aware higher-earner handling.** Salaried exempt staff are modeled through PTO donation or a documented voluntary salary reduction — not partial-day docking, which risks exempt status.
- **Pay-equity analysis** built into every view, including proportional-contribution comparisons across pay levels.
- **FTE-equivalent translation.** Savings are also expressed as base-wage FTE-years, so the impact reads in the units leadership actually plans in.
- **Optional employer payroll-tax uplift.** Reduced wages also reduce the employer FICA match; toggle it on for a fuller picture. Off by default.
- **Editable deficit reference.** Set your organization's operating-loss figure to see each scenario's contribution in context — framed explicitly as one component of a broader recovery strategy, never as a standalone fix.
- **Shareable scenario links.** Any single-role scenario serializes into a URL — send a colleague a link that opens pre-configured. No files, no accounts, nothing stored.
- **Print-ready** for a one-page summary, and a "Show the Math" tab that lays out every formula and reference calculation.

## Design & accessibility

- **Zero dependencies, no build step.** One self-contained HTML file, vanilla JS. Open it in any browser; host it anywhere static.
- **Accessible by construction.** Semantic landmarks, a skip link, a full WAI-ARIA tablist with arrow-key navigation, associated labels on every control, visible focus states, and reduced-motion support.
- **Privacy by construction.** No network calls, no analytics, no storage. The math happens in front of you.

## Limitations (read these)

- Figures are **gross payroll estimates**. They do not model morale, turnover, recruitment cost, or care-delivery impact — all of which are real and can outweigh the savings shown.
- Voluntary salary reductions for exempt staff require **written agreements** and may carry state-level notice requirements. The tool flags this but is not a substitute for HR and legal review.
- Timekeeping systems (e.g. Symplr) may auto-refill early clock-out minutes from PTO/APL banks; a dedicated zero-pay code or the PTO-donation model may be required. The tool notes where this applies.
- Participation is assumed voluntary throughout. A program that is voluntary in name only is a different thing than what this models.

## Run it

Open `index.html` in any modern browser. Nothing else to install.

To host on GitHub Pages: enable Pages on the repo (Settings → Pages → deploy from `main`, root). The tool will be served at `https://<username>.github.io/workforce-preservation-calculator/`.

## Tech

Vanilla HTML / CSS / JavaScript · no framework · no build · no runtime dependencies · single file.

Part of **Tanni's Desk Tools** — a suite of PHI-free-by-construction, no-build clinical-quality and healthcare-operations tools.

## License

MIT — see `LICENSE`. This is a permissive license: anyone may use, modify, redistribute, or build on this code commercially, provided the copyright notice and license text are retained.

## Disclaimer

This software is provided for educational and decision-support purposes only. It does not constitute legal, human resources, payroll, labor relations, or financial advice. Organizations should consult appropriate legal, HR, payroll, and labor professionals before implementing any workforce program. Use of this software does not imply endorsement of any employment practice or policy.

All calculations are gross payroll estimates and do not account for morale, turnover, recruitment cost, or care-delivery impact. See `DISCLAIMER.md` for the full statement.
