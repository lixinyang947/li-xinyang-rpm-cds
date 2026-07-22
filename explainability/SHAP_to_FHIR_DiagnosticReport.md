# SHAP Explanation to FHIR DiagnosticReport Framework

## Overview

This document describes the explainability layer of the RPM-CDS framework.

The framework converts machine-learning feature attribution into a structured clinical artifact using HL7 FHIR R4.

---

# Explainable AI Workflow

---

# SHAP Attribution Model

For each prediction event:

The framework records:

- Predicted risk level
- Important contributing features
- Direction of contribution
- Clinical interpretation
- Timestamp
- Patient context

---

# FHIR Representation

Explanation outputs are represented as:

FHIR R4 DiagnosticReport resources.

The DiagnosticReport contains:

- Risk interpretation
- Supporting observations
- Feature contribution summary
- Explanation narrative

---

# Clinical Workflow Integration

The generated explanation artifact supports:

- Clinician review
- Alert interpretation
- Decision support workflow
- Auditability

---

# Design Principle

The framework treats explainability as a clinical interoperability artifact rather than an isolated analytical visualization.
