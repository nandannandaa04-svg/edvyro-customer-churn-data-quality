# EdVyro Customer Churn — Task 02 Submission Package

This package is prepared for **Data Quality and Exploratory Analysis**.

## Included
- `customer_churn_data_quality_analysis.ipynb` — reproducible Colab/Jupyter analysis.
- `README.md` — submission instructions.
- `requirements.txt` — packages used.

## Run in Google Colab
1. Open Google Colab: https://colab.research.google.com/
2. Upload `customer_churn_data_quality_analysis.ipynb`.
3. Run **Runtime → Run all**.
4. The notebook first downloads the supplied EdVyro dataset from:
   `https://edvyro.in/datasets/customer_churn_sample.csv`
5. If direct CSV download is blocked, the notebook opens an upload prompt. Upload the **exact supplied `customer_churn_sample.csv`**.
6. Confirm `ALL VALIDATION CHECKS PASSED`.

## Generated deliverables
The notebook creates `customer_churn_outputs/` containing:
- `customer_churn_cleaned.csv`
- `data_quality_summary.csv`
- `data_profile.csv`
- `cleaning_log.csv`
- `validation_checks.csv`
- `outlier_audit.csv`
- summary-statistics and churn-segment CSVs
- PNG charts
- `customer_churn_data_quality_report.xlsx`
- `submission_report.md`

## Submission
Put the notebook and the generated `customer_churn_outputs` folder in one GitHub repository, Google Drive folder, or other public/view-only location. Submit that single link to EdVyro.

## Important data-quality choices
- Missing/invalid required records are excluded rather than silently imputed.
- Exact duplicate rows are removed.
- Duplicate customer IDs are logged and the first record is retained because the source guide defines `customer_id` as a synthetic unique identifier.
- IQR outliers are flagged but not automatically removed because an extreme observation can still be valid.
- Descriptive associations are not presented as causal claims.

## Source requirements
The analysis follows the EdVyro guide: profile missing values, duplicates and outliers; document cleaning decisions; validate the final dataset; and inspect meaningful distributions.
