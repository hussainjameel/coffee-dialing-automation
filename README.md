# ☕ Coffee Dialling Automation
 
> AI/ML-based coffee quality intelligence for specialty coffee analysis, quality prediction and flavour profiling.
> Developed for **URKU Chocolate, Melbourne** as part of **ITW601 Work Integrated Learning**.
 
---
 
## Table of Contents
 
- [Overview](#overview)
- [Machine Learning Approach](#machine-learning-approach)
- [Dataset](#dataset)
- [Model Development](#model-development)
- [Key Outcomes](#key-outcomes)
- [Tech Stack](#tech-stack)
- [Repository Structure](#repository-structure)
- [Project Status](#project-status)
- [Future Scope](#future-scope)
- [Authors](#authors)
- [Acknowledgement](#acknowledgement)
---
 
## Overview
 
Coffee Dialling Automation applies machine learning to the **Arabica Coffee Quality dataset** from the Coffee Quality Institute. The dataset contains sensory, physical and processing-related attributes of specialty coffee batches.
 
The main objective was to explore how historical coffee quality data can be transformed into a data-driven decision support system for coffee evaluation, profiling, and future automation — using three core ML approaches:
 
| Approach | Purpose |
|---|---|
| **Classification** | Explore quality category prediction |
| **Regression** | Predict the overall coffee quality score |
| **Clustering** | Discover natural coffee profiles and sensory patterns |
 
---
 
## Machine Learning Approach
 
The project follows a complete ML workflow:
 
- Exploratory Data Analysis
- Data preprocessing & feature engineering
- Outlier handling & missing value treatment
- Categorical encoding
- Supervised learning (classification & regression)
- Unsupervised learning (clustering)
- Cross-validation & model evaluation
- Cluster profiling & visual analytics
---
 
## Dataset
 
The project uses the Arabica coffee quality dataset with the following features:
 
**Sensory features:** Aroma, Flavor, Aftertaste, Acidity, Body, Balance
 
**Physical & processing features:** Moisture Percentage, Altitude, Defects, Country of Origin, Processing Method
 
**Target:** Overall Quality Score
 
---
 
## Model Development
 
### Classification
 
A supervised classification approach was explored to predict coffee quality categories using selected non-sensory and supporting features — testing whether batches could be grouped into low, medium, and high quality levels. This also highlighted the inherent challenges of classifying a dataset where most samples already belong to the specialty-grade range.
 
### Regression
 
A supervised regression approach was used to predict the **Overall** coffee quality score. The final cleaned regression workflow used key sensory features (aroma, flavor, aftertaste, acidity, body, balance) alongside selected supporting features to estimate quality scores.
 
This model demonstrates how future coffee batches could be scored automatically when new sensory or live-streamed feature data becomes available.
 
### Clustering
 
An unsupervised clustering approach was used to identify hidden coffee profiles based on sensory and quality-related patterns. The model groups coffee samples into distinct clusters based on similarities in flavour, balance, acidity, body, and other quality indicators.
 
Business applications include:
 
- Coffee batch profiling
- Flavour group identification
- Product segmentation
- Sourcing decisions
- Future recommendation systems
- Assigning new live coffee samples to existing quality clusters
---
 
## Key Outcomes
 
The project successfully developed an end-to-end ML pipeline that can:
 
- Clean and prepare raw coffee quality data
- Extract meaningful EDA insights
- Identify important sensory and quality-related features
- Predict overall coffee quality scores via regression
- Explore quality category prediction via classification
- Create sensory-based coffee clusters via unsupervised learning
- Export model-ready datasets, cluster summaries and visual outputs
---
 
## Tech Stack
 
| Tool | Purpose |
|---|---|
| Python | Core programming language |
| pandas | Data manipulation and analysis |
| NumPy | Numerical computing |
| scikit-learn | Machine learning models and pipelines |
| matplotlib | Data visualisation |
| seaborn | Statistical data visualisation |
| Jupyter Notebook / Google Colab | Interactive development environment |
| GitHub | Version control and collaboration |
 
---
 
## Repository Structure
 
```text
coffee-dialling-automation/
│
├── data/
│   ├── raw/
│      └── Arabica Dataset
│
├── models/
|   ├── classication
│   ├── regression
│   └── clustering
│
├── results/
│   └── classification_results
│   └── regression_results
|   └── clustering_results
|
|
├── reports/
│   └── project_reports/
│
├── README.md
└── requirements.txt
```
 
---
 
## Project Status
 
**Completed:**
- [x] Data preprocessing pipeline
- [x] Exploratory data analysis
- [x] Classification experimentation
- [x] Regression modelling
- [x] Cross-validation and evaluation
- [x] Clustering model development
- [x] Cluster interpretation
- [x] Exportable datasets and visualisations
**Planned:**
- [ ] Live data stream integration
- [ ] Real-time prediction workflow
- [ ] Automated cluster assignment for new samples
- [ ] Dashboard or API deployment
---
 
## Future Scope
 
The current system is built on historical coffee quality data. The next stage is to extend it toward live data integration:
 
- Connecting real-time coffee sensor data
- Using live roasting or storage conditions as model inputs
- Predicting overall quality scores for new coffee batches
- Assigning incoming samples to existing sensory clusters
- Building a dashboard for coffee quality monitoring
- Developing an API for automated coffee scoring and profiling
- Improving model performance with larger and more diverse datasets
With live data integration, the project can evolve from a notebook-based ML analysis into a real-time coffee intelligence system.
 
---
 
## Authors
 
- **Hussain Jameel**
---
 
## Acknowledgement
 
This project was completed for **URKU Chocolate, Melbourne** as part of the **ITW601 Work Integrated Learning** project at Torrens University Australia.
