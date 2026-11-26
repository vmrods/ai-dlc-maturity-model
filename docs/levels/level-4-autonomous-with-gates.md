# Level 4 · Autonomous with gates

**Machines integrate, people approve.** People only review and approve at G1, G2 and G3.

[← L3](level-3-orchestrated.md) · [All levels](README.md)

## What changes at this level

- Agents integrate, test, deploy to staging and assemble release evidence
- Canary releases with automatic rollback
- Each incident drafts its own regression test, eval or guardrail
- Compliance evidence produced as code

## Exit criteria

A team reaches Level 4 when every criterion below is met with evidence.

| Dimension | Criterion | How to get there | Owner |
|---|---|---|---|
| Governance | Model and prompt changes gated and audited like code | Put model and prompt changes through G1–G3 with an audit trail | AI platform team + compliance |
| Lifecycle | Manual touchpoints only at the three gates | Remove every manual touchpoint outside G1, G2 and G3 | Engineering excellence |
| Lifecycle | Canary releases with automatic rollback | Release through canaries with automatic rollback | SRE |
| Platform | ≥ 90% of pipeline steps automated | Automate 90% of pipeline steps; agents run integration and staging deploys | Platform |
| Platform | Release evidence assembled by the pipeline | Have the pipeline assemble release evidence for every G3 | QE + compliance |
| People | Roles updated; approver load reviewed quarterly | Update roles for gate-based work and review approver load every quarter | VP Engineering |
| Measurement | Change failure rate ≤ 6% | Bring change failure rate to 6% or below | SRE |
| Measurement | Lead time ≤ 2 days | Bring lead time to 2 days or below | Engineering excellence |
| Measurement | Time to restore ≤ 2 hours | Bring time to restore under 2 hours | SRE |
| Measurement | Every incident feeds a test, eval or guardrail | End every incident review with a linked test, eval or guardrail | SRE + pods |
| Partners | Partner delivery metrics within 20% of in-house | Bring partner teams' lead time and failure rate within 20% of in-house teams | Vendor management + directors |

## First steps

- Agents run integration and staging deploys after G2
- Pipeline assembles the release evidence for every G3
- Canary releases with automatic rollback

## Risks to watch

- Approvers stop reading as changes arrive faster
- Automatic rollback hides recurring faults
- Model or vendor changes break pinned behaviour

## Central assets

**Documents**

- Release evidence package spec
- Canary and rollback policy
- Incident review template with stage routing
- Runbook template
- Automation exception register

**Shared skills**

- Release notes and change record
- Incident timeline and review
- Regression test from an incident
- Runbook drafting
- Compliance evidence assembly

**Training**

- Champions: Expert (8 h)
- Release owners and SRE: automated release and rollback (4 h)

## Habits that make the move stick (level 3 → 4)

- Automate the most frequent manual step first
- Sample gate approvals monthly so reviews stay real
- Baseline time to restore before automating rollback

## Evidence

Our planning assumption; no published measurement yet. See [evidence](../evidence.md).
