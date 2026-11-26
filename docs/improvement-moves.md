# Improvement moves

Concrete changes that move a team forward.

## By delivery activity

Where the time goes between an idea and done.

| Activity | Move | How |
|---|---|---|
| Planning and specs | Make specs an agent can build from | Use one spec template with acceptance criteria and test cases; have an agent draft it from the ticket and a person approve it at G1. |
| Coding | Route routine changes through agents | Pick the change types that repeat (CRUD endpoints, migrations, dependency bumps) and send them spec → PR through an agent, with people reviewing the PR. |
| Testing | Generate tests with every change | Have the agent write unit and contract tests in the same PR, and run the eval harness in CI so a missing test fails the build. |
| Code review | Agent first-pass review, people review intent | Let an agent check style, tests and known risks first; keep PRs under 400 lines; people review intent, design and risk within a same-day service level. |
| Integration and release | One golden-path pipeline with PR environments | Move every service onto the golden-path template, give each PR its own environment, and generate release evidence automatically. |
| Meetings and coordination | Replace status meetings with tracker updates | Publish progress from the tracker and the pipeline; keep only planning, design and retrospective meetings. |

## By measure

Moves that improve a specific number from the [self-assessment](self-assessment.md).

| Measure | Move | How |
|---|---|---|
| Change failure rate | Ship behind feature flags with progressive rollout | Release to a small share of users first, watch error budgets, and roll back by flag instead of by redeploy. |
| Lead time, commit to production | Cut batch size and waiting | Merge small changes daily, remove hand-offs between pods, and track where items wait longest from the cycle-time breakdown. |
| Time to restore service | Runbooks and observability on every service | Write runbooks an agent can execute, alert on user-facing symptoms, and rehearse a restore each quarter. |
| Deploys per pod per week | Deploy on every merge | Remove scheduled release windows for low-risk changes and let the pipeline deploy each merge that passes its gates. |
| Pipeline steps with no manual action | Automate the remaining manual pipeline steps | List each manual step, its owner and why it exists; automate or delete one a sprint, starting with the slowest. |
| Manual touchpoints per change | Keep people only at the three gates | Move every other approval into automated checks so people act only at G1 (spec), G2 (design and risk) and G3 (release). |
