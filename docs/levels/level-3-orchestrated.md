# Level 3 · Orchestrated

**Agents carry work from spec to PR.** People approve plans, merges and releases; the pipeline verifies.

[← L2](level-2-assisted.md) · [All levels](README.md) · [L4 →](level-4-autonomous-with-gates.md)

## What changes at this level

- Spec-driven agents build code and tests in mob sessions
- Three human gates: G1 plan, G2 merge, G3 release, with risk tiers
- Tests, evals and security scans are required pipeline checks
- Ephemeral PR environments; prompts and models versioned like code

## Exit criteria

A team reaches Level 3 when every criterion below is met with evidence.

| Dimension | Criterion | How to get there | Owner |
|---|---|---|---|
| Governance | Prompts and model versions pinned like code | Version and pin prompts and model versions in a registry | AI platform team |
| Lifecycle | Spec-to-PR agent flow is the default for new work | Move delivery to the spec-driven agent flow with Mob Elaboration and Mob Construction | Product + pod leads |
| Lifecycle | G1, G2 and G3 enforced by the pipeline | Enforce G1, G2 and G3 in the pipeline, recording approver and evidence | Platform |
| Lifecycle | Tests, security and dependency scans and evals required before merge | Make tests, security and dependency scans and evals required checks before merge | Platform + QE |
| Platform | A short-lived environment for every PR | Give every PR its own short-lived environment | Platform |
| Platform | Critical-path test coverage ≥ 70% | Raise critical-path test coverage to 70% | QE + pods |
| Platform | ≥ 70% of pipeline steps automated | Automate 70% of pipeline steps | Platform |
| People | Gate approvers trained; ladders reward specs and reviews | Train gate approvers and update career ladders to reward spec and review quality | VP Engineering + HR |
| Measurement | Change failure rate ≤ 10% | Bring change failure rate to 10% or below | Engineering excellence + SRE |
| Measurement | Lead time ≤ 5 days | Bring lead time to 5 days or below | Engineering excellence |
| Partners | AI-DLC practices and metrics in partner contracts | Add AI-DLC practices, gates and shared metrics to vendor SOWs | Vendor management + legal |

## First steps

- Run spec-driven Mob Elaboration and Mob Construction
- Make tests, scans and evals required pipeline checks
- Enforce G1, G2 and G3 in the pipeline, with risk tiers

## Risks to watch

- Weak tests turn faster merges into faster incidents
- Agents working from vague specs
- Gates becoming rubber stamps

## Central assets

**Documents**

- Risk-tier rubric
- Gate definitions with required evidence (G1–G3)
- Eval plan template
- Prompt and model change record
- Golden-path pipeline spec
- Definition of done for agent-built changes

**Shared skills**

- Spec to units of work
- Contract test generation
- Eval case authoring
- Security review
- Dependency upgrade

**Training**

- Champions: Advanced (12 h)
- Gate approvers: reviewing at G1, G2 and G3 (3 h)

## Habits that make the move stick (level 2 → 3)

- Raise test coverage on critical paths during Level 2
- Require a spec for any work over 3 days
- Start with 2–3 well-tested products

## Evidence

Extrapolated from published results and DORA performance bands. See [evidence](../evidence.md).
