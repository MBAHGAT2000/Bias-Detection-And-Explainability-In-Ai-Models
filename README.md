Bias Detection and Explainability in AI Job Screening Models
📋 Project Overview
This project implements a comprehensive bias detection and explainability framework for AI-powered job screening systems. The analysis focuses on identifying, measuring, and mitigating gender bias in hiring decisions using structured candidate data and logistic regression models.

🎯 Challenge Objectives
Bias Detection: Identify and quantify gender bias in AI hiring models

Fairness Measurement: Calculate key fairness metrics (Demographic Parity, Equal Opportunity, Average Odds Difference)

Explainability: Use SHAP analysis to understand model decision-making patterns

Bias Mitigation: Implement reweighing techniques to reduce discriminatory outcomes

Trade-off Analysis: Evaluate the balance between model accuracy and fairness


📊 Dataset Description
Size: 1,500 job candidate records

Features: 10 structured attributes including Age, Gender, Education, Experience, Interview/Skill/Personality Scores

Target: Binary hiring decision (Hire vs. Not Hire)

Bias Simulation: Intentionally imbalanced training data (67% male, 33% female)


🔧 Technical Implementation
Models Implemented
Baseline Logistic Regression: Standard implementation

Standardized Model: Feature-scaled logistic regression

Class-Balanced Model: Built-in class weight balancing

Reweighing Model: Sample-weighted training approach

Fairness Metrics
Demographic Parity: Equal positive prediction rates across groups

Equal Opportunity: Equal true positive rates for qualified candidates

Average Odds Difference: Combined TPR and FPR differences

Explainability Tools
SHAP Analysis: Feature importance and individual prediction explanations

Feature Attribution: Understanding which factors drive hiring decisions


📈 Key Results
Model Performance
Model	Accuracy	Precision	Recall
Baseline	86.3%	81.1%	71.2%
Standardized	86.7%	82.0%	71.8%
Reweighing	84.4%	72.0%	81.5%
Bias Detection
Gender Gap Identified: 3.2% difference in hiring predictions

Successful Mitigation: Complete elimination of demographic parity gap


