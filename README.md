## Executive Summary  
This project harnessed workforce event data from Primoris Renewable Energy to develop an end-to-end people-analytics solution. A unified dataset of hires, rehires, promotions, demotions, transfers, and terminations was assembled and cleaned. Predictive churn models (Random Forest for involuntary churn and XGBoost for voluntary churn) were trained, and a dynamic Tableau dashboard was delivered to enable real-time HR decision-making.

## Business Understanding  
Primoris Renewable Energy operates in a high-growth, project-driven environment with critical talent pipelines. Rising employee turnover was identified as a risk to operational continuity and cost efficiency. Project objectives included uncovering drivers of attrition, quantifying churn risk, and recommending targeted retention strategies to foster long-term organizational stability.

## Data Cleaning & Preprocessing  
All event tables were merged into a master employee history, standardized to a single unique identifier (ee_number), and stripped of irrelevant fields. Inconsistencies in date formats and categorical labels were resolved, missing values were imputed or flagged, and redundant columns were dropped. Feature engineering produced time-since-last-event metrics and binary flags for recent promotions or transfers.

## Exploratory Data Analysis  
Attrition patterns were profiled by voluntary vs. involuntary exit, with peak termination rates observed among mid-career cohorts. Promotion and demotion trends highlighted potential engagement gaps at senior levels. Transfer volumes suggested uneven internal mobility across departments, and rehire behavior revealed opportunities for alumni-based rehiring campaigns.

## Predictive Modeling  
A Random Forest classifier—targeting involuntary churn—achieved 85.5 % accuracy with 18.5 % recall on the test set, offering interpretable feature-importance rankings for HR leaders. An XGBoost classifier—focused on voluntary departures—demonstrated superior precision in flagging at-risk employees without overwhelming stakeholder capacity. Key predictors included days since last promotion, recent project assignment changes, and tenure.

## Dashboard & Visualization  
An interactive Tableau workbook presents three core KPI views—Workforce Trends, Employee Experience, and Talent Retention. End users can filter by department, region, and time period, compare predicted risk vs. historical churn, and drill into individual risk profiles. Visual alerts surface emerging turnover hotspots and drive data-backed intervention.

## Agile Methodology & Project Management  
The eight-week engagement followed two-week sprint cycles, with a prioritized backlog maintained in Excel and Jira. Progress was tracked via burndown charts, and bi-weekly demos solicited stakeholder feedback. Sprint retrospectives captured lessons learned, ensuring continuous refinement of data pipelines, modeling workflows, and dashboard features.

## Results & Conclusions  
The combined approach delivered a robust workforce analytics toolkit:  
- A clean, merged employee dataset supporting future analyses  
- Predictive models that identify both involuntary and voluntary churn with operationally acceptable trade-offs  
- A self-service dashboard enabling HR to monitor workforce health and test “what-if” retention scenarios  
These assets empower Primoris leadership to allocate retention resources more effectively and anticipate staffing needs with confidence.

## Future Work  
Recommended enhancements include integration with the HRIS for automated data refreshes, deployment of trigger-based alerts for high-risk employees, incorporation of employee-engagement survey metrics, quarterly model retraining, and scenario-simulation capabilities for strategic workforce planning.
