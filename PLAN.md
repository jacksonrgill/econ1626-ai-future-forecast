# Project Plan: AI & The Accounting Industry — 2030 Forecast

**ECON1626 Assessment 3 | Jackson Gill**

---

## Thesis

By 2027–2030, AI will bifurcate the accounting and financial advisory industry: compliance-heavy commodity work (bookkeeping, tax preparation, payroll, basic audit) will be largely automated, concentrating productivity gains in large firms and platforms. The advisory relationship becomes more valuable but harder to access at the mid-tier. Without active policy, this reinforces market concentration and locks displaced junior accountants out of the transition.

---

## Format: Choose Your Own Adventure

The reader selects a character and navigates three policy decision points. Choices accumulate to determine one of three 2030 endings. Each ending shows both the industry outcome and the personal outcome for the chosen character.

---

## Characters

| Character | Role | Stake |
|---|---|---|
| **Sam** | Junior accountant, 3 yrs in tax compliance, mid-tier firm, $65k | Am I about to be automated out of a job? |
| **Rachel** | Managing partner, 12-staff regional firm, 20 years in industry | Can my firm survive against Big 4 AI? |
| **James** | Policy advisor, Treasury | What do I recommend, and what if I'm wrong? |
| **Priya** | CFO of mid-sized construction company | Do I adopt AI tools and cut my accounting team? |
| **Marcus** | Big 4 partner, AI making his team more productive | I'm winning — but for how long? |

---

## Story Structure

### Prologue (no choice)
- Scene-setting: 2024, AI is reshaping accounting
- Task automation probability chart (Frey & Osborne anchor: ~94% for accountants)
- Key capabilities: LLM document processing, ML audit sampling, automated bookkeeping platforms

### Chapter 1 — The Adoption Wave
**Event:** Major platforms (Xero, QuickBooks, MYOB) roll out AI. Big 4 deploy internal tools.

**Choice:**
- A) Fast-track AI adoption (government tax incentives for AI investment)
- B) Wait and see (no active adoption policy)

**Data shown:** AI capability timeline 2022–2024, task displacement by role

### Chapter 2 — The Displacement
**Event:** Bookkeeper and junior accountant roles declining. Retraining is expensive and slow.
*(Charts adjust severity based on Chapter 1 choice)*

**Choice:**
- A) Launch reskilling fund (levy on platform revenue)
- B) Market-led retraining (some workers retrain independently)
- C) No coordinated response

**Data shown:** Employment projections by role, wage polarisation chart

### Chapter 3 — The Concentration Problem
**Event:** Xero/Intuit capture 70%+ of SME accounting market. Small practices squeezed out.

**Choice:**
- A) Mandate open APIs — level the playing field
- B) Let the market consolidate

**Data shown:** Market share by firm size, concentration index

### Endings (determined by policy score from choices)

| Score | Ending | World |
|---|---|---|
| 3 strong policy choices | Upside 2030 | AI democratised advisory, small practices survive, displaced workers retrained |
| 1–2 mixed choices | Baseline 2030 | Moderate disruption, growing inequality, muddling through |
| 0 policy choices | Downside 2030 | Concentration, displacement, advice becomes a luxury |

Each ending includes:
- Industry outcome (employment, market structure, consumer access)
- Character-specific personal outcome
- "What the economics says" explainer (mechanisms: so-so automation, task framework, concentration)
- Side-by-side comparison of all three worlds
- "Try again" button

---

## Economic Mechanisms

1. **Task substitution** (Autor et al. 2003): routine cognitive tasks — data entry, reconciliation, basic tax — are codifiable and automatable without eliminating the occupation wholesale
2. **Augmentation** (Brynjolfsson et al.): AI raises productivity of senior advisors; within-occupation divergence widens
3. **So-so automation** (Acemoglu & Restrepo 2019): productivity gains insufficient to trigger strong reinstatement effect; labour displaced without equivalent new task creation
4. **Market concentration**: firms with compute/data advantages (Big 4, platforms) capture disproportionate gains; compounding over time

