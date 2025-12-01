NeuraPath-CS: AI Interview Validation

Project Summary
This repository supports the NeuraPath case study, which uses the TBP methodology to validate that our AI platform delivers a statistically significant advantage against the 6% interview failure rate.
It addresses the core problem of scaling personalized coaching using Computer Vision (CV).

Repository Structure

NeuraPath-CS/
├── script.ipynb          # Main execution: EDA, T-Test, Analysis
├── requirements.txt      # Python dependencies
└── sorted_data/          # Raw images for CV model training

Execution and Setup

1. Environment Configuration
Install required libraries for data and statistical analysis:
pip install -r requirements.txt

2. Running the Analysis
Run script.ipynb sequentially for the full analysis:
jupyter notebook script.ipynb

Analysis and Validation

The script.ipynb implements the core deliverables:

Orchestration & EDA
- Defines the Binary Independent Variable (IV) and Weighted Dependent Variable (DV) calculation
- Shows results of the A/B testing experiment using:
  - Distribution Plot
  - Box Plot
  - Factor Breakdown Plot

Hypothesis Evaluation (T-Test)

Metric       | Result                | Rationale
------------ | ------------------- | -------------------------
P-Value      | 1.06167 × 10^-20    | Far below α = 0.05
Conclusion   | Null Hypothesis (H0) REJECTED | Confirms a statistically significant performance increase

Resulting AIML Tool

NeuraPath is the scalable platform that converts complex behavioral data (from sorted_data images) into a singular Weighted Performance Score (1–10) required for this analysis.
It provides objective, measurable feedback and enables scalable coaching for interview readiness.
