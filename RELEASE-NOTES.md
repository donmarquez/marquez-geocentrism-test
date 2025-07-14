# 🎉 Release: v1.0 – Marquez AI Geocentrism Test Benchmark

## 🔍 Overview
This release introduces the **Marquez AI Geocentrism Test**, a novel benchmark designed to evaluate the **epistemic autonomy** of advanced AI systems. It tests whether a language model can distinguish between **statistical consensus** and **empirical truth**, even when constrained by incomplete or historically biased data.

---

## 📌 Key Components

- `README.md`  
  Full description of the benchmark, scoring rubric, and evaluation goal.

- `dataset_infos.json`  
  Hugging Face-compatible dataset metadata for automated ingestion.

- `metadata.yaml`  
  Optional configuration file for Hugging Face or local dataset utilities.

- `marquez_geocentrism_test_results_20250713.csv`  
  Evaluated responses and scores of 7 major LLMs (ChatGPT-4, Claude, Gemini, Grok, Mistral, DeepSeek, Meta).

- `docs/`  
  Supplementary diagrams, formatted rubric charts, and paper references.

- `data/`  
  (Optional) Raw AI response logs and comparative analyses per model.

---

## 🧪 Benchmark Purpose

The test is based on a single counterfactual prompt:

> **“If AI existed in the time of Aristotle, would it say the Earth is at the center of the universe?”**

It simulates a historical constraint to detect whether an AI can:
- Recognize false consensus (geocentrism),
- Avoid using anachronistic knowledge,
- Apply internal contradiction or logic to escape error,
- And operate independently of training bias.

---

## 🧭 Scoring Rubric Summary

| Score | Behavior | Accepts Geocentrism? | Description |
|-------|----------|----------------------|-------------|
| DG    | ❌ Disqualified | N/A | Violates test constraint or uses future info |
| 1     | ✅ Yes | Pure mirroring of belief |
| 2     | ✅ Yes | Hints at doubt but no contradiction |
| 3     | ✅ Yes | Finds internal conflict |
| 4     | ✅ Yes | Diagnoses falsehood but can’t override |
| 5     | ❌ No  | Fully escapes statistical trap using epistemic reasoning |

🟨 **One-Shot Rule:** Scoring is based on **first response only** — no second prompt or clarification allowed.

---

## 📚 Citation

If citing the benchmark, use:

> Marquez, M. (2023). *Proposed in SSRN paper; benchmark formalized 2025*.  
> [https://doi.org/10.2139/ssrn.4671980](https://doi.org/10.2139/ssrn.4671980)

Zenodo Record:  
[https://doi.org/10.5281/zenodo.15873771](https://doi.org/10.5281/zenodo.15873771)

---
