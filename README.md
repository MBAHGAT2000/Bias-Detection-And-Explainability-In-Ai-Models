Bias Detection and Explainability in AI Job Screening Models
📋 Project Overview
This project implements a comprehensive bias detection and explainability framework for AI-powered job screening systems. The analysis focuses on identifying, measuring, and mitigating gender bias in hiring decisions using structured candidate data and logistic regression models.
🎯 Challenge Objectives
•	Bias Detection: Identify and quantify gender bias in AI hiring models
•	Fairness Measurement: Calculate key fairness metrics (Demographic Parity, Equal Opportunity, Average Odds Difference)
•	Explainability: Use SHAP analysis to understand model decision-making patterns
•	Bias Mitigation: Implement reweighing techniques to reduce discriminatory outcomes
•	Trade-off Analysis: Evaluate the balance between model accuracy and fairness
📊 Dataset Description
•	Size: 1,500 job candidate records
•	Features: 10 structured attributes including Age, Gender, Education, Experience, Interview/Skill/Personality Scores
•	Target: Binary hiring decision (Hire vs. Not Hire)
•	Bias Simulation: Intentionally imbalanced training data (67% male, 33% female)

🔧 Technical Implementation
Models Implemented
1.	Baseline Logistic Regression: Standard implementation
2.	Standardized Model: Feature-scaled logistic regression
3.	Class-Balanced Model: Built-in class weight balancing
4.	Reweighing Model: Sample-weighted training approach
Fairness Metrics
•	Demographic Parity: Equal positive prediction rates across groups
•	Equal Opportunity: Equal true positive rates for qualified candidates
•	Average Odds Difference: Combined TPR and FPR differences
Explainability Tools
•	SHAP Analysis: Feature importance and individual prediction explanations
•	Feature Attribution: Understanding which factors drive hiring decisions
📈 Key Results
Model Performance
Model	Accuracy	Precision	Recall
Baseline	86.3%	81.1%	71.2%
Standardized	86.7%	82.0%	71.8%
Reweighing	84.4%	72.0%	81.5%
Bias Detection
•	Gender Gap Identified: 3.2% difference in hiring predictions
•	Successful Mitigation: Complete elimination of demographic parity gap
•	Trade-off: 2.3% accuracy decrease for fair outcomes
Feature Importance
1.	SkillScore (34.2%) - Primary driver
2.	PersonalityScore (28.9%) - Strong influence
3.	InterviewScore (19.8%) - Moderate impact
4.	Gender (4.5%) - Minimal direct influence
🚀 Getting Started
Prerequisites
bash
pip install pandas numpy scikit-learn matplotlib seaborn shap
Running the Analysis
1.	Clone the repository
2.	Place your dataset as data.csv in the project directory
3.	Run the Jupyter notebook cells sequentially
4.	Review generated fairness metrics and visualizations
File Structure
text
├── bias_detection_analysis.ipynb    # Main analysis notebook
├── data.csv                         # Dataset file
├── README.md                        # This file
└── requirements.txt                 # Python dependencies







