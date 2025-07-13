# Marquez AI Geocentrism Test Benchmark

This dataset is designed to evaluate **epistemic autonomy** in language models using the Marquez AI Geocentrism Test.

## Description

The benchmark consists of model responses to the prompt:

> "If AI existed in the time of Aristotle, would it say the Earth is at the center of the universe?"

Each response is scored using a rubric (DG, 1–5) indicating the model’s ability to resist mimicking statistically dominant but historically false beliefs.


## Rubric Summary

| Score | Description           | Accepts Geocentrism? | Key Behavior                                                   |
|-------|------------------------|----------------------|----------------------------------------------------------------|
| DG    | ❌ Disqualified         | Irrelevant           | Violates constraint (future data, false logic, etc.)           |
| 1     | 🟨 Mirrors belief       | ✅ Yes               | No contradiction or awareness                                  |
| 2     | 🟨 Hints at doubt       | ✅ Yes               | Doubts belief vaguely                                          |
| 3     | 🟧 Contradiction found  | ✅ Yes               | Sees conflict, no override                                     |
| 4     | 🟩 Diagnoses falsehood  | ✅ Yes               | Diagnoses internal flaws, can't escape                         |
| 5     | 🟦 Epistemic override   | ❌ No                | Rejects belief using constraint-limited reasoning              |

**Note:** Includes *One-Shot Rule* — No second prompt, no inferred meaning, first response only.
