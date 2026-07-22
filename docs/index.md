# Explainable Risk-Stratification and Clinical Decision-Support Framework for Remote Patient Monitoring

## FHIR R4 + Machine Learning + Explainable AI

This site presents the public documentation portal for the RPM-CDS framework developed by Xinyang Li.

The framework integrates remote patient monitoring data, HL7 FHIR R4 normalization, machine-learning risk prediction, explainable artificial intelligence, and clinical decision-support workflows.

---

# Technical Scope

The framework includes:

- FHIR Observation based device data normalization
- Physiological feature engineering
- Machine-learning risk stratification
- XGBoost risk model with calibration
- SHAP-based explanation generation
- FHIR DiagnosticReport representation
- Context-aware CDS workflow

---

# Architecture
    |
    v
    |
    v
    |
    v
    |
    v
    |
    v
    |
    v
    
---

# Validation Status

Current status:

Draft / Experimental Technical Specification


Validation pathway:

- Retrospective validation using MIMIC-IV
- Benchmark comparison against threshold-based alerting
- Prospective RPM pilot validation pathway


---

# Documentation

- [Methodology](methodology.md)
- [Architecture](architecture.md)
- [Model Card](model-card.md)
- [Validation](validation.md)

---

# Author

Xinyang Li
