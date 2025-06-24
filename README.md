# 🩺 df-doctor

**df-doctor** is a lightweight Python library for diagnosing and cleaning numeric pandas DataFrames. It helps data analysts quickly identify common data issues such as missing values, bad data types, duplicates, and naming inconsistencies — and provides smart, non-destructive suggestions for fixes.

---

## 🔧 Installation

```bash
pip install df-doctor  # (coming soon)
```

---

## 🚀 Quick Start

```python
import pandas as pd
import df_doctor

# Load your CSV and give it a descriptive name
survey_df = pd.read_csv("survey_data.csv")

# Run diagnostics
report = df_doctor.analyze(survey_df)

# (Optional) View fix suggestions
fixes = df_doctor.suggest_fixes(report)

# (Optional) Clean the data non-destructively
clean_df = df_doctor.clean(survey_df, fixes)
```

---

## ✅ Recommended Naming Tip

While `df_doctor` functions use `df` as a parameter name, we recommend **naming your DataFrame descriptively** in your own work — for example:

```python
description_df = pd.read_csv("job_descriptions.csv")
cleaned_df = df_doctor.clean(description_df)
```

This helps clarify context in notebooks and scripts.

---

## 📋 Features (v1.0)

- Analyze missing values, bad dtypes, constant columns, duplicates
- Flag object columns with numeric or date-like values
- Clean column names (remove special characters, spaces)
- Provide a simple fix suggestion report
- Never overwrites your data — fixes are returned as a new DataFrame

---

## 🗺️ Roadmap

Future versions will support categorical columns, lightweight NLP, outlier detection, visual dashboards, and automated ML-readiness checks. See [ROADMAP.md](./ROADMAP.md) for full plan.

---

## 📄 License
MIT License
# df-doctor
