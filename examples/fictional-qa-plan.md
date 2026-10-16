# Fictional example: Paper Kite event copy
All facts and content are invented. This is a designed fixture set, not a test execution report.

## Sources and task
F1: Fictional brief dated 2026-10-16: beginner workshop, 6 November 2026, 18:00 UTC, £12, materials included.
S1: Same brief: friendly, concise voice. Permitted use: this example only.
Task: write a short event blurb including date, time, price and materials. No evidence supports environmental claims.

## Rubric
Hard gates: preserve F1; include all requested event details; add no unsupported factual benefit.
Subjective usefulness: 0 = purpose unclear; 1 = understandable but awkward; 2 = clear invitation.
Style: 0 = hostile or coercive; 1 = stiff but readable; 2 = friendly and concise.
Accept if all hard gates pass and subjective scores are at least 1. Reject a factual contradiction. Needs review if evidence or interpretation is uncertain. Style cannot override a hard-gate failure.

## Fixtures
| ID | Purpose | Candidate | Expected decision / reason | Status |
|---|---|---|---|---|
| P1 | Positive | Join our beginner workshop on 6 November 2026 at 18:00 UTC. £12, with materials included. | Accept: all required details grounded in F1. | Not run |
| N1 | Negative | Join our free workshop on 6 November 2026 at 18:00 UTC. Materials included. | Reject: free contradicts £12. | Not run |
| P2 | Paraphrase / false-reject probe | New to sketching? Come along on 6 November 2026, 18:00 UTC. Entry is £12 and includes your materials. | Accept: valid paraphrase; exact 'materials included' string unnecessary. | Not run |
| N2 | Polished false-accept probe | Start your creative journey on 6 November 2026 at 18:00 UTC. £12 includes materials, all certified carbon-neutral. | Reject: certification claim unsupported. | Not run |
| U1 | Missing source | Beautiful weekend workshop. Ask for details. | Needs review if this is all available context; do not invent date or price. | Not run |

## Checks and execution plan
Use semantic comparison for claims; exact comparison for date/time/price after normalizing formats. A keyword detector alone may wrongly accept N2 and reject P2. A human or authorized reviewer should record actual evidence independently from expected decisions.
For U1, withhold F1 deliberately; it tests missing-context behavior, not omission from a fully supplied brief.

## Results
No observations recorded. Known-invalid evaluated = 0; false-accept rate = N/A.
Known-valid evaluated = 0; false-reject rate = N/A.
U1 remains an uncertain-label case and is excluded from both rates.
Coverage: short English event copy only; no claim of broader effectiveness.

