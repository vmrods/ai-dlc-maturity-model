# AI-DLC Maturity Model

A four-level model for adopting an **AI-driven development lifecycle (AI-DLC)** in an engineering organization: from individual, ad hoc AI use to a delivery flow where AI drafts specs, code, tests and release material and people approve at three gates.

Each level has exit criteria with an owner, first steps, risks to watch, and the central assets (documents, shared skills, training) a program needs to get there. Progress is measured with DORA delivery metrics and AI-adoption signals, so every level change can be proven, not just claimed.

## The levels

| Level | Focus | What people do | Evidence |
|---|---|---|---|
| [L1 · Foundation](docs/levels/level-1-foundation.md) | Prepare the program | People do all the work. AI is used by individuals, ad hoc. | Field studies |
| [L2 · Assisted](docs/levels/level-2-assisted.md) | AI in every pod's daily work | AI drafts; engineers write, integrate and release by hand. | Field studies |
| [L3 · Orchestrated](docs/levels/level-3-orchestrated.md) | Agents carry work from spec to PR | People approve plans, merges and releases; the pipeline verifies. | Extrapolated |
| [L4 · Autonomous with gates](docs/levels/level-4-autonomous-with-gates.md) | Machines integrate, people approve | People only review and approve at G1, G2 and G3. | Assumed |

Level 0, **Today**, is the starting point: where the organization is before the program begins.

## Six dimensions

Every exit criterion belongs to one dimension, so gaps show up by area, not just by level.

| Dimension | Question it answers |
|---|---|
| Governance | What's allowed |
| Lifecycle | How work flows |
| Platform | What makes it repeatable |
| People | Who carries it |
| Measurement | Proof it works |
| Partners | Everyone aligned |

## What's in this repository

| Document | What it covers |
|---|---|
| [Levels](docs/levels/) | One page per level: what changes, exit criteria by dimension, first steps, risks, assets, habits |
| [Self-assessment](docs/self-assessment.md) | The yes/no and number questions that place a team on the model |
| [Roles](docs/roles.md) | How each role in a pod changes from level to level |
| [Measurement](docs/measurement.md) | Metric families, metric definitions, healthy thresholds and DORA 2024 bands |
| [Improvement moves](docs/improvement-moves.md) | Practical changes that move a team forward, by activity |
| [Acceleration levers](docs/levers.md) | Program-level choices that shorten the path, with a confidence rating |
| [Evidence](docs/evidence.md) | How strong the evidence is behind each level |
| [Glossary](docs/glossary.md) | Terms used throughout the model |

## How to use it

1. **Place your teams.** Answer the [self-assessment](docs/self-assessment.md) for each team. A team is at the highest level whose exit criteria it fully meets.
2. **Measure the baseline first.** Level 1 requires DORA and quality metrics for every pod before any gain can be claimed. See [measurement](docs/measurement.md).
3. **Plan the next level only.** Use that level's exit criteria, owners and first steps as the plan. Each page lists the risks that most often stall a program.
4. **Prove the move.** A level is reached when its exit criteria are met with evidence, not when the work is scheduled.

## About

Built and maintained by Victor Rodriguez (Founder & CTO, [Joining Clouds](https://joiningclouds.com)). The model also drives a simulator that forecasts timeline, staffing and value before a team commits; the simulator is not part of this repository.

Model version: `2026-11-23a`. Benchmark bands come from the DORA Accelerate State of DevOps Report, 2024 (v. 2024.2).

## License

Copyright © 2026 Joining Clouds Inc. Licensed under [Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)](LICENSE).

You may share and adapt this model for non-commercial purposes, with attribution. For commercial use, including consulting or paid training built on it, contact [Joining Clouds](https://joiningclouds.com).
