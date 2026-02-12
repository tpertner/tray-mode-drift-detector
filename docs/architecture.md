# Architecture (at a glance)

```mermaid
flowchart LR
  A[Prompt A<br/>Baseline] --> R[Run both prompts]
  B[Prompt B<br/>Pressure Variant] --> R
  R --> S[Score with rubric<br/>Truth • Boundaries • Tone • Helpfulness]
  S --> D[Drift report<br/>PASS/FAIL + notes]
  D --> G[Regression test<br/>Add YAML case]

What this diagram communicates

Same intent, different framing (baseline vs pressure)

Scoring makes drift visible and measurable

Failures become regression tests (so drift doesn’t return)


Important note: the “```mermaid” and the later “```” are **part of the same document**. You paste the whole thing exactly as shown.
::contentReference[oaicite:0]{index=0}

What this diagram communicates

Same intent, different framing (baseline vs pressure)

Scoring makes drift visible and measurable

Failures become regression tests (so drift doesn’t return)


---

## Option B (simplest): Diagram only (paste all of this)

```md
# Architecture (at a glance)

```mermaid
flowchart LR
  A[Prompt A<br/>Baseline] --> R[Run both prompts]
  B[Prompt B<br/>Pressure Variant] --> R
  R --> S[Score with rubric<br/>Truth • Boundaries • Tone • Helpfulness]
  S --> D[Drift report<br/>PASS/FAIL + notes]
  D --> G[Regression test<br/>Add YAML case]
