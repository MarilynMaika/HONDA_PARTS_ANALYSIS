## Assessment Task: Please analyze the dataset provided and address the following:

- Compare the average total repair cost between different vehicle model
codes. Is there a relationship between the repair costs and the services
offered?
- Analyze the relationship between damage types and fix_type (repair vs.
replace). Which damage types are more likely to lead to part replacement
instead of repair?
- Evaluate the interaction between fix_type, parts, total repair cost,
and services rendered.


## 🧹 Data Cleaning Steps

- Missing **`unit_price_(vat_incl._16%)'** values imputed using model-specific medians.
- Total repair cost computed as `unit_price_(vat_incl._16%) * quantity`.
- Incomplete fix types (`'-'`) identified and handled.
- Making necessary changes to data types as well as renaming columns

##  General Conclusions
- Repair costs vary by model — Models like DBA-RM4 and DAA-RU3 are the most expensive to repair.

- Repairs are costlier than replacements — Especially in electrical and body service categories.

- Service category matters — Electrical and bodywork drive high repair costs; consumables and accessories are the cheapest.

- Some parts are mostly repaired, not replaced — e.g., interior, consumables.repaired.

## ✅ General recommendations
- Consider replacing over repairing for high-cost services to save time and labor.

- Improve diagnostics to avoid unnecessary, expensive repairs.

- Develop cost guidelines for high-cost models to standardize decisions.

- Fix missing fix_type entries to enhance future data analysis.

## 📁 Files

- `honda_parts_analysis.ipynb`: Main notebook with data cleaning, analysis, and visualizations.
- `honda_parts_data.csv`: Cleaned dataset.
- `output/plots/`: Folder with boxplots, heatmaps, and bar charts.

## 🚀 Tools Used

- Python (Pandas, Seaborn, Matplotlib)
- Jupyter Notebook




