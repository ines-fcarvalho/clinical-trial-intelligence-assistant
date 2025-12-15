# Ablation Study — Organization & Execution

This project uses a single notebook (`ablations/notebooks/Ablation.ipynb`) to run ablations for phases I/II/III on datasets (CTOD/HINT). Outputs are saved into `ablations/results/`:

- `results/csv/`     per-phase CSVs (e.g., `ctod_phase_I_topk20.csv`)
- `results/plots/`   top-10 bar charts per phase (`ctod_phase_I_top10.png`, etc.)
- `results/excel/`   merged workbook (`ablation_summary.xlsx`)
- `logs/`            run metadata (timestamp, versions)

**How to run**
1) Open `ablations/notebooks/Ablation.ipynb`.
2) Set `USE_DATASET` and `PHASES`.
3) Run all cells. See `ablations/results/` for outputs.

**Notes**
- Inference-time ablation (zeroing columns), no retraining.
- Baselines are logged per phase.
- If feature-name JSON exists, CSVs include a `feature_name` column.
