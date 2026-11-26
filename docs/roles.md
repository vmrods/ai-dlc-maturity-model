# Roles

How each role in a delivery pod, and the roles shared across pods, changes from level to level.

## The three gates

| Gate | Who approves |
|---|---|
| G1 plan | Product manager + pod lead; architect joins for high-risk work |
| G2 merge | The engineer who owns the change; pod lead or a staff engineer for high-risk changes |
| G3 release | Release owner (pod lead or engineering manager), with QE's evidence and SRE's rollback plan |

## Pod lead

*Staff or senior engineer.*

Sets technical direction for the product, runs Mob Construction, owns the pod's repo instructions and approves high-risk merges at G2.

| Level | What changes |
|---|---|
| L1 · Foundation | Learns the tools and policy; picks the pod's first AI use cases. |
| L2 · Assisted | Sets the pod's AI norms and reviews AI-written code with the team. |
| L3 · Orchestrated | Turns approved specs into units of work for agents; signs G2 for high-risk changes. |
| L4 · Autonomous with gates | Reviews agent-run integration and release evidence; spends most time on design and gate decisions. |

## Engineers

*One of them is the champion.*

Build features by steering agents; write and review specs, tests and code. Each is the named owner of their changes.

| Level | What changes |
|---|---|
| L1 · Foundation | Use approved tools on their own work, inside the policy. |
| L2 · Assisted | AI drafts code, tests and first-pass reviews; engineers integrate and release by hand. |
| L3 · Orchestrated | Agents carry work from spec to PR; engineers steer, review and sign G2 as named owners. |
| L4 · Autonomous with gates | Mostly specs, reviews and gate approvals; agents integrate, test and deploy. |

## Champion

*One of the engineers, 10–20% of their time.*

Leads adoption in the pod: context library, shared skills, coaching, and feedback to the AI Enablement team.

| Level | What changes |
|---|---|
| L1 · Foundation | Takes Foundation training and helps run the pilot. |
| L2 · Assisted | Onboards the pod, curates its context library and publishes a skill. |
| L3 · Orchestrated | Coaches spec-driven work and gate reviews; writes eval sets. |
| L4 · Autonomous with gates | Automates the remaining manual steps; turns incident lessons into skills and context. |

## Embedded QE

*Quality engineer.*

Owns test strategy and evals, keeps the automated checks honest, and validates releases independently before G3.

| Level | What changes |
|---|---|
| L1 · Foundation | Baselines escaped defects and critical-path test coverage. |
| L2 · Assisted | Reviews AI-drafted tests and raises critical-path coverage. |
| L3 · Orchestrated | Owns the required pipeline checks and the eval sets for AI features. |
| L4 · Autonomous with gates | Validates the release evidence the pipeline assembles; samples gate quality. |

## Product manager

*1 per pod or product.*

Brings the intent and acceptance criteria; approves the spec and plan at G1 with the pod lead.

| Level | What changes |
|---|---|
| L1 · Foundation | Joins the pilot ceremonies and defines what success looks like. |
| L2 · Assisted | Writes specs from the template, with AI drafting. |
| L3 · Orchestrated | Runs Mob Elaboration with the pod; signs G1. |
| L4 · Autonomous with gates | Turns usage and SLO signals into new intents; signs G1. |

## Engineering manager

*1 per 2 pods.*

People, hiring, capacity and delivery commitments; protects the champion's time.

| Level | What changes |
|---|---|
| L1 · Foundation | Sets adoption goals with the directors. |
| L2 · Assisted | Tracks adoption and rework, and removes blockers. |
| L3 · Orchestrated | Moves roles and career ladders toward specs, reviews and gate quality. |
| L4 · Autonomous with gates | Plans how to use the capacity automation frees. |

## Architect

*1 per group of pods.*

ADRs, risk tiers and cross-product design; joins G1 for high-risk work.

| Level | What changes |
|---|---|
| L1 · Foundation | Reviews the AI policy and gateway design. |
| L2 · Assisted | Publishes the spec and ADR templates agents read. |
| L3 · Orchestrated | Sets risk tiers; joins G1 for high-risk units. |
| L4 · Autonomous with gates | Owns the architecture guardrails agents follow. |

## SRE

*Shared platform team.*

SLOs, incidents and release safety; owns canary releases and rollback.

| Level | What changes |
|---|---|
| L1 · Foundation | Baselines time to restore and incident rates. |
| L2 · Assisted | Keeps releases stable as change volume rises. |
| L3 · Orchestrated | Adds SLO checks to the pipeline. |
| L4 · Autonomous with gates | Runs canary releases with automatic rollback; leads incident learning. |
