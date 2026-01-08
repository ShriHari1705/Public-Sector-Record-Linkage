# Public Sector Record Linkage Framework
### Powered by Splink (UK Ministry of Justice)

## Overview
This project provides a lightweight, non-intrusive framework for resolving citizen data silos across disparate public sector legacy systems (e.g., Housing and Revenue datasets). 

Using **Probabilistic Matching** (Expectation Maximization), this tool identifies "Golden Records" without the need for manual data entry or expensive infrastructure replacement.

## Key Features
* **Probabilistic Matching:** Utilizes the Fellegi-Sunter model via the Splink library.
* **Security-First:** Designed for local execution within secure environments (Azure/On-Prem).
* **Privacy-Preserving:** Supports linkage on hashed or pseudonymized identifiers to ensure GDPR compliance.
* **Explainability:** Includes Waterfall Charts to visualize and audit match decisions.

## Architecture
The framework is designed to sit as a "Read-Only Overlay" within a cloud-native architecture.



1. **Ingest:** Secure extraction of data subsets into a 'Raw' container.
2. **Link:** Python-based matching engine processes records.
3. **Serve:** Golden records provided to BI Dashboards (Power BI/Tableau).

## Getting Started
1. Clone the repo: `git clone https://github.com/ShriHari1705/Public-Sector-Record-Linkage`
2. Install dependencies: `pip install -r requirements.txt`
3. Run the demo notebook: `notebooks/02_Record_Linkage_Pilot.ipynb`