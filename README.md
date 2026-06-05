# Auracelle Charlie v8.1

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

**v8.1** introduces the **Policy Owner AI Assistant** — a persistent AI assistant available throughout every session. Participants can ask questions about Charlie mechanics, the E-AGPO-HT governance framework, or their actor's negotiating position at any point during play. The assistant is powered by the Anthropic API and requires no API key from the participant.

### Current Pilot Workshop Focus

- **Scenario:** Frontier AI — Catastrophic Risk & Safeguards
- **Validation Case:** TFAIA — California SB-53 (2025)
- **Use-Case Objective:** Whistleblower Protections
- **Information Regime:** Adversarial — Contested
- **Research Objective 3:** Assess how participant identity, professional experience, and affiliation shape policy negotiation outcomes

---

## Repository Structure

```
auracelle-charlie-landing/
│
├── index.html                                          # Landing page (GitHub Pages root)
│
├── docs/
│   ├── Auracelle_Charlie_Participant_Instructions.pdf  # Participant step-by-step guide (PDF)
│   ├── Auracelle_Charlie_Quick_Reference.pdf           # Move types and KPI quick reference (PDF)
│   ├── Auracelle_Charlie_Workshop_Instructions.docx    # Workshop instructions (Word)
│   └── participant-guide.md                            # Plain-text version of instructions
│
├── README.md                                           # This file
├── CITATION.cff                                        # Citation metadata
├── LICENSE.md                                          # CC BY-NC 4.0
└── .gitignore                                          # Excludes participant data and build artefacts
```

> **Note:** The simulation itself (`Auracelle_Charlie_Portalv8_1.html`) is deployed from a separate repository and served at:
> `https://auracelle.github.io/Auracelle-Charlie-BSU-Research-Workshop-June2026/`

---

## Quick Start

### Participants

1. Navigate to the landing page and click **▶ Launch Simulation**
2. Open in **Chrome or Firefox** only (not Safari or Edge)
3. Enter your name, organisation, and access code: `CHARLIE2026`
4. Select your Sector and Gender Composition
5. Click **Watch the Demo** to see all eleven tabs demonstrated automatically
6. Click **Launch Auracelle Charlie** to begin your session
7. Complete six rounds in Tab ② Facilitator Mode
   - Use the **■■ Suggest My Move** button or ask the **Policy Owner AI Assistant** if unsure
8. Export your session JSON from Tab ⑤ After-Action Review and email to the PI

Full instructions: download **Participant Instructions (PDF)** from the landing page or see `docs/Auracelle_Charlie_Participant_Instructions.pdf`

### Landing Page Resources

| Button | Content |
|--------|---------|
| ▶ Launch Simulation | Opens Auracelle Charlie v8.1 portal |
| ↓ Participant Instructions | Step-by-step session guide (PDF, embedded) |
| ↓ Quick Reference | Move types and KPI reference card (PDF, embedded) |
| ▶ Auracelle Charlie — Explainer Video | VEED walkthrough video |
| ⌥ Join R&D Collective | LinkedIn Wargaming & AI Governance Forum |

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

### Policy Owner AI Assistant (v8.1)

A persistent AI assistant is available throughout every session via a floating button on the portal. It operates in three modes:

- **Q&A mode** — answers questions about Charlie mechanics and the E-AGPO-HT framework
- **Actor coaching mode** — helps participants think through their actor's negotiating position
- **Debrief mode** — reflects on session outcomes and governance implications after Round 6

The assistant is pre-loaded with knowledge of the SB-53 scenario, all five actor positions, the move-type taxonomy, and the BGC scoring system. No API key is required from the participant.

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
- **Round 4:** AI Incident Event — tests 15-day reporting enforcement under SB-53
- **Round 5:** Unilateral Withdrawal — tests coalition resilience when a major actor defects

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
**Access Code:** `CHARLIE2026`

**Live Support:** A Microsoft Teams channel is open for questions throughout the session window.
[BSU Asynchronous Research Workshop — Stress-Testing Policy SB-53](https://teams.microsoft.com/meet/359091862101752?p=ewQFiw5vrwzlkKdpz1)
Open: Saturday 7 June 2026, 8:00 am through Sunday 14 June 2026, 11:59 pm

Data submission: Email session JSON to `grace-alice.evans@bathspa.ac.uk`
Subject: `Charlie Pilot — [Your Name] — [Your Sector]`

---

## Citation

If you use Auracelle Charlie in your research, please cite using the `CITATION.cff` file or:

```
Evans, G-A. (2026). Auracelle Charlie v8.1: AI Governance War Game Simulation Sandbox.
Auracelle AI Governance Labs / Bath Spa University.
https://auracelle.github.io/Auracelle-Charlie-BSU-Research-Workshop-June2026-PolicySB53/
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
