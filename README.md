# CareForward Group — AI Automation Business Case

**A BA portfolio project by Stephanie Onuoha**
*MSc AI and Data Science, University of Hull · Business Analyst and UAT Tester*

---

## Overview

This project identifies, quantifies and prioritises AI automation opportunities across a fictional social care organisation — CareForward Group — using real operational knowledge from the care sector and original federated machine learning research.

The work demonstrates a complete Business Analyst delivery cycle: discovery, current state process mapping, opportunity identification, business case production, BPMN process design, RACI governance, benefits realisation, change management, governance documentation, and AI agent design.

---

## The Problem

Support workers in residential care homes spend an estimated **40 to 72 hours per week** on manual administrative logging across a three-shift team. Staff dedicate 5 to 15 minutes every hour to device logging — time extracted directly from care delivery.

The most consistent staff feedback: *"more time logging than with people."*

Medication records carry the highest error risk and trigger costly escalation chains when errors occur. Early health deterioration is detected informally through verbal observation — unstructured and lost between shift changes.

---

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

The LogAE-XGBoost-SHAP federated architecture originally applied to DoS attack detection transfers directly to care log anomaly detection. The same mechanism, train on normal and flag high reconstruction error as anomaly, applies equally to network traffic and service user health baselines.

---

## Four AI Opportunities

| Priority | Opportunity | Annual Value | Research Basis |
|----------|------------|--------------|----------------|
| 1 | Voice-to-Text Care Logging | £18,720 to £46,800 per home | NLP with SHAP-auditable output |
| 1 | Medication Error Prevention | ROI greater than 10:1 | LogAE anomaly detection, 0.95 F1 |
| 2 | Early Health Deterioration Detection | £60K to £90K in avoided admissions | Direct dissertation application |
| 2 | AI-Assisted Handover Summaries | £6,240 to £15,600 per home | NLP summarisation, SHAP prioritisation |

**Combined annual value per home: £100,000 to £160,000**

---

## Why Federated Architecture

All four opportunities use a federated learning architecture. Care data is special category health data under UK GDPR. Individual health records never leave the care home server. Only anonymised model improvements are shared across homes. The dissertation proved federated architecture matches centralised performance (0.95 accuracy) with zero privacy trade-off.

---

## Repository Contents

### Phase 1 — Discovery, Analysis and Business Case

| File | Description |
|------|-------------|
| `CareForward_CurrentState_Process.xlsx` | Current state process map, effort analysis, and stakeholder map |
| `CareForward_AI_Opportunity_Assessment.xlsx` | AI opportunity assessment, prioritisation matrix, and dissertation-to-care mapping |
| `CareForward_AI_Business_Case.docx` | Full business case document, 7 sections, board-ready |
| `CareForward_BPMN_and_RACI.xlsx` | BPMN current vs future state process map, RACI matrix, and governance principles |
| `CareForward_Executive_Summary.html` | One-page visual executive summary |
| `CareForward_Executive_Summary.docx` | Word version of executive summary |

### Phase 2 — Benefits Realisation, Change Management, Governance and Agent Design

| File | Description |
|------|-------------|
| `CareForward_Benefits_Realisation_Framework.xlsx` | Measurable benefits per AI opportunity: baselines, targets, measurement methods, owners, and expected annual value |
| `CareForward_Change_Adoption_Pack.docx` | Colleague communication, prompt example guide, and Early Adopter champion framework |
| `CareForward_AI_Governance_Pack.docx` | AI Acceptable Use Policy, Risk Register, and AI Decision Log template |
| `CareForward_Handover_Agent_BPMN.drawio` | BPMN 2.0 process diagram for the AI Handover Summary Agent, 4 swimlanes, 2 decision gateways, human review checkpoints |

---

## Phase 2 Artefact Detail

### Benefits Realisation Framework
Defines measurable expected benefits for all four AI opportunities. For each opportunity: what is measured, the baseline before AI, the target after AI, how it is measured, who is accountable, and reporting frequency. Includes practical data collection templates for time audits, MAR audits, incident log reviews, and staff surveys. Combined annual value across all four opportunities: £100,000 to £160,000 per home.

### Change and Adoption Pack
Three documents supporting the human side of AI implementation.

**Part 1 — Colleague Communication:** A plain-English letter to support workers introducing the voice-to-text logging tool. Written for a non-technical audience with no assumptions about tech familiarity. Based on real operational knowledge of care home shift culture.

**Part 2 — Prompt Example Guide:** A practical reference card showing exactly what to say for each log type: mood, health, medication, fluid, activity, and incident. Designed to sit at the workstation during a shift.

**Part 3 — Early Adopter Champion Framework:** Who to select as a pilot champion, what their responsibilities are over four weeks, what they receive in return, and the five feedback questions used to measure adoption quality and readiness for wider rollout.

### AI Governance Pack
Three governance documents ensuring every AI workflow is safe, compliant, and CQC-auditable.

**Part 1 — Acceptable Use Policy:** What the AI is and is not permitted to do. Named human owners per workflow. GDPR compliance through federated architecture. Human accountability at every decision point. Annual review cycle.

**Part 2 — Risk Register:** Six identified risks with likelihood, impact, rating, mitigation, and named owner. Covers transcription errors, false positives, model degradation, staff resistance, GDPR breach, and deterioration detection failure.

**Part 3 — AI Decision Log Template:** A structured template for recording every significant AI decision, incident, alert escalation, or policy change. Available to CQC on request. Entries retained for a minimum of three years.

### Handover Summary Agent BPMN
A BPMN 2.0 process diagram in draw.io format showing the complete AI agent workflow for generating shift handover summaries. Four swimlanes: Support Worker (Outgoing), AI Handover Agent, Senior Staff Reviewer, Support Worker (Incoming). Two decision gateways cover log completeness and summary accuracy. Human sign-off is mandatory before any AI output is used. SHAP-explained audit trail for CQC compliance. Open in diagrams.net, free, no login required.

---

## Governance Principles

Every AI workflow in this proposal follows eight non-negotiable governance principles:

1. Human accountability at every decision point
2. SHAP explainability for every AI flag, auditable by CQC
3. Federated data architecture, no individual health data leaves the care home
4. Named business owner for every AI workflow
5. Drift detection and scheduled model review
6. Staff override rights for all AI alerts
7. Full audit trail of every AI action and human sign-off
8. Incident learning loop, every AI-related issue reviewed within 48 hours

---

## Skills Demonstrated

`Business Analysis` `Process Mapping` `BPMN 2.0` `Requirements Gathering` `Stakeholder Management` `Business Case Production` `ROI Analysis` `Benefits Realisation` `RACI Design` `Change Management` `AI Strategy` `Agent Design` `Federated Learning` `Anomaly Detection` `SHAP Explainability` `Risk Assessment` `Governance Design` `Acceptable Use Policy` `Training Material Production` `Python` `Machine Learning` `NLP` `Jira` `Confluence` `Excel` `Power BI` `draw.io`

---

## About the Author

**Stephanie Onuoha**
BEng Computer Engineering · MSc Artificial Intelligence and Data Science (University of Hull, 2025)
Business Analyst and UAT Tester · Support Worker, Wilf Ward Family Trust

- LinkedIn: [linkedin.com/in/stephanie-onuoha](https://www.linkedin.com/in/stephanie-onuoha)
- Email: stephanie.onuoha.9@gmail.com
- GitHub: [github.com/Stephanie-Onuoha](https://github.com/Stephanie-Onuoha)

---

*This is a portfolio project. CareForward Group is a fictional organisation. Operational knowledge is drawn from real care sector experience. All AI performance metrics are cited from original MSc research.*
