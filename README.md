# Revathy_Projects
Data Analysis done using Python 

Project Documentation 
Project Title: Incident Management Analysis using Pandas, Matplotlib, and Seaborn 
1. Project Overview
 This project utilizes event logs from an incident management process extracted from the audit system of a ServiceNow™ platform instance used by an IT company. This project focuses on analysing incident data using Pandas for data cleaning and 
analysis, and Matplotlib and Seaborn for data visualization. The goal is to identify 
resourse utilization, work distribution, operational efficiency  to support better business 
decisions. 
2. Tools Used 
• Pandas – Data cleaning and manipulation 
• Matplotlib – Basic data visualization 
• Seaborn – Advanced and statistical visualizations 
3. Dataset 
• Source: Incident management process enriched event log - UCI Machine Learning Repository
• Description: The dataset contains event log of an incident management process with following key columns:
number: incident identifier (24,918 different values);
incident state: eight levels controlling the incident management process transitions from opening until closing the case;
active: boolean attribute that shows whether the record is active or closed/canceled;
reassignment_count: number of times the incident has the group or the support analysts changed;
reopen_count: number of times the incident resolution was rejected by the caller;
sys_mod_count: number of incident updates until that moment;
made_sla: boolean attribute that shows whether the incident exceeded the target SLA;
caller_id: identifier of the user affected;
opened_by: identifier of the user who reported the incident;
opened_at: incident user opening date and time;
sys_created_by: identifier of the user who registered the incident;
sys_created_at: incident system creation date and time;
sys_updated_by: identifier of the user who updated the incident and generated the current log record;
sys_updated_at: incident system update date and time;
contact_type: categorical attribute that shows by what means the incident was reported;
location: identifier of the location of the place affected;
category: first-level description of the affected service;
subcategory: second-level description of the affected service (related to the first level description, i.e., to category);
u_symptom: description of the user perception about service availability;
cmdb_ci: (confirmation item) identifier used to report the affected item (not mandatory);
impact: description of the impact caused by the incident (values: 1â€“High; 2â€“Medium; 3â€“Low);
urgency: description of the urgency informed by the user for the incident resolution (values: 1â€“High; 2â€“Medium; 3â€“Low);
priority: calculated by the system based on 'impact' and 'urgency';
assignment_group: identifier of the support group in charge of the incident;
assigned_to: identifier of the user in charge of the incident;
knowledge: boolean attribute that shows whether a knowledge base document was used to resolve the incident;
u_priority_confirmation: boolean attribute that shows whether the priority field has been double-checked;
notify: categorical attribute that shows whether notifications were generated for the incident;
problem_id: identifier of the problem associated with the incident;
rfc: (request for change) identifier of the change request associated with the incident;
vendor: identifier of the vendor in charge of the incident;
caused_by: identifier of the RFC responsible by the incident;
close_code: identifier of the resolution of the incident;
resolved_by: identifier of the user who resolved the incident;
resolved_at: incident user resolution date and time (dependent variable);
closed_at: incident user close date and time (dependent variable).
4. Steps Followed 
1. Imported the dataset using Pandas. 
2. Cleaned the data by: 
o Removing missing and duplicate values 
o Converting date  columns to proper formats 
3. Performed exploratory data analysis (EDA) using Pandas. 
4. Created visualizations using Matplotlib and Seaborn, such as: 
   Box plot 
   Bar charts 
   Pie charts
   Histogram
6. Interpreted the results to extract meaningful insights. 
5. Key Insights 
    - Operational Stability – The incident priority distribution shows a strong dominance of moderate issues, confirming that the system operates in a stable environment with minimal emergencies.
- Resilient Management – The rarity of critical incidents highlights effective system reliability and preparedness, while balanced handling of high and low severity cases ensures comprehensive coverage.
- User Behavior Insights – The overwhelming reliance on phone communication indicates a preference for real-time support, while low adoption of self-service and email suggests opportunities for digital engagement improvements.
- Data Attribution Gaps – A significant portion of incidents remain unattributed (“Not found”), pointing to weaknesses in tracking and accountability that need immediate attention for better performance measurement.
- Strategic Recommendations – Focus resources on managing moderate incidents efficiently, promote self-service adoption, encourage email for non-urgent cases, and strengthen data capture processes to ensure fair workload distribution among associates.


6. Files Included 
• incident_event_log.csv – Raw dataset 
• IncidentManagement.ipynb– Pandas analysis and visualizations 
• README.md – Project description and usage instructions 
7. How to Use 
1. Open IncidentManagement.ipynb using Jupyter Notebook or JupyterLab. 
2. Run the notebook cells step by step to view data cleaning, analysis, and 
visualizations. 
3. Modify the code to explore additional insights if needed. 
8. Conclusion 
This project demonstrates how Python libraries such as Pandas, Matplotlib, and 
Seaborn can be effectively used for real-world data analysis. The insights gained 
from this analysis can help businesses understand incident management process and make data
driven decisions.
