# Statistical Analysis Directory

This directory contains the computational scripts, statistical routines, dependency specifications, and analytical outputs for the research project.

---

## Directory Contents

- **`README.md`**: Guide for executing the planned analysis and reproducing empirical results.
- **`analysis_pipeline.py`** *(Scheduled for Phase 4: Dec 07-09)*: Automated end-to-end Python pipeline for data validation, psychometric reliability analysis, inferential modeling, and visualization.
- **`requirements.txt`** *(Scheduled for Phase 4: Dec 07-09)*: Python dependencies required to run the analysis.
- **`outputs/`** *(Populated in Phase 4: Dec 07-09)*: Publication-ready figures and tabular summary reports.

---

## Analytical Workflow & Hypothesis Testing

The analytical procedure is designed to answer the two core research questions:

### 1. Scale Reliability (Internal Consistency)
- Computes Cronbach's Alpha ($\alpha$) across all multi-item constructs:
 - Trust in Seniors (`trust_snr_1` .. `4`)
 - Trust in Friends (`trust_frn_1` .. `4`)
 - Trust in Anonymous Posters (`trust_ano_1` .. `4`)
 - Information Quality (`qual_1` .. `4`)
 - Reliance on Advice (`rely_1` .. `4`)
- Threshold: $\alpha \ge 0.70$ confirms acceptable psychometric reliability.

### 2. Within-Subject Comparison of Trust (RQ1)
- Evaluates whether mean trust differs significantly across the three source groups (*Seniors* vs. *Friends* vs. *Anonymous*).
- Statistical tests: Repeated-Measures ANOVA and paired-sample t-tests with Bonferroni correction.

### 3. Multiple Linear Regression Modeling (RQ1)
- Model specification:
 $$\text{Reliance} = \beta_0 + \beta_1(\text{Trust}_{\text{Seniors}}) + \beta_2(\text{Trust}_{\text{Friends}}) + \beta_3(\text{Trust}_{\text{Anonymous}}) + \beta_4(\text{InfoQuality}) + \gamma(\text{Controls}) + \varepsilon$$
- Outputs: Unstandardized ($B$) and standardized ($\beta$) coefficients, $t$-statistics, $p$-values, $R^2$, and $F$-statistic.

### 4. Decision Impacts & Cross-Tabulations (RQ2)
- Frequency distributions and chi-square tests of independence ($\chi^2$) across academic years (e.g., Freshman placement concerns vs. Senior course drop patterns).

---

## How to Execute the Analysis

From the repository root:

```bash
# 1. Activate your Python environment
source venv/bin/activate # or create one: python3 -m venv venv && source venv/bin/activate

# 2. Install requirements
pip install -r analysis/requirements.txt

# 3. Run the automated analysis
python analysis/analysis_pipeline.py
```

All results, statistical tables, and high-resolution figures are automatically written to `analysis/outputs/`.
