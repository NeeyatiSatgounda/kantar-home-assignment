\# Kantar Home Assignment



\## Overview



This repository contains my solution for the \*\*Kantar Data Science Fraud Detection Assignment\*\*.



The assignment consists of two independent tasks:



\* \*\*01\_Task\_1\_Anomaly\_Detection.ipynb\*\*

\* \*\*02\_Task\_2\_Fraud\_Classification.ipynb\*\*



The primary objective of this submission is to demonstrate a structured analytical workflow, experimentation, and problem-solving approach rather than focusing solely on achieving the highest predictive performance.



\---



\## Repository Structure



```text

kantar-fraud-detection-assignment/

│

├── README.md

├── requirements.txt

├── dataset\_20260430.xlsx

│

└── notebooks/

&#x20;   ├── 01\_Task\_1\_Anomaly\_Detection.ipynb

&#x20;   └── 02\_Task\_2\_Fraud\_Classification.ipynb

```



\---



\## Environment Setup



Install the required Python dependencies using:



```bash

pip install -r requirements.txt

```



\---



\## Running the Solution



Open and execute the notebooks in the following order:



1\. `01\_Task\_1\_Anomaly\_Detection.ipynb`

2\. `02\_Task\_2\_Fraud\_Classification.ipynb`



\---



\# Notebook Overview



\## Task 1 – Anomaly Detection



This notebook addresses the anomaly detection task by identifying the registration period with an unusually high concentration of fraudulent users.



The notebook is organized into the following sections:



\### Data Understanding



Performed an initial exploration of the dataset, including:



\* Dataset shape

\* Data types

\* Missing value assessment

\* Basic exploratory analysis



This section helped build an overall understanding of the data before proceeding with further analysis.



\### Anomaly Detection



Focused on identifying:



\* The specific anomalous registration date range

\* Fraud concentration over time using graphical analysis



\### Unsupervised Detection Discussion



Discussed potential approaches for automatically detecting similar anomalous periods in scenarios where fraud labels are unavailable, including suitable unsupervised learning techniques and statistical approaches.



\### Miscellaneous – Variable Level Deep Dive



Performed additional exploratory analysis on important variables and categorical features to understand their relationship with fraudulent users.



Several observations from this exploratory analysis were later validated through SHAP-based feature importance analysis in Task 2, providing consistency between exploratory findings and model interpretation.



\---



\## Task 2 – Fraud Classification



This notebook develops a binary classification model to predict fraudulent users.



To improve readability, the notebook presents the final selected solution first, followed by the experimentation process used to arrive at that solution.



The notebook includes:



\* Data preprocessing

\* Feature engineering

\* Model training

\* Hyperparameter optimization

\* Performance evaluation

\* SHAP-based model interpretation



\### Appendix 1 – XGBoost Experimentation



This section documents the different XGBoost modelling strategies explored throughout development.



Each approach includes the reasoning behind its implementation, evaluation, and why it was ultimately retained or discarded before selecting the final model.



\### Appendix 2 – Baseline Models



Implemented Decision Tree and Random Forest models as baseline approaches.



These models established reference performance before transitioning to gradient boosting methods, where XGBoost demonstrated superior predictive performance through sequential learning.



\---



\# Submission Notes



\* All plots, visualizations, model evaluation metrics, and observations are embedded directly within the notebooks.

\* Each notebook contains Markdown explanations describing the methodology, reasoning, and conclusions at every major stage of the analysis.

\* The notebooks are intentionally structured to document both successful and unsuccessful experiments, highlighting the complete analytical thought process behind the final solution.



\---



\# Further Improvements



Given additional time or data, potential enhancements would include:



\* Additional feature engineering using temporal and behavioural patterns.

\* More extensive hyperparameter optimization.

\* Ensemble modelling and model stacking.

\* Probability calibration and threshold optimization based on business objectives.

\* Evaluation using cost-sensitive learning frameworks for highly imbalanced fraud detection problems.

\* Investigation of semi-supervised and self-supervised approaches for fraud detection when labeled data is limited.



\---



\*\*Author:\*\* Neeyati Satgounda



