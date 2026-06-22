## CareForward Group — AI Automation Business Case

A BA portfolio project by Stephanie Onuoha
MSc AI and Data Science, University of Hull · Business Analyst and UAT Tester

## Overview

This project identifies, quantifies and prioritises AI automation opportunities across a fictional social care organisation — CareForward Group — using real operational knowledge from the care sector and original federated machine learning research.

The work demonstrates a complete Business Analyst delivery cycle: discovery, current state process mapping, opportunity identification, business case production, BPMN process design, RACI governance, and executive communication.

## The Problem

Support workers in residential care homes spend an estimated **40 to 72 hours per week** on manual administrative logging across a three-shift team. Staff dedicate 5 to 15 minutes every hour to device logging — time extracted directly from care delivery.

The most consistent staff feedback: *"more time logging than with people."*

Medication records carry the highest error risk and trigger costly escalation chains when errors occur. Early health deterioration is detected informally through verbal observation — unstructured and lost between shift changes.

## Research Foundation

All AI recommendations are grounded in original MSc dissertation research:

**Zero Trust and Traditional Trust in Federated and Centralised Learning for DoS Attack Vectors**
*Stephanie Onuoha — University of Hull, August 2025*

| Metric | Result |
|--------|--------|
| Model Accuracy | 0.95 |
| F1-Score | 0.95 |
| AUC | 0.99 |
| SHAP Stability (Spearman rank) | 0.9934 |
| Low-confidence predictions | 0% across 21,871 classifications |
| Robustness under 30% feature corruption | F1 greater than 0.90 maintained |

The LogAE-XGBoost-SHAP federated architecture originally applied to DoS attack detection transfers directly to care log anomaly detection. The same mechanism — train on normal, flag high reconstruction error as anomaly — applies equally to network traffic and service user health baselines.

## Four AI Opportunities

| Priority | Opportunity | Annual Value | Research Basis |
|----------|------------|--------------|----------------|
| 1 | Voice-to-Text Care Logging | £18,720 to £46,800 per home | NLP with SHAP-auditable output |
| 1 | Medication Error Prevention | ROI greater than 10:1 | LogAE anomaly detection, 0.95 F1 |
| 2 | Early Health Deterioration Detection | £60K to £90K in avoided admissions | Direct dissertation application |
| 2 | AI-Assisted Handover Summaries | £6,240 to £15,600 per home | NLP summarisation, SHAP prioritisation |

**Combined annual value per home: £100,000 to £160,000**


## Why Federated Architecture

All four opportunities are implemented using a federated learning architecture for a specific, research-evidenced reason: care data is special category health data under UK GDPR.

- Individual health records never leave the care home server
- Only anonymised model improvements are shared across homes
- The dissertation proved federated architecture matches centralised performance (0.95 accuracy) with zero privacy trade-off
- Drift detection monitors each home's data distribution independently

## Repository Contents

| File | Description |
|------|-------------|
| `CareForward_CurrentState_Process.xlsx` | Current state process map, effort analysis, and stakeholder map |
| `CareForward_AI_Opportunity_Assessment.xlsx` | AI opportunity assessment, prioritisation matrix, and dissertation-to-care mapping |
| `CareForward_AI_Business_Case.docx` | Full business case document — 7 sections, board-ready |
| `CareForward_BPMN_and_RACI.xlsx` | BPMN current vs future state process map, RACI matrix, and governance principles |
| `CareForward_Executive_Summary.html` | One-page visual executive summary |
| `CareForward_Executive_Summary.docx` | Word version of executive summary |


## Artefact Highlights

### Current State Process Map
Nine-step swimlane map covering all three daily shifts (07:00 to 14:30, 14:00 to 21:00, 21:00 to 07:00). Actors: Night Staff, Day Staff, Medication Lead, Senior Staff, Manager. Pain points quantified per step. Effort analysis: 40 to 72 hours per week lost to manual logging.

### AI Opportunity Assessment
Four opportunities scored across six criteria: business value, staff impact, technical feasibility, compliance safety, speed to implement, and dissertation alignment. Includes a direct mapping of dissertation capabilities to care applications — showing exactly how LogAE anomaly detection, SHAP explainability, federated architecture, drift detection, and XGBoost classification transfer from cybersecurity to social care.

### BPMN Process Map — Current vs Future State
Side-by-side comparison of the manual process and the AI-enabled future state across 14 process steps and three decision gateways. Every future state activity shows the AI component (purple), the time saving (green), and the human accountability checkpoint preserved.

### RACI Matrix
23 activities across 8 roles including a dedicated AI System column. Governance principle: no AI activity is final without human sign-off. Every medication and clinical decision has a human as Accountable — AI holds no A roles.

### Executive Summary
One-page board-ready summary with headline stats, four opportunity cards with dissertation metrics, ROI summary, and architecture recommendation. Designed for LinkedIn sharing and portfolio showcasing.

## Governance Principles

Every AI workflow in this proposal follows eight non-negotiable governance principles:

1. Human accountability at every decision point
2. SHAP explainability for every AI flag — auditable by CQC
3. Federated data architecture — no individual health data leaves the care home
4. Named business owner for every AI workflow
5. Drift detection and scheduled model review
6. Staff override rights for all AI alerts
7. Full audit trail of every AI action and human sign-off
8. Incident learning loop — every AI-related issue reviewed within 48 hours

## Skills Demonstrated

`Business Analysis` `Process Mapping` `BPMN` `Requirements Gathering` `Stakeholder Management` `Business Case Production` `ROI Analysis` `RACI Design` `AI Strategy` `Federated Learning` `Anomaly Detection` `SHAP Explainability` `Risk Assessment` `Change Management` `Governance Design` `Python` `Machine Learning` `NLP` `Jira` `Confluence` `Excel` `Power BI`


## About the Author

**Stephanie Onuoha**
BEng Computer Engineering · MSc Artificial Intelligence and Data Science (University of Hull, 2025)
Business Analyst and UAT Tester · Support Worker (Wilf Ward Family Trust)

- LinkedIn: [linkedin.com/in/stephanie-onuoha](https://www.linkedin.com/in/stephanie-onuoha)
- Email: stephanie.onuoha.9@gmail.com
- GitHub: [github.com/Stephanie-Onuoha](https://github.com/Stephanie-Onuoha)

---

*This is a portfolio project. CareForward Group is a fictional organisation. Operational knowledge is drawn from real care sector experience. All AI performance metrics are cited from original MSc research.*
