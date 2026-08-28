<div align="center">

# Diego Gallina

**Economics · quantitative finance research · applied AI**

Undergraduate in Economics & Business Administration — Fucape Business School
Business Development Specialist @ Wisers Information Limited (Hong Kong)
President @ Fucape Jr.

📍 Vitória, ES, Brazil

</div>

<br>

## About

I care most about the part of empirical work that decides whether a result is real: how the sample was built, what was chosen after looking at the data, and how much of the estimate survives the number of times you tried. Three years as a funded research assistant (Fapes/Ifes) got me into that habit; the projects since have been an attempt to hold myself to it in public.

The rest of my time goes to business development at Wisers — market intelligence and entry strategy for firms coming into Brazil, negotiating in English with stakeholders across Asia — and to Fucape Jr., where I led a restructuring that grew annual revenue **+500%**.

<br>

## Research

### [Benevente](https://github.com/diegogallina1/benevente) — reproducible factor investing on the Brazilian market

A pre-registered multifactor portfolio study on B3 (quality, value, momentum), built so that the methodology can be audited and the result can fail. `Python` · [benevente.dgo.fi](https://benevente.dgo.fi)

**Identification and sample construction**

- Price panel rebuilt from B3's COTAHIST so delisted firms stay in the universe — **survivorship bias removed**; the original panel was silently dropping 139 of 497 issuers. Delisting is liquidated at the last observable price, not recorded as a zero return.
- Fundamentals from CVM's official ITR/DFP filings, TTM on accumulated periods only, cut by filing-receipt date so no decision uses information unavailable in the January it was made.
- Costs, liquidity-dependent B3 fees and Brazilian capital gains tax modeled; buy-and-hold within the year rather than free daily rebalancing.

**Inference under multiple testing**

- **73 trials audited** with deflated Sharpe ratio and probability of backtest overfitting. The published rule's raw Sharpe does not survive the correction, and the repository says so.
- **Seven hypotheses tested and rejected are published in the same detail as the positive results** — including the one that mattered most: widening the configuration search from 36 to 256 candidates, with identical inputs, code and window, made the system *worse* (CAGR 15.31% → 12.68%; deflated Sharpe 0.957 → 0.777, below significance). With ten annual observations you cannot rank 256 candidates. The search was retired and replaced by a configuration **declared and frozen in advance with a public hash**.
- A 2026 self-audit found seven methodology defects. Every one of them had biased the results in the flattering direction — a benchmark that was accidentally the strategy itself, solvency metrics that were always null, a fixed 15bp cost assumption. All seven are documented in the README with their effect and their fix.

**What it does not claim**

The full 2015–2025 series is development sample: the factors, constraints and the decision to declare rather than search were all made while looking at that window. The project's own commercial-readiness gate returns `research_only`, and the reason is not the returns — it is that no frozen holdout exists. The confirmatory sample begins with the first trading day of 2027.

Two papers written up from the work: Fucape BTech 2026 and IEEE CIFEr 2027, with a single source of truth for every number in the manuscripts and SHA-256 manifests at each pipeline step.

<br>

### [SantaTeresa-Microclima-Lab](https://github.com/diegogallina1/SantaTeresa-Microclima-Lab) — microclimate analysis of Santa Teresa (ES)

Interdisciplinary collaboration with an environmental science student at Ifes: climatology of a mountain valley from INMET/INCAPER historical series — extremes, monthly rainfall concentration, humidity trend, and a logistic rainfall predictor. I handle ingestion, cleaning and modeling; my collaborator sets the environmental criteria and interprets the findings. `Python` `Jupyter` — in progress.

<br>

## Other public work

**[painel-criticos](https://github.com/diegogallina1/painel-criticos)** — four synthetic readers with distinct evaluation criteria critique a text (paper, thesis, valuation, CV), returning a score, the specific passages that bothered each one, and a revision. Next.js, Claude/Gemini API, Redis rate limiting, MIT. Live at [painel.dgo.fi](https://painel.dgo.fi).

<br>

## Applied work

**DSisCont** — Fucape Jr. Full accounting platform I designed and built from scratch: income statement and balance sheet (ROE/ROA), OFX bank reconciliation, NF-e invoice parsing, and LLM-based document classification that removed **~70%** of manual categorization. `React` `Electron` `TypeScript` `Python`

Also built and maintained privately: a WhatsApp scheduling agent on the Claude API with tool use, a clinic cash-flow and receivables dashboard, and a marketplace price-anomaly monitor. Happy to walk through any of them.

<br>

## Experience

```
2024 — present   Business Development Specialist · Wisers Information Limited
                 Cross-border market intelligence and expansion advisory
                 9 contracts closed · English-language negotiation across Asia

2025 — present   President · Fucape Jr.
                 Strategic restructuring · +500% annual revenue
                 Architected DSisCont end to end

2025 — 2026      Board member · Fucape Finance League
                 Governance · institutional immersion program in Brasília

2021 — 2024      Research assistant (funded) · Fapes / Ifes
                 Applied research and quantitative analysis
```

<br>

## Education & certifications

**B.A. Economics & Business Administration** — Fucape Business School, 2023–2027
100% merit scholarship for academic performance

IBM AI Engineering Professional Certificate · CEAV Virtual Asset Specialist · EF SET English C2 · Excel with AI (DIO)

<br>

## Toolkit

<div align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![R](https://img.shields.io/badge/R-276DC3?style=flat-square&logo=r&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat-square&logo=powerbi&logoColor=black)

</div>

<div align="center">
<sub>Portuguese (native) · English (C2) — open to research collaborations.</sub>
</div>

<br>

<div align="center">

<sub>DGO Foresight & Intel · AI, automation and advisory</sub>

</div>
