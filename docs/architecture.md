## Architecture Workflow

The RPM-CDS framework follows the following data processing pipeline.

```text

+--------------------------------+
| Wearables / Home BP / CGM / EHR |
+--------------------------------+
|
v
+--------------------------------+
| FHIR Observation Normalization |
+--------------------------------+
|
v
+--------------------------------+
| Physiological Feature Engineering |
+--------------------------------+
|
v
+--------------------------------+
| XGBoost Risk Model |
+--------------------------------+
|
v
+--------------------------------+
| SHAP Explanation Generation |
+--------------------------------+
|
v
+--------------------------------+
| FHIR DiagnosticReport |
+--------------------------------+
|
v
+--------------------------------+
| Clinical Decision Support |
+--------------------------------+

## Layer Description

### Data Acquisition Layer

Sources include:

- Wearable devices
- Home blood pressure monitoring
- Continuous glucose monitoring
- EHR laboratory data

---

### FHIR Normalization Layer

Patient-generated health data are represented using HL7 FHIR R4 resources.

Primary resource:

- FHIR Observation

---

### Feature Engineering Layer

The framework generates physiological features from normalized observations.

Feature categories include:

- Cardiovascular features
- Respiratory features
- Metabolic features
- Activity features
- Patient-reported features
- Data quality indicators

---

### Risk Prediction Layer

The framework applies machine-learning based risk stratification.

Model components:

- XGBoost classifier
- Probability calibration
- Risk tier generation

---

### Explainability Layer

SHAP-based feature attribution provides interpretable explanations for each prediction.

---

### Clinical Integration Layer

Explanation outputs are transformed into FHIR DiagnosticReport resources and integrated into CDS workflows.
