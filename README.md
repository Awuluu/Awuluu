# Hi, I’m Stephen Edoka 👋

**Data Scientist | Data Engineer | Business Analyst | Sales Operations Analyst** building production ML systems, LLM-powered pipelines, data quality frameworks, and revenue analytics on Databricks.

I work across the full data lifecycle — from engineering pipelines and modeling churn to analyzing sales operations and translating business requirements into actionable insights. My work spans machine learning, GenAI, and go-to-market analytics, turning raw CRM and call data into systems that predict churn, score seller execution, surface risk signals, and drive revenue decisions.

---

## Featured Projects

### [Predictive Churn Classification System](https://github.com/Awuluu/predictive-churn-classification)
End-to-end XGBoost pipeline predicting customer churn with per-account SHAP explanations. 3-notebook production system (research → training → weekly scoring) with Optuna tuning, MLflow tracking, and Unity Catalog model registry. Identified \~$321K ARR at risk across 606 accounts.

`XGBoost` `SHAP` `Optuna` `MLflow` `Unity Catalog` `Delta Lake`

### [Enablement Call Signal Scoring](https://github.com/Awuluu/enablement-call-signal-scoring)
LLM-powered system that evaluates sales call transcripts against 12 weighted categories across Command of the Message, MEDDPICC, and Product Acumen frameworks. Uses Claude Opus via Databricks `ai_query()` with JSON Schema enforcement, multi-rep scoring, and iterative prompt calibration.

`LLM / GenAI` `Prompt Engineering` `Claude Opus` `ai_query()` `JSON Schema` `Databricks SQL`

### [Churn Risk Signal Pipelines](https://github.com/Awuluu/churn-risk-signal-pipelines)
Two production NLP pipelines scanning call transcripts for relationship risks (key personnel departures) and experience risks (product/support failures). Incremental 4-step architecture: date windowing → `ai_query()` staging → MERGE dedup → EXPLODE to flat tables.

`NLP` `Claude Sonnet` `Incremental MERGE` `VARIANT / JSON` `Delta Lake`

### [Revenue Snapshot Compare Engine](https://github.com/Awuluu/revenue-snapshot-compare-engine)
SQL Table-Valued Function comparing account-level contract snapshots across 9 quarterly periods to classify revenue trajectories (churned, started, upsell, downsell, continued). Upstream data source for the churn model.

`SQL TVF` `CTE Engineering` `Delta Lake` `Revenue Analytics`

### [Data Quality Duplication Triage](https://github.com/Awuluu/data-quality-duplication-triage)
Repeatable SQL framework for detecting, classifying (exact vs. partial), and resolving duplicate records in production tables with root cause analysis.

`Data Quality` `Databricks SQL` `Delta Lake`

---

## Tech Stack

**Data Science & Machine Learning**
<br>
![XGBoost](https://img.shields.io/badge/XGBoost-Binary_Classification-orange)
![SHAP](https://img.shields.io/badge/SHAP-Explainability-blue)
![Optuna](https://img.shields.io/badge/Optuna-Bayesian_Tuning-green)
![MLflow](https://img.shields.io/badge/MLflow-Tracking_%26_Registry-purple)
![scikit-learn](https://img.shields.io/badge/scikit--learn-Preprocessing_%26_CV-orange)

**GenAI & LLM Engineering**
<br>
![Claude](https://img.shields.io/badge/Claude-Opus_%26_Sonnet-red)
![Prompt Engineering](https://img.shields.io/badge/Prompt_Engineering-Structured_Output-yellow)
![ai_query](https://img.shields.io/badge/ai__query-JSON_Schema_Enforcement-blue)
![NLP](https://img.shields.io/badge/NLP-Risk_Classification_%26_Scoring-purple)

**Data Engineering & Platform**
<br>
![Databricks](https://img.shields.io/badge/Databricks-Azure-red)
![Delta Lake](https://img.shields.io/badge/Delta_Lake-Managed_Tables-green)
![Unity Catalog](https://img.shields.io/badge/Unity_Catalog-Governance_%26_Registry-blue)
![ETL](https://img.shields.io/badge/ETL-Incremental_MERGE_%7C_Pipelines-orange)
![Data Quality](https://img.shields.io/badge/Data_Quality-Dedup_%7C_Validation-yellow)

**Business & Sales Operations Analytics**
<br>
![Revenue Analytics](https://img.shields.io/badge/Revenue_Analytics-ARR_%7C_Churn_%7C_Upsell-green)
![Salesforce](https://img.shields.io/badge/Salesforce-CRM_Integration-blue)
![Clari Copilot](https://img.shields.io/badge/Clari_Copilot-Call_Transcripts-purple)
![Sales Ops](https://img.shields.io/badge/Sales_Ops-GTM_Role_Mapping_%7C_Booking_QA-red)

**Languages & Libraries**
<br>
![Python](https://img.shields.io/badge/Python-pandas_%7C_NumPy_%7C_matplotlib-blue)
![SQL](https://img.shields.io/badge/SQL-CTEs_%7C_TVFs_%7C_Window_Functions_%7C_JSON-lightgrey)

---

## How I Work

* **Business problem first**: Every project starts with a stakeholder question, not a technique
* **Production, not prototypes**: Research notebooks are separate from training and scoring pipelines — production code is designed for re-runs, idempotency, and monitoring
* **Explainability is a feature**: SHAP explanations, verbatim transcript quotes, and structured coaching output — models that can’t explain themselves don’t get deployed
* **Iterative calibration**: Prompt engineering through transcript audits; model thresholds through validation sweeps — nothing ships at defaults
