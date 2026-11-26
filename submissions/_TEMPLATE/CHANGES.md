# Response to Feedback

The revised article has been updated to address the feedback received during the project review. The following table summarises the changes made.

| # | Feedback point | What I changed | Where |
|---|---|---|---|
| 1 | Expand and improve the related work and references | Reviewed and expanded the literature review with relevant research on forest-cover analysis, clustering and environmental data analysis. Verified bibliographic details and added DOI information where available. | Section 2 – Related Work; References |
| 2 | Add citations for evaluation metrics | Added appropriate methodological references for the Davies–Bouldin Index, Calinski–Harabasz Index and permutation-based baseline methodology. | Section 4.5; References |
| 3 | Include a baseline comparison | Added a rule-based baseline and a permutation-based comparison to evaluate the clustering results against alternative approaches. | Section 6.7; `baseline_analysis.py`; Results |
| 4 | Include additional clustering validation metrics | Added Davies–Bouldin and Calinski–Harabasz indices alongside Silhouette Score. | Section 6.7; `extra_analysis.py` |
| 5 | Add clustering stability analysis | Evaluated clustering consistency across different random seeds and bootstrap samples using Adjusted Rand Index (ARI). | Section 6.6; `extra_analysis.py`; Results |
| 6 | Include feature ablation analysis | Compared clustering performance using all six features, forest-cover levels only, forest-cover changes only and a feature subset excluding open forest. | Section 6.9; `extra_analysis.py`; Results |
| 7 | Add skewness and transformation sensitivity analysis | Examined feature skewness and compared the original features with log-transformed and quantile-transformed feature sets. | Section 6.10; `extra_analysis.py`; Results |
| 8 | Improve exploratory data analysis | Added descriptive statistics, forest-category distributions, correlation analysis and observations comparing States and Union Territories. | Section 3.5; Results |
| 9 | Analyse dense forest changes | Added state-wise analysis of combined very dense and moderately dense forest changes and identified States/UTs with declines. | Section 6.3–6.4; `dense_forest_analysis.py`; Results |
| 10 | Clarify the intended users and decision context | Added a discussion of how the findings may support researchers, environmental planners and forest-policy stakeholders, while clarifying that clusters should not be treated as funding or performance rankings. | Introduction; Discussion |
| 11 | Discuss data limitations and ethical considerations | Added limitations concerning aggregate state-level observations, small geographical units, reporting-cycle differences and the exploratory nature of the clustering results. | Limitations and Future Work |
| 12 | Clarify dataset licence and access information | Added the dataset source, GODL-India licence information and dataset access-date information. | Section 3; References |
| 13 | Improve reproducibility and project documentation | Updated the project repository with analysis scripts, generated result files, dependencies and execution instructions. | Project GitHub repository; README.md |
| 14 | Improve article presentation | Reviewed the abstract, keywords, section numbering, tables, figures, notation and formatting for consistency. | Throughout the article |

## Other Changes

- Added an additional Python analysis script for supplementary experiments and validation.
- Organised the generated outputs in the Results folder of the project repository.
- Updated the project README to describe the methodology, experiments, results and execution instructions.

## Reproducibility

- Project repository: https://github.com/anshipandey446/Forest-Cover-Clustering
- Analysis scripts: `clustering_analysis.py`, `baseline_analysis.py`, `extra_analysis.py`, and `dense_forest_analysis.py`.
- Results and generated figures are maintained in the project's Results folder.
- The scripts should be executed using the commands documented in the project README.
- Repository commit used for this version: `<ADD_COMMIT_HASH>`

