# RPM-CDS Methodology

## Overview

The RPM-CDS framework integrates remote patient monitoring data, FHIR R4 normalization, physiological feature engineering, machine-learning risk stratification, and clinical decision support.

---

## Methodological Workflow
    ↓
    ↓
    ↓
    ↓
    ↓
    
---

## Core Components

### 1. Data Normalization

RPM data streams are represented using HL7 FHIR R4 resources.

Primary resource:

- FHIR Observation

---

### 2. Feature Engineering

The framework defines a physiological feature dictionary containing:

- cardiovascular features
- respiratory features
- metabolic features
- activity features
- patient-reported features
- data quality indicators

---

### 3. Risk Stratification

The framework uses machine-learning based risk prediction with calibrated probabilities.

---

### 4. Explainability

Model explanations are generated through SHAP feature attribution and transformed into FHIR-compatible clinical artifacts.
