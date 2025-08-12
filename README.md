# Rule606_BrokerRouting_Risk

**Project Overview**
This repository contains the analysis, code, and visualizations for the research paper:
Measuring BrokerDealer Routing Risk and Transparency Using SEC Rule 606 Disclosures

The project examines publicly available SEC Rule 606 broker-dealer routing data to evaluate venue concentration, routing consistency, and payment for order flow (PFOF) incentives — providing insight into how these factors may impact execution quality and market transparency.

**Key Features**
- Data Ingestion & Parsing – Extracts and processes quarterly Rule 606 XML disclosures from multiple brokers.

- Metrics Calculation –

  - Herfindahl–Hirschman Index (HHI) for venue concentration.

  - Routing Volatility via quarterly HHI standard deviation.

  - Cents Per Hundred Shares (CPH) for incentive measurement.

- Composite Risk Scoring – Combines concentration, incentive, and volatility metrics.

- Visualization – Tableau dashboard for broker comparisons and drill-down by security type.

- Reproducible Jupyter Notebook – End-to-end analysis in Python.


**Repository Structure**
├── Code_BrokerDealer_Routing_Risk_Analysis.ipynb     # Python data processing & analysis
├── Tableau_BrokerDealer_Routing_Risk_Dashboard.twbx  # Interactive Tableau dashboard
├── Dashboard_BrokerDealer_Routing_Risk.png           # Static dashboard preview
├── Measuring_BrokerDealer_Routing_Risk_SEC_Rule606.pdf  # Full research paper (APA format)
└── README.md                                         # Project documentation

**Methodology**
1. Data Acquisition – Downloaded Rule 606 XML files from broker-dealer public disclosures.
2. Data Processing – Parsed XML into structured tables and normalized by security type.
3. Metric Computation –
  - Venue Concentration (HHI): Measures market share concentration.
  - Routing Volatility: Standard deviation of HHI over time.
  - Incentive Measurement (CPH): Calculates payment per hundred shares.
4. Risk Scoring – Weighted composite score integrating all three metrics.
5. Visualization – Built Tableau dashboard for comparative analysis.

**Technologies**
- Python – pandas, numpy, matplotlib
- Tableau – interactive data visualization
- SEC Rule 606 XML disclosures – public broker-dealer routing data

