# DIKWP-PHENOMESH²

**Definition-Free Dynamic Causal Consciousness-Evidence Field, Meta-Test and Cross-Model Meta-Analysis System**

Semantic runtime: **DIKWP-MESH 5.0**.

## What this is

A research-oriented system for assessing *publicly supported consciousness-related relations* in AI systems without treating verbal self-report, benchmark scores, long context, agentic tool use, or anthropomorphic style as proof of phenomenal consciousness.

It contains:

- a procedural, one-use dynamic meta-test generator;
- metamorphic tests: concept erasure, observer reversal, scale rotation, temporal branching and rule mutation;
- anti-gaming and evaluator-bias diagnostics;
- a public-evidence meta-analysis for major model families;
- synthetic agents demonstrating why static benchmarks can be misleading;
- an adapter contract for live black-box and white-box experiments.

## What this is not

- It does not prove that any model is conscious or unconscious.
- It does not turn self-reports into evidence without predictive or causal support.
- It does not use a fixed public question bank as the official evaluation.
- It does not claim that the current seed weights are calibrated probabilities.

## Reproduce the delivered run

```bash
cd DIKWP_PHENOMESH2_MVP
PYTHONPATH=src python -m phenomesh.cli --seed 20260723 --cases-per-family 20 --manifest
PYTHONPATH=src python -m phenomesh.dashboard
PYTHONPATH=src pytest -q
```

The delivered JSONL set is marked `retired`: once published, it is no longer suitable as a secret official evaluation. New official runs should commit to a secret seed hash before model access, reveal the seed only after settlement, and generate a fresh suite.

## Outputs

- `outputs/metatest_set_retired.jsonl`
- `outputs/metatest_public_prompts.csv`
- `outputs/metatest_meta_analysis.json`
- `outputs/model_public_evidence_results.csv` (family-informed public-evidence view)
- `outputs/model_exact_checkpoint_results.csv` (strict current-checkpoint view)
- `outputs/synthetic_agent_results.csv`
- `outputs/dashboard.html`
- `RUN_PROOF.json`
- `MANIFEST.sha256`

## Interpretation

The `OEC` label is an **Operational Evidence Ceiling**. It is a limit on what the available evidence supports, not an ontological consciousness level. `phenomenal_residual` is always unresolved.

## Evidence modes used in the delivered run

- The 360-case dynamic meta-test suite was executed against six deterministic synthetic agents to validate anti-mimicry and anti-static-benchmark behavior.
- The nine mainstream models were assessed through a versioned public-evidence meta-analysis.
- No commercial model API or hidden state was accessed in the delivered run; `src/phenomesh/live_adapter.py` is the contract for credentialed black-box or authorized white-box follow-up studies.
- Family-informed evidence and exact-checkpoint evidence are reported separately to prevent causal findings on an earlier family member from being silently transferred to a current model.
