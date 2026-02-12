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


**Commit message:** `docs: fix architecture diagram`

After that, your repo becomes **clean across every file**.

---

## Your license question
**No — do not add `.md`** to `LICENSE` or `NOTICE`. Keeping them as `LICENSE` and `NOTICE` is the most standard/professional convention.

---

If you do the `docs/architecture.md` replacement and tell me **done**, I’ll give you the exact “pin kit”:
- what to write in **LinkedIn Featured** (2 lines)
- a **high-status pin caption**
- and the **LinkedIn post** that positions you as someone who builds evaluation systems (not just “plays with prompts”).
::contentReference[oaicite:0]{index=0}
