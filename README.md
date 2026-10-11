# Urban-TabM

Processed research data accompanying **Urban-TabM: Multisource Expert Learning for Parcel-Level Urban Land-Use Classification With Limited Labels and Geographic Transfer**.

## Repository contents

- `data/figure_source_data/`: numerical and parcel-level source data used to produce the manuscript figures and tables.
- `data/evaluation_splits/`: frozen spatial fivefold and leave-one-region-out train/test index files for label budgets of 100, 300, and 1,000 parcels and seeds 11, 23, and 37.
- `data/analysis_results/`: aggregate model comparisons, class and region analyses, routing diagnostics, source-removal results, calibration results, and targeted ablations.
- `config/hyperparameters.json`: final HEA and CMCR training configuration.
- `MANIFEST.csv`: file sizes and SHA-256 checksums for the public release.

## Scope and third-party inputs

This repository contains processed data and derived evaluation outputs needed to verify the values reported in the article. It does not redistribute raw satellite imagery, raw point-of-interest records, original building and road layers, pretrained DINOv2 weights, or the complete MSLU-100K source dataset. Those inputs remain governed by their original providers and licenses.

The evaluation split files store array indices used by the frozen experiments. The figure source files include only the processed attributes required for the published visualizations and statistical summaries.

## Reproducibility notes

- Development regions: Beijing, Tianjin, Shanghai, and a selected Pearl River Delta area.
- External evaluation cities: Chengdu, Wuhan, and Xi'an.
- Target classes: residential, commercial, public service, industrial, and agricultural/natural land.
- Evaluation protocols: spatial fivefold and leave-one-region-out evaluation.
- Label budgets: 100, 300, and 1,000 parcels.
- Sampling seeds: 11, 23, and 37.

## Citation

Please cite the associated article when using these materials. Full bibliographic information will be added after publication.

## Contact

Xintian Liu  
Department of Urban Planning and Design, The University of Hong Kong  
xintianliu@connect.hku.hk
