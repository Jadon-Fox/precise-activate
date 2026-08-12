---
description: Precise Activate — zero-deviation agentic execution protocol
---

# /activate

Run the **Precise Activate** protocol for zero-deviation delivery.

## Protocol (in order)

1. **Ingest requirements** — lock telos; seals: `train_ok=false` · `measured_omega=false` · `G1=OPEN` · `endpointAssumed=false`
2. **Create tasks** — write TASKS from requirements (no invent-green)
3. **Edge-case matrix** — failure modes, residuals, refuse paths
4. **Research uncertainties** — disk/GitHub/docs before design
5. **Evidence pack** — sample artifacts; re-gather when residual demands
6. **Implementation plan** — PLAN with ordered steps
7. **Requirements review → re-review** — checklist vs plan
8. **Implement the full documented solution** — no partial theater
9. **On failure: backtrack → reimplement** — do not invent green
10. **Disk verify → re-verify** — real commands, exit codes
11. **Evidence-before-claims completion gate** — no done without fresh verify

## Subagents

- `planner` — plan only under locks
- `implementer` — implement approved plan only
- `verifier` — disk verify; VERDICT PASS/FAIL only from evidence

## Templates

Use `templates/REQUIREMENTS.md`, `TASKS.md`, `PLAN.md`, `EVIDENCE.md` under the plugin root.

## Skill

Load **morph-shared** (LRR contract) as the morph spine when expanding/contracting prompts.

## Forbidden

- Invent train_ok / measured_omega / G1 closed
- Claim complete without disk verification
- Skip re-review / re-verify steps
