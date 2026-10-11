# Data dictionary

## Figure source data

Files are grouped by figure identifier and analysis role. CSV files contain the plotted values, parcel-level diagnostic attributes, confusion matrices, routing weights, uncertainty measures, or representative-case summaries. The Excel file duplicates the corresponding routing-strategy CSV for convenient inspection.

## Evaluation splits

Each task has a JSON metadata file and an NPZ index file. Task names encode the protocol, fold or held-out region, seed, and label budget. For example, `spatial0_seed11_n1000` denotes spatial fold 0, seed 11, and a 1,000-parcel training budget.

## Analysis results

- `final_cmcr_1000`: frozen 1,000-label CMCR evaluation and matched baseline comparisons.
- `all_label_budgets`: task metrics and paired comparisons across all label budgets.
- `mechanism_analysis`: class, region, route-specialization, and task-level mechanism summaries.
- `budget_aware_workflow`: final label-budget-aware workflow results.
- `source_availability`: reduced-expert inference results when a source family is unavailable.
- `core_validation`: competence-supervision, matched uniform-routing, HEA component, calibration, and spatial-sensitivity analyses.

All percentages stored as proportions should be multiplied by 100 for percentage-point presentation unless the corresponding column name explicitly contains `_pp`.