---

## Scenarios — Parameter Table

| Driver | Upside | Baseline | Downside |
|---|---|---|---|
| Adoption speed | Fast, broad | Gradual, uneven | Fast, concentrated |
| Policy strength | Proactive (all 3 levers) | Reactive | Minimal |
| Bookkeeper employment (2030 vs 2024) | −10% | −20% | −35% |
| Senior advisor employment | +20% | +8% | +2% |
| Small practice market share change | Stable | −12% | −25% |
| Consumer access to advice | Improved | Slight improvement | Worsened |

---

## Policy Levers

1. **Adoption incentives** — shape speed and distribution of AI uptake
2. **Reskilling fund** — levy on platform revenue finances portable credentials for displaced workers
3. **Open API mandates** — prevent platform lock-in, allow small practices to access AI tools
4. **AI advice liability framework** — define when AI-generated advice requires human sign-off
5. **Competition & merger review** — updated criteria for AI-specific market power

---

## Interactive Elements

1. **Character select screen** — 5 cards, name/role/stake/difficulty indicator
2. **Task automation chart** — horizontal bar, 10 accounting sub-tasks by automation probability (Chart.js)
3. **Chapter narrative** — character-voiced text updates per choice, smooth transitions
4. **Employment projection chart** — updates live as choices are made
5. **Market share diagram** — before/after stacked bar by scenario
6. **Ending comparison table** — all three worlds side by side

---

## Data Sources

| Source | Use |
|---|---|
| Frey & Osborne (2013) | Automation probability anchor (~94% for accountants) |
| BLS Occupational Outlook: Accountants & Auditors | US employment projections 2022–2032 |
| ACCA (2019) *Professional Accountants: The Future* | AI adoption survey data |
| McKinsey Global Institute (2023) | % of accountant tasks susceptible to generative AI |
| Goldman Sachs (2023) | Professional services task automation estimates |
| IBISWorld: Accounting Services Australia | Industry revenue, firm count, employment |
| Acemoglu & Restrepo (2019) | So-so automation framing |
| Autor, Levy & Murnane (2003) | Task framework: routine vs non-routine |
| OECD (2023) | AI and labour market employment outlook |

---

## Technical Stack

- Single self-contained `forecast.html` — all CSS and JS inline
- Chart.js v4 (CDN) for all charts
- Vanilla JavaScript state machine for choice tracking
- CSS custom properties for theming (dark navy + amber accent)
- Smooth transitions between chapters
- Mobile responsive via CSS flexbox/grid
- Renders directly on GitHub Pages — no build step

---

## Commit Plan (target 12+ meaningful commits)

1. `init: scaffold repo with README and PLAN`
2. `feat: add forecast.html base structure and CSS theme`
3. `feat: add character select screen (5 characters)`
4. `feat: add prologue section with task automation chart`
5. `feat: add chapter 1 — adoption wave with choice logic`
6. `feat: add chapter 2 — displacement with dynamic employment chart`
7. `feat: add chapter 3 — concentration problem`
8. `feat: add upside 2030 ending with character outcomes`
9. `feat: add baseline and downside 2030 endings`
10. `feat: add scenario comparison table and try-again flow`
11. `feat: add methods, data, and references section`
12. `fix: mobile responsiveness and cross-browser polish`
13. `docs: update README with GitHub Pages link`

---

## Rubric Alignment

| Criterion | How this plan addresses it |
|---|---|
| Economic analysis & forecasting (30%) | Explicit task-level mechanisms, so-so automation framing, parameterised scenarios with named drivers |
| Policy scenarios & governance (20%) | 3 scenarios, 4 policy levers, each with trade-offs and KPIs, mapped to character outcomes |
| Evidence, data & methods (15%) | Named sources with specific claims, explicit assumptions log, uncertainty section |
| Communication & design (15%) | Interactive narrative, character-driven stakes, charts update with choices |
| Technical implementation (20%) | Single-file HTML, GitHub Pages, 12+ meaningful commits, reproducible |
