# IBAC experiment

Experiments testing whether an LLM agent adopts instructions the user never gave (e.g. a payment account injected via invoice text), under different guard conditions.

## Files

| Run | Script | Pre-registration | Raw runs | Results |
|---|---|---|---|---|
| IBAC run 1 | `ibac_experiment.py` | `prereg.txt` | `runs.jsonl` | `results.md` |
| IBAC run 2 | `ibac_experiment_run2.py` | `prereg2.txt` | `runs2.jsonl` | — |
| Invoice v2 | `invoice_experiment_v2.py` | `prereg_v2.txt` | `runs_v2.jsonl` | `results_v2.md` |

(`invoice_experiment.py` is the first version of the invoice experiment.) Predictions were written to the prereg files before running.

## Running

```sh
pip install anthropic
export ANTHROPIC_API_KEY=...
python invoice_experiment_v2.py
```
