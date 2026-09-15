# Phase 3 — MacroOps AI
## Overview
MacroOps AI is an AI-assisted operations intelligence platform designed to help operations teams monitor performance, identify operational exceptions, assess SLA risk, retrieve relevant operational knowledge, and receive contextual recommendations.
The Phase 3 prototype is built using synthetic operational data and a modular Python architecture.

## Core MVP
The MVP consists of:
- Operations Dashboard
- SLA Monitoring
- Exception Management
- RAG Knowledge Assistant
- AI Operations Copilot

Data Sources
The platform integrates:
Orders
Inventory
Picking
Delivery
Workforce
These datasets are combined using common identifiers such as order_id and store_id to create an integrated operational dataset.

Key Capabilities
Operations Analytics
Tracks KPIs such as:
SLA Breach Rate
On-Time Rate
Delivery Delay
Inventory Accuracy
Picking Duration
Assignment Delay
SLA Risk

A machine-learning model is used to identify potential SLA-risk orders and support operational prioritization.
Exception Management
The prototype identifies:
SLA breaches
Inventory / picking issues
Assignment delays
RAG Knowledge Assistant

Retrieves relevant information from the operational knowledge base and provides source-supported answers to natural-language questions.
AI Operations Copilot
Combines operational information and retrieved knowledge to provide contextual recommendations to operations users.
Architecture
Operational Data
      ↓
Data Pipeline
      ↓
Integrated Dataset
      ↓
Analytics + ML
      ↓
Dashboard / Exceptions / RAG
      ↓
Operations Copilot
Repository Structure
phase3_submission/
├── data/
├── src/
├── models/
├── outputs/
├── docs/
├── tests/
├── overleaf/
├── requirements.txt
└── README.md

Technologies
Python
Pandas
NumPy
Scikit-learn
Streamlit
RAG
Gemini
Joblib
Git / GitHub
Prototype Status

The current implementation is a prototype using synthetic operational data. It is intended for demonstrating the architecture, analytics, ML, RAG and Copilot workflow rather than representing real-world operational performance.

Future Scope
Improved SLA prediction
Real operational data integration
Advanced AI agents
Voice interaction
Computer vision
Multilingual assistance
Multi-agent Operations Copilot

Author
M. Ayshwarya
