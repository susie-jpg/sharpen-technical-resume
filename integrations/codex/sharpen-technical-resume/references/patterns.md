# Rewrite Patterns

Use these as reasoning patterns, not mandatory visible templates.

## Full project

```text
[Project / System] | [technical theme] | [date]
- Background / Goal: [user or business problem], under [constraint], targeting [measurable goal].
- Scope: [led / co-built / implemented] [bounded responsibility and decisions].
- Architecture / Execution chain: [input] -> [core stages] -> [output]; explain the hardest 1-3 mechanisms and why they exist.
- Results: [metric with unit, baseline, sample/window if known]; [quality, cost, speed, adoption, or reliability impact].
- Evidence: [repository / paper / demo / award / article].
```

## Compact bullet

```text
[Strong verb] [system/mechanism] to solve [problem], using [important design choice]; achieved [measured result] under [scale/constraint].
```

## Before and after

Weak:

```text
负责 Agent 平台开发，使用 Docker、Python 和大模型，提升了效率。
```

Strong only when supported:

```text
主导评测 Agent 的隔离执行链路，将仓库恢复、容器申请、补丁运行与结果回传统一为 `spec -> session -> run -> restore -> report`；在 200 个任务上将单任务准备时间由 4.2 分钟降至 55 秒，失败任务可从 checkpoint 续跑。
```

The stronger version works because it states attribution, mechanism, scale, baseline, result, and recovery behavior. If any element is unknown, omit it or mark it for confirmation.

## Evidence hierarchy

Prefer evidence in this order:

1. Measured production or benchmark result with scope and window.
2. Public artifact such as repository, paper, demo, or award.
3. Concrete architecture and decision with a clearly bounded personal contribution.
4. Named technology without mechanism or result.
5. Self-assessment or generic adjective.

Cut lower-level evidence when space is limited.

## Compression

- Combine repeated stack lists into one mechanism-focused bullet.
- Keep at most 2-4 bullets for a normal project and 4-6 for the strongest project.
- Use arrows for genuine pipelines, not decorative sequences.
- Move secondary technologies to a compact skills section.
- Delete background that a target recruiter already knows unless it establishes a constraint.

## High-value questions

- What did you personally decide or build, versus the team?
- What was the before/after result, metric definition, sample, and time window?
- What scale or constraint made the problem difficult?
- What failure mode did the design prevent or recover from?
- Is there a public link or artifact that verifies the claim?
