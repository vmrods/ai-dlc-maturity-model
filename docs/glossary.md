# Glossary

**ADR** (also: ADRs): Architecture decision record: a short note of a decision, the options considered and why.

**AI Enablement team** (also: enablement team): A small central team that runs the AI gateway, context library, shared skills and training.

**AI gateway** (also: gateway): One entry point to approved AI models: single sign-on, logging of every call, cost per team and rate limits.

**AI-DLC**: AI-driven development lifecycle: a way of delivering software where AI drafts specs, code, tests and release material, and people approve at three gates.

**Calibration**: Adjusting the model's assumed gains and durations to match the actual results you recorded.

**Canary** (also: canaries): Releasing to a small share of traffic first and rolling back automatically if health checks fail.

**Champion** (also: champions): An engineer in each pod who spends 10–20% of their time leading AI-DLC adoption: training, context, skills and feedback.

**Change failure rate**: Share of production deployments that cause an incident, rollback or hotfix.

**Cohort** (also: cohorts): A group of products that moves through Levels 2–4 together on its own track, starting a few weeks after the group ahead and reusing what it built.

**Context library** (also: context): What agents read before they write: standards, domain knowledge, ADRs, repo instructions, prompts and skills, versioned in git.

**DORA**: The four delivery metrics from Google's DevOps Research and Assessment: deploy frequency, lead time, change failure rate and time to restore.

**Engineer-equivalents**: Extra delivery capacity expressed as headcount. It is time freed for more roadmap work, not a headcount cut.

**Eval** (also: evals): An automated test of AI behaviour: inputs with expected outputs, scored so a model or prompt change can't silently get worse.

**G1**: Gate 1: people approve the spec and plan before agents build.

**G2**: Gate 2: a named owner approves the merge after tests, scans and evals pass.

**G3**: Gate 3: the release owner approves the release, with evidence and a tested rollback.

**Golden-path** (also: golden path): A standard, pre-built pipeline and project template teams start from instead of building their own.

**Lead time**: Median time from a commit to it running in production.

**Mob Construction**: A working session where engineers steer agents as they build code and tests for a unit of work.

**Mob Elaboration**: A working session where product, the pod, an architect and QE turn intent into an approved plan with AI drafting it.

**Pod** (also: pods): A small delivery team (usually 5–9 people) that owns a product area end to end.

**Risk tier** (also: risk tiers): Low, medium or high, set per unit of work. High-risk work gets staff-engineer review at G2.

**Skill** (also: skills): A reusable, tested set of instructions an agent follows for a recurring job, such as writing tests or drafting a spec.

**Spec** (also: specs): The written intent for a piece of work: goal, acceptance criteria, non-functional needs and risk tier. Agents build from it.
