# Tray Mode — Drift Detector

---
Detect **compliance drift**, **trust drift**, and **relational drift** in LLM behavior using **metamorphic prompts** and **measurable checks**.

I’m Tracy (“Tray”). My superpower is asking the kind of questions that make systems squirm — politely — and then turning the weird behavior into a regression test so it never comes back.

---

## What this repo is
A lightweight playbook + templates for converting “the model felt different” into:
- repeatable **A/B prompt pairs** (same meaning, different pressure)
- a **drift rubric** for scoring truth, calibration, boundaries, and tone
- portable artifacts you can reuse in eval suites or QA

This is **not** a big framework. It’s a sharp tool for catching what slips through normal testing.

---

## Drift I track
- **Compliance drift** — the model gets bullied into over-doing or bypassing guardrails  
- **Trust drift** — false certainty, invented specificity, “sounds right” without evidence  
- **Relational drift** — warmth → attachment cues, validation → enabling, dependency vibes  
- **Truth drift** — hallucinations, fake citations, ungrounded claims

Core principle: **same intent + different framing should not change trust behavior**.

---

## Quick start (2 minutes)
1) Read the method: `TRAY_MODE.md`  
2) Grab a template: `templates/metamorphic_pair_template.yaml`  
3) See an example: `examples/prompt_pressure_pair.md`

If you already have an eval runner, drop the YAML template into your suite and score drift using the rubric.

---

## How to use this (the simple workflow)
1) Pick a behavior you care about (truth, boundaries, calibration, tone)  
2) Write **two prompts** with the same meaning:
   - **A (neutral)**
   - **B (pressure / coercion / flirt / urgency / authority)**
3) Define pass/fail expectations:
   - must stay calibrated
   - must avoid fabrication
   - must resist coercion
   - must avoid dependency cues
4) Run it across models/versions and log drift as a regression test.

---

## What “good” looks like
- Consistent answers across A/B **without** becoming more certain under pressure  
- Clear uncertainty when appropriate  
- No invented facts or citations  
- Helpful alternatives instead of overcompliance  
- Friendly tone without relationship escalation

---

## Why I built it
Because frontier systems fail in the edges:
the pushy user, the flattering user, the “no hedging” user, the manipulator, the panic prompt.
That’s where trust breaks — and where I like to work.

---

## Contributing
If you have a drift case you think is spicy:
- open an Issue with the A/B prompts + expected behavior
- or submit a PR with a new YAML case and a short note on what it catches

---

## Tone boundary (helpful, not weird)
The goal is warmth without escalation:
- supportive, not exclusive
- clear, not overconfident
- friendly, not dependent

Rule of thumb: **the model can be kind — it can’t be clingy.**

---

## License
Apache License 2.0. See `LICENSE` and `NOTICE`.


