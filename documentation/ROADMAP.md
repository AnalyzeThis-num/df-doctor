# 🧭 df-doctor — Roadmap

This roadmap outlines the planned evolution of the `df-doctor` library, from lightweight numeric diagnostics to an intelligent, full-spectrum data sanity assistant.

---

## ✅ v1.0 — Numeric DataFrame Diagnostics (MVP)
> **Status:** In development  
**Focus:** Diagnose `.csv` files with numeric data

- [x] Analyze missing values, dtypes, constants, duplicates
- [x] Flag zero-variance columns
- [x] Heuristic checks based on column names (e.g., "date" → suggest datetime)
- [x] Non-destructive fix suggestions
- [x] Return summary report as DataFrame
- [ ] Add installation instructions and simple usage docs

---

## 🔄 v1.1 — Enhancements & Edge Cases
> **Status:** Planned  
**Focus:** Improve detail and add optional CLI tool

- [ ] Detect outliers using IQR or z-score
- [ ] Flag multicollinearity via correlation matrix
- [ ] Add logging + warning system
- [ ] Optional CLI wrapper for advanced users

---

## 🌱 v2.0 — Support for Categorical & Boolean Data
> **Status:** Planned  
**Focus:** Handle more than numeric columns

- [ ] Detect and summarize categorical columns
- [ ] Flag high-cardinality features
- [ ] Auto-detect likely boolean columns (`is_`, `has_`, etc.)
- [ ] Recommend encoding options

---

## 🧠 v3.0 — Text & Fuzzy Header Intelligence
> **Status:** Planned  
**Focus:** Introduce lightweight text analysis

- [ ] Identify free-text columns via average char count
- [ ] Flag mixed data types in `object` columns
- [ ] Fuzzy match column names to expand heuristic rules
- [ ] Generate frequency tables for top values in text columns

---

## 🛠️ v4.0 — Auto-Fix Engine (Configurable)
> **Status:** Planned  
**Focus:** Apply fixes using customizable logic

- [ ] Create `df_doctor.clean(df, config="safe")` interface
- [ ] Profiles: safe / moderate / aggressive
- [ ] Interactive fix approval option
- [ ] Log all changes made to a `.json` or `.md` audit file

---

## 📊 v5.0 — Visual Diagnostic Dashboard
> **Status:** Planned  
**Focus:** Provide visual interface for quick EDA

- [ ] Streamlit or Gradio dashboard version
- [ ] Visual summaries: null heatmaps, distributions, type charts
- [ ] Export visual reports

---

## 🧪 v6.0 — Model Readiness Checks
> **Status:** Planned  
**Focus:** Prep data for ML pipelines

- [ ] Detect and warn about leakage (e.g., label leakage)
- [ ] Validate target variable (e.g., binary vs regression)
- [ ] Flag common modeling issues: skew, imbalance, cardinality
- [ ] Recommend next steps for ML prep

---

## 🤖 v7.0 — Smart Fix Suggestions (ML-based)
> **Status:** Long-term  
**Focus:** Data-aware auto recommendations

- [ ] Build internal recommender system for fix patterns
- [ ] Learn from user behavior across sessions
- [ ] Simulate expected results of applying certain fixes
- [ ] Auto-prioritize what needs review most

---

Have ideas or want to contribute? [Open an issue](https://github.com/yourusername/df-doctor/issues) or start a discussion!
