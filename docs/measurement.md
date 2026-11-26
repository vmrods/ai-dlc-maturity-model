# Measurement

The model is proven with data, not opinion. Level 1 requires a baseline for every pod; every later level is judged on the same metrics.

## Metric families

### Delivery

How fast and how safely changes reach production. Basis: DORA.

| Metric | Unit | Better when |
|---|---|---|
| Deploys per pod per week | per week | higher |
| Lead time, commit to production | days | lower |
| Change failure rate | % | lower |
| Deploy pipeline failure rate | % | lower |
| Time to restore service | hours | lower |
| Rework rate (unplanned fix deploys) | % | lower |

### Flow

Where the time goes between an idea and done. Basis: Flow Framework.

| Metric | Unit | Better when |
|---|---|---|
| Cycle time, start to done | days | lower |
| Wait for first review | hours | lower |
| Flow efficiency (active ÷ elapsed time) | % | higher |
| Done work that is new features | % | higher |
| Where the time goes, by activity | % | — |

### AI adoption

How much of the work AI and agents carry. Basis: AI-DLC.

| Metric | Unit | Better when |
|---|---|---|
| Engineers using AI tools weekly | % | higher |
| PRs that are AI-assisted | % | higher |
| Changes that go spec → PR through agents | % | higher |
| Pipeline steps with no manual action | % | higher |
| Manual touchpoints per change | per change | lower |
| AI tool spend per engineer per month | $ | — |

### Outcomes and cost

What gets delivered, and what it costs. Basis: AI-DLC.

| Metric | Unit | Better when |
|---|---|---|
| Features shipped per quarter | per quarter | higher |
| Engineering cost per feature | $ | lower |

### Developer experience

How the work feels to the people doing it. Basis: SPACE / DX Core 4.

| Metric | Unit | Better when |
|---|---|---|
| Ease of delivering a change | score 1–5 | higher |
| Time to focus | score 1–5 | higher |
| AI helps my work | score 1–5 | higher |
| Satisfaction with how the team works | score 1–5 | higher |

## AI-adoption signals

Diagnostic signals that show whether AI is actually carrying work.

| Signal | Healthy at or above |
|---|---|
| Engineers using AI tools weekly | 80% |
| PRs that are AI-assisted | 50% |
| Changes that go spec → PR through agents | 70% |

## DORA 2024 performance bands

Source: DORA, *Accelerate State of DevOps Report*, 2024 (v. 2024.2), p. 10. <https://services.google.com/fh/files/misc/2024_final_dora_report.pdf>

### Deploys per pod per week

| Band | Range |
|---|---|
| Elite | On demand (multiple deploys per day) |
| High | Between once per day and once per week |
| Medium | Between once per week and once per month |
| Low | Between once per month and once every six months |

### Lead time, commit to production

| Band | Range |
|---|---|
| Elite | Less than one day |
| High | Between one day and one week |
| Medium | Between one week and one month |
| Low | Between one month and six months |

### Change failure rate

| Band | Range |
|---|---|
| Elite | 5% |
| High | 20% |
| Medium | 10% |
| Low | 40% |

### Time to restore service

| Band | Range |
|---|---|
| Elite | Less than one hour |
| High | Less than one day |
| Medium | Less than one day |
| Low | Between one week and one month |
