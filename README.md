**Project Aegis-YT: Adversarial AI Content Guardrail & Pipeline
Executive Summary**
Project Aegis-YT is a modular Trust & Safety system designed to detect adversarial and harmful content on video platforms. Using LLMs for semantic evaluation, it identifies leetspeak, prompt injection, and other evasion techniques that standard filters miss. The system calculates a Composite Video Risk Index (CVRI) to prioritize enforcement actions.
**Features**
Adversarial Detection: Classifies comments by intent (Harassment, Hate Speech, Self-Harm) and flags bypass patterns.
Severity Scoring: Assigns a numeric risk score (0–10) for each comment.
Video-Level Risk Aggregation: CVRI aggregates individual comment risk to focus enforcement on coordinated attacks.
Dynamic Enforcement Actions: Auto-Action, Human Review, or Monitor, based on severity thresholds.
Visual Reporting: Matplotlib plots showing detection uplift and CVRI distribution.
Modular Design: Easy to extend with new policies (YAML-based config structure placeholder included).
**Demo / How to Run**
Clone the repository
git clone https://github.com/vetapalem-pravallika/Adversarial-AI-Content-Guardrail-Pipeline.git
**Notebook**
Open 01_policy_classifier_pipeline.ipynb in Colab.
Update the placeholder variable for your local service account JSON if required:
SERVICE_ACCOUNT_JSON = "YOUR_SERVICE_ACCOUNT_JSON_PATH"
Run the cells to see:
Comment-level classification
CVRI calculation
Enforcement actions
Risk visualizations
CSV Output
The pipeline exports results to adversarial_demo_final.csv for executive review.
**Data**
Sample adversarial comments and results included in CSV.
Dataset is anonymized and safe for demonstration purposes.
**Technical Stack**
Language: Python 3
Libraries: Pandas, Matplotlib, YAML
LLM: Gemini 3 / LLM-as-a-Judge (placeholder for demonstration)
SQL / BigQuery: Drafted queries for Coordinated Spike Detection
**Portfolio / Interview Highlights**
Modular Design: Policies can be updated by non-technical stakeholders.
Adversarial Robustness: Detects leetspeak, prompt injections, and bypass attempts.
Video-Level Risk: Aggregates comment-level risk into CVRI for automated escalation.
Visual Proofs: Charts showing CVRI vs. thresholds and “Bypass Gap” uplift.
**Notes**
Security: No credentials are included in this repository. Keep your service account JSON local.
Extensibility: The project can be extended for new policies, datasets, and visualization dashboards.
