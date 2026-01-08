# Public Sector Record Linkage Framework
### Powered by Splink (UK Ministry of Justice)

## Overview
This repository demonstrates a non-intrusive, privacy-preserving framework for linking citizen records across disparate public sector data silos (e.g., Housing and Benefits systems). 

By utilizing **Probabilistic Matching** (the Fellegi-Sunter model), we can resolve duplicate identities caused by typos or nicknames without manual intervention or expensive infrastructure changes.

## Why this approach?
* **UK Government Standard:** Built on Splink, the open-source library developed by the **Ministry of Justice**.
* **Zero Software Cost:** Utilizes open-source Python tools.
* **Security First:** Designed as a "Read-Only Overlay" to run within secure environments like **Azure Data Factory**.

## Repository Structure
- `notebooks/`: Contains the data generation and matching logic.
- `data/`: Placeholder for synthetic datasets (secured via .gitignore).
- `Technical_Concept_Citizen_Record_Linkage.pdf`: The executive-level proposal.

## Getting Started
1. Install dependencies: `pip install -r requirements.txt`
2. Run `notebooks/02_Record_Linkage_Pilot.ipynb` to see the matching engine in action.
