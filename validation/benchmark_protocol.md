# RPM-CDS Validation Benchmark Protocol

## Overview

This document defines the validation methodology for the explainable risk-stratification and clinical decision-support framework.

The validation strategy includes retrospective benchmarking and prospective validation planning.

---

# Phase 1: Retrospective Validation

## Dataset

MIMIC-IV public critical-care dataset.

Population:

- Adult ICU patients
- First ICU stay
- Length of stay ≥24 hours


---

# Prediction Task

Primary endpoint:

24-hour composite deterioration event:

- In-hospital death
- New invasive ventilation
- New vasopressor initiation


---

# Model Evaluation

The framework compares:

## Baseline

Static threshold-based alerting:

- Vital sign thresholds
- Conventional alert rules


## Proposed Method

Machine-learning risk stratification:

- XGBoost model
- Probability calibration
- SHAP explanation generation


---

# Evaluation Metrics

Metrics include:

- AUROC
- AUPRC
- Brier score
- Alert precision
- False-positive rate
- Calibration performance


---

# Reproducibility

Each experiment run should record:

- Dataset version
- Code version
- Model parameters
- Random seed
- Generated metrics


Manual entry of performance results is prohibited.

All reported metrics must originate from executable experiment runs.

---

# Limitations

Current validation represents:

- Retrospective research validation
- Simulation-based benchmarking
- Literature-supported comparison

It does not represent completed clinical deployment.

Prospective RPM pilot validation is required for real-world assessment.
