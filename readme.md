STAGE 1: https://drive.google.com/file/d/1Kr36CcdyiMF6uiKuToFM3S_2dPxiHogg/view?usp=sharing
STAGE 2: https://drive.google.com/file/d/1E1-56JMUYHBNPfMiG6mcBnB9Af_RAYl-/view?usp=sharing

Agricultural Subsidy Leakage Detector

Project Description

The Agricultural Subsidy Leakage Detector is a web-based dashboard designed to enhance transparency and accountability in agricultural subsidy distribution.



The primary goal is to detect anomalous subsidy distribution patterns across multiple dimensions, including dealers, beneficiaries, seasons, and geographies.



Key Features

This application provides a comprehensive interface for investigating potential subsidy fraud:



Key Performance Indicators (KPIs): Real-time monitoring of total Transactions, Unique Beneficiaries, active Dealers, and Flagged Anomalies.



Data Visualization: Charts showing Dealer Volume and distribution of Anomaly Types for high-level insight.



Geospatial Analysis: An interactive map powered by Leaflet.js to visualize transaction density and pinpoint Geo-Temporal Cluster Anomalies.



Dynamic Filtering: Ability to filter data and anomalies by:



Scheme (Fertilizer, Seeds, Equipment)



Season (Kharif, Rabi)



District



Anomaly Severity (High, Medium, Low)



Anomaly Investigation Table: A detailed, sortable table displaying all flagged anomalies with their Severity, Score, Type, and an ML-generated Explanation showing feature importance (Quantityhttps://www.google.com/search?q=/Land, Geo-Isolation, Dealer Z-score).



Drilldown Capability: Search and view specific transaction history and statistical information for individual Dealers and Beneficiaries.



Data Importhttps://www.google.com/search?q=/Export: Functionality to upload new data via a CSV file or load a sample dataset, and to download the full anomaly report as a CSV.



Anomaly Detection Methodology

The system employs a hybrid detection approach combining traditional rule-based heuristics with an advanced unsupervised machine learning model to detect both known and novel leakage patterns.



1\. AIhttps://www.google.com/search?q=/ML Model (Simulated Isolation Forest)

The core mechanism is a multi-feature ML Outlier model, simulating an Isolation Forest, which simultaneously scores deviations across multiple features. It flags transactions that are statistically isolated in the dataset.



Feature Importance: The model uses deviations in Quantityhttps://www.google.com/search?q=/Land Ratio, Geo-Location Isolation, and Dealer Volume Z-score to determine the final anomaly score.



2\. Rule-Based Heuristics

Rules are applied to catch clear, pre-defined types of potential fraud:



Quantity vs. Land: Transactions where the subsidy quantity exceeds the established rule-of-thumb caps per acre for the specific scheme.



Dealer Outliers: Dealers whose transaction volumes are statistically far above the regional average (high Z-score).



Geo Clusters: Identification of dense, temporally tight claims in specific geographical locations, suggesting potential coordination.



Getting Started

Since this project is implemented as a single, self-contained HTML file, running it is straightforward.



Prerequisites

You only need a modern web browser (Chrome, Firefox, Edge, Safari).



Running the Application

Download: Save the stage1.html file to your local machine.



Run: Double-click the stage1.html file, or open it directly in your web browser.



Application Workflow

The typical user workflow is as follows:



Upload: Load a new CSV data file or use the built-in sample data.



Filter: Use the filter panel to narrow down the scope of investigation by scheme, season, district, or anomaly severity.



Investigate: Use the drilldown panels to analyze specific dealers or beneficiaries, and review the Anomaly Table for detailed ML explanations.



Export: Download the filtered list of anomalies as a CSV for external audit or further processing.


