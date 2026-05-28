# Auracelle Charlie v6.0

**AI Governance War Game Simulation Sandbox**

[![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc/4.0/)
[![BSU Doctoral Research](https://img.shields.io/badge/BSU-Doctoral%20Research-003D6B)](https://www.bathspa.ac.uk)
[![UC Berkeley CLTC](https://img.shields.io/badge/UC%20Berkeley-CLTC-003262)](https://cltc.berkeley.edu)
[![Framework](https://img.shields.io/badge/Framework-E--AGPO--HT%20v3.1-2d9d8e)](https://auracelle.github.io)
[![NATO STO SAS-219](https://img.shields.io/badge/NATO%20STO-SAS--219-003087)](https://www.sto.nato.int)

---

## Overview

Auracelle Charlie is a structured wargaming instrument for stress-testing AI governance policy. Participants negotiate a real-world governance scenario — currently **California Senate Bill 53 (2025), Transparency in Frontier AI Act** — through six adversarial rounds with five AI agents, two automated Red Team shocks, and a Policy Owner agent that issues governance challenges each round.

The instrument is designed for **autonomous participation**: a single participant can complete a full six-round session without a facilitator, generating structured research data for doctoral analysis at Bath Spa University under the E-AGPO-HT v3.1 measurement framework.

### Current Pilot Workshop Focus

- **Scenario:** Frontier AI — Catastrophic Risk & Safeguards
- **Validation Case:** TFAIA — California SB-53 (2025)
- **Use-Case Objective:** Whistleblower Protections
- **Information Regime:** Adversarial — Contested
- **Research Objective 3:** Assess how participant identity, professional experience, and affiliation shape policy negotiation outcomes

---

## Repository Structure

```
auracelle-charlie/
│
├── Auracelle_Charlie_Portalv7.html     # Single-file deployment — portal + simulation
│
├── docs/
│   ├── Auracelle_Charlie_Workshop_Instructions.docx   # Participant step-by-step guide
│   ├── Auracelle_Charlie_Pilot_Workshop.docx          # One-page workshop overview
│   └── participant-guide.md                           # Plain-text version of instructions
│
├── data/
│   └── .gitkeep                        # Participant JSON exports go here (not tracked)
│
├── assets/
│   └── .gitkeep
│
├── README.md                           # This file
├── CITATION.cff                        # Citation metadata
├── CONTRIBUTING.md                     # Contribution guidelines
├── LICENSE.md                          # CC BY-NC 4.0
├── SECURITY.md                         # Security policy
└── .gitignore                          # Excludes participant data and build artefacts
```

---

## Quick Start

### Participants

1. Download `Auracelle_Charlie_Portalv7.html`
2. Open in **Chrome or Firefox** (not Safari or Edge)
3. Enter your name, organisation, and access code: `CHARLIE2026`
4. Select your Sector and Gender Composition
5. Click **Watch the Demo** to see all eleven tabs demonstrated
6. Click **Launch Auracelle Charlie** to begin your session
7. Complete six rounds in Tab ② Facilitator Mode
8. Export your session JSON from Tab ② and email to the PI

Full instructions: see `docs/Auracelle_Charlie_Workshop_Instructions.docx`

### GitHub Pages Deployment

This repository is configured to serve `Auracelle_Charlie_Portalv7.html` directly via GitHub Pages. Once Pages is enabled on the `main` branch:

```
https://<your-org>.github.io/auracelle-charlie/Auracelle_Charlie_Portalv7.html
```

No build step is required. The portal is a fully self-contained single-file HTML application.

---

## The Simulation

### Eleven Tabs

| Tab | Name | Function |
|-----|------|----------|
| ① | Session Design | Configure scenario, validation case, composition group |
| ② | Facilitator Mode | Live negotiation — log actor moves, receive AI guidance |
| ③ | Governance Indicators | Real-time BGC domain scores and g-GWC index |
| ④ | Foresight Validation | Kalman trajectory vs. historical governance cases |
| ⑤ | After-Action Review | PSTOA score, session export, RL data download |
| ⑥ | SIPRI Data | Military expenditure and arms transfer intelligence |
| ⑦ | MARL Engine | Multi-agent reinforcement learning optimisation |
| ⑧ | Autonomous Sim | Fully AI-driven session, no human input required |
| ⑨ | Red Team & Shocks | Adversarial shock injection and resilience testing |
| ⑩ | Agentic AI | Policy Owner and Red Team agent configuration |
| ⑪ | Session Archive | Cross-session tracking and export |

### E-AGPO-HT v3.1 Framework

The scoring engine implements the **Evaluative Agentic Governance Policy Optimisation — Hybrid Taxonomy** framework. Seven Broad Governance Capability (BGC) domains are scored in real time:

| Code | Domain |
|------|--------|
| STI | Strategic Threat Intelligence |
| SAD | Security Architecture Design |
| ESI | Exploratory Simulation Intelligence |
| NDM | Negotiation Dynamics Modeling |
| SRA | Strategic Rationality Assessment |
| IIC | Institutional Implementation Capacity |
| ASI | Adaptive Scalability Intelligence |

The **g-GWC** (General Governance Wargaming Capacity) score aggregates all seven domains. A Kalman filter tracks trajectory across rounds and projects forward.

### Red Team Agent

The Red Team Agent fires pre-configured shocks automatically:
- **Round 4:** AI Incident Event — tests 15-day reporting enforcement
- **Round 5:** Unilateral Withdrawal — tests coalition resilience

Each shock logs a structured turn entry and computes governance indicator deltas.

### Reinforcement Learning Data

Every participant move is stored with:
- `rl_session_id`, `rl_scenario`, `rl_info_regime`, `rl_use_case`
- `rl_gwc_before`, `rl_gwc_after`, `rl_reward` (GWC delta)
- `rl_participant: true` (distinguishes human from AI moves)
- Full BGC snapshot at time of move

Session data is exported as JSON (primary research file) or CSV (flat analysis table).

---

## Research Context

**Principal Investigator:** Grace-Alice Evans, Founder, Auracelle AI Governance Labs
**Doctoral Programme:** Bath Spa University, School of Design
**Supervisor:** Dr. John Curry
**Thesis:** *Testing Public Policy Outcomes through War Gaming Methodologies for Strengthening AI Governance*

**Affiliations:**
- Non-Resident Senior Fellow, UC Berkeley Center for Long-Term Cybersecurity (CLTC)
- Technical Role Member, NATO STO SAS-219 (WinterStorm 2030)
  - R4: Disruptive Capabilities
  - R5: Digitally-Enabled Wargaming
  - R7: Diplomacy

**Key Publication:** Evans (Cleaveland, Evans et al.), UC Berkeley CLTC White Paper, December 2021

---

## Five Research KPIs

| KPI | Measurement | Instrument |
|-----|-------------|------------|
| 1 · Multilateralism | Coalition rate across six rounds | Turn log analysis |
| 2 · Stress Test Effectiveness | g-GWC shift pre/post shock | Kalman delta |
| 3 · Process Acceleration | Accel(AGPO) vs. 18-month baseline | PSTOA computation |
| 4 · Foresight Sustainability | Kalman trend direction | Forward projection |
| 5 · Weight Sensitivity | Pareto-optimal BGC weight config | MARL engine output |

---

## Pilot Workshop

**Dates:** June 7–14, 2026
**Format:** Autonomous, asynchronous — participants complete at any time within the window
**Duration:** 60–75 minutes
**Access Code:** Provided on registration confirmation

**Registration:** [Microsoft Forms — Registration Form Link]

Data submission: Email session JSON to `grace-alice.evans@bathspa.ac.uk`
Subject: `Charlie Pilot — [Your Name] — [Your Sector]`

---

## Citation

If you use Auracelle Charlie in your research, please cite using the `CITATION.cff` file or:

```
Evans, G-A. (2026). Auracelle Charlie v6.0: AI Governance War Game Simulation Sandbox.
Auracelle AI Governance Labs / Bath Spa University.
https://github.com/auracelle/auracelle-charlie
```

---

## License

This work is licensed under **Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)**.

You may share and adapt for non-commercial purposes with attribution.
Commercial use requires written permission from the PI.

See `LICENSE.md` for full terms.

---

## Contact

**Grace-Alice Evans**
Founder & Principal Investigator, Auracelle AI Governance Labs
grace-alice.evans@bathspa.ac.uk

LinkedIn: [grace-alice-evans-5a9632a3](https://www.linkedin.com/in/grace-alice-evans-5a9632a3)
Platform: [Auracelle AI Governance Labs](https://auracelle.github.io/Auracelle-AI-Governance-Labs-Platform-Comms-Public)

---

*Auracelle Charlie is part of the Auracelle suite of AI governance simulation platforms, which also includes Auracelle Orion (cybersecurity), Auracelle Lyra (multi-domain assurance), Auracelle Polaris (space governance), Auracelle Delphi (cognitive warfare / neurotech), and Auracelle WinterStorm2030 (NATO SAS-219 instrument).*
