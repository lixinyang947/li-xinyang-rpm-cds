# Explainable Risk-Stratification and Clinical Decision-Support Framework for Remote Patient Monitoring

## Overview

This repository presents the Remote Patient Monitoring (RPM) explainable risk-stratification and clinical decision-support framework developed by Xinyang Li.

The framework integrates:

- HL7 FHIR R4 data normalization
- physiological feature engineering
- machine-learning risk prediction
- explainable AI
- clinical decision-support workflow integration


## Technical Contribution

The framework transforms patient-generated health data into explainable clinical decision-support artifacts.

Key components include:

- FHIR Observation based data ingestion
- approximately 80-feature physiological data model
- calibrated XGBoost risk model
- SHAP-based explanation generation
- FHIR DiagnosticReport representation
- context-aware CDS workflow


## Architecture
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
    

## Validation Status

Current status:

Draft / Experimental Technical Specification


Validation approach:

- Retrospective validation using public datasets
- Benchmark comparison against threshold-based alerting
- Prospective RPM pilot validation pathway


## Repository Structure


## Author

Xinyang Li


## Citation

Xinyang Li.

Explainable Risk-Stratification and Clinical Decision-Support Framework for Remote Patient Monitoring.

Version 0.1.0.

GitHub Repository, 2026.
