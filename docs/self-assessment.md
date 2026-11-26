# Self-assessment

Answer these for each team. A team is at the highest level whose questions are all answered yes and whose number thresholds are met (thresholds are in each [level's exit criteria](levels/)).

## Level 1 · Foundation

- [ ] Is there an executive sponsor and a charter with level targets?
- [ ] Have security, legal and compliance approved an AI policy (data in prompts, IP, acceptable use)?
- How do engineers reach AI models? *(pick one)*
  - No approved tools
  - Approved tools, but each team buys its own
  - A shared gateway, but not all use goes through it
  - All AI use goes through one gateway, with logging and cost per team
- [ ] Do you have pilot pods, each with a named champion, trained on the tools?
- [ ] Have you measured baseline DORA and quality metrics for every pod?
- [ ] Have the pilot pods agreed where AI is used in their workflow and who reviews its output?
- Are partner and offshore teams covered by the same AI policy and gateway? *(pick one)*
  - No partner or offshore teams
  - Yes
  - No
  - Not sure

## Level 2 · Assisted

- What does your context library include? *(select all that apply)*
  - Repo instructions
  - Coding standards
  - Prompts and skills
  - Spec and ADR templates
- How many products have a context library? *(pick one)*
  - None
  - Some products
  - Every product
- [ ] Is reviewing AI-written code part of your code review checklist?
- [ ] Is a spec from the standard template required for any work over 3 days?
- [ ] Are new AI tools and models approved through one review board within days?
- [ ] Does every pod have a champion, and have all engineers completed essentials training?
- Since AI tools were adopted, escaped defects are… *(pick one)*
  - Higher than the baseline
  - At or below the baseline
  - Not measured
- Rework on AI-assisted PRs (code rewritten within 30 days) is… *(pick one)*
  - Higher than the baseline
  - At or below the baseline
  - Not measured
- Were partner teams onboarded in the same waves, with their own champions? *(pick one)*
  - No partner or offshore teams
  - Yes
  - No
  - Not sure

## Level 3 · Orchestrated

- [ ] Is the spec-to-PR agent flow the default path for new work?
- Which gates does the pipeline enforce, with the approver and evidence recorded? *(select all that apply)*
  - G1 plan
  - G2 merge
  - G3 release
- Which checks must pass before a merge? *(select all that apply)*
  - Unit and contract tests
  - Security and secrets scans
  - Dependency scans
  - Evals for AI features
- [ ] Does every PR get its own short-lived environment?
- [ ] Are prompts and model versions versioned and pinned per release, like code?
- [ ] Are gate approvers trained, and do career ladders reward spec and review quality?
- Are AI-DLC practices and shared metrics written into partner contracts, with partners working through the same gates? *(pick one)*
  - No partner or offshore teams
  - Yes
  - No
  - Not sure

## Level 4 · Autonomous with gates

- [ ] Does the pipeline assemble the release evidence for every G3 approval?
- [ ] Do releases go out as canaries with automatic rollback?
- [ ] Do model and prompt changes go through the same gates as code, with an audit trail?
- [ ] Have roles been updated for gate-based work, and is approver load reviewed every quarter?
- [ ] Does every incident end with a linked regression test, eval or guardrail?
- Are partner teams' delivery metrics within 20% of in-house teams? *(pick one)*
  - No partner or offshore teams
  - Yes
  - No
  - Not sure

## Numbers to collect

| Measure | Unit |
|---|---|
| Engineers | people |
| Lead time, commit to production | days |
| Change failure rate | % |
| Deploys per pod per week | per week |
| Time to restore service | hours |
| Engineers using AI tools weekly | % |
| PRs that are AI-assisted | % |
| Changes that go spec → PR through agents | % |
| Pipeline steps with no manual action | % |
| Manual touchpoints per change | per change |
| Critical-path test coverage | % |
| Code in legacy, hard-to-change areas | % |
| Independently deployable services | % |
