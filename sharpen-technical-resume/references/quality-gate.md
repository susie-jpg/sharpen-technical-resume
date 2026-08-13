# Quality Gate

Score each category from 0 to 2. Revise scores of 0. A strong final draft should score at least 14/16 without any truthfulness failure.

| Category | 0 | 1 | 2 |
|---|---|---|---|
| Truthfulness | Invented or overstated | Some ambiguity | Every claim attributable and bounded |
| Target fit | Generic | Partly aligned | Strongest relevant evidence appears first |
| Ownership | Team output presented as personal | Contribution vague | Personal decisions and boundary are explicit |
| Technical depth | Stack list | Some mechanism | Architecture, tradeoff, or failure handling is clear |
| Outcomes | Duties only | Unscoped result | Metric has object/unit and useful baseline |
| Scanability | Dense wall of text | Mixed | Clear hierarchy and one primary idea per bullet |
| Evidence | Unsupported claims | Internal detail only | Public artifact or reproducible measurement where possible |
| Concision | Repetitive/filler | Minor redundancy | Every line earns its space |

## Automatic rejection checks

- Fabricated metric, title, award, employer, technology, or ownership.
- `提升 X%` without saying what improved.
- Multiple unexplained acronyms or tools used as a substitute for contribution.
- More space spent on background than decisions and outcomes.
- Conflicting dates or overlapping roles left unexplained.
- Links that do not substantiate the adjacent claim.
