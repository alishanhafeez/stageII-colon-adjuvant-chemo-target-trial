METHODS (Pre-Data Protocol)
Study Design
This study is an observational causal inference analysis designed to emulate a hypothetical randomized controlled trial (target trial emulation). The objective is to estimate the intention-to-treat effect of adjuvant chemotherapy versus observation among patients with high-risk stage II colon cancer using SEER–Medicare data.
Data Source
The study uses the Surveillance, Epidemiology, and End Results (SEER)–Medicare linked database, which integrates population-based cancer registry data with longitudinal Medicare claims. SEER provides detailed information on tumor characteristics, staging, and patient demographics, while Medicare claims capture treatment delivery and outcomes. The study includes patients diagnosed between 2006 and 2018 to reflect contemporary adjuvant chemotherapy practices.
Emulated Target Trial Specification
Eligibility Criteria
Eligible individuals are adults aged 18 years or older with histologically confirmed stage II colon adenocarcinoma who underwent curative-intent surgical resection. Patients must have at least one high-risk feature, defined as T4 tumor stage, bowel obstruction or perforation at presentation, or examination of fewer than 12 lymph nodes. Continuous enrollment in Medicare Parts A and B for at least 12 months prior to surgery is required to ensure complete capture of baseline covariates and treatment exposure. Patients with a prior history of malignancy or receipt of neoadjuvant chemotherapy or radiotherapy are excluded. Patients who died within 30 days of surgery are excluded to ensure eligibility for adjuvant treatment decision-making.
Treatment Strategies
Two treatment strategies are compared. The adjuvant chemotherapy strategy is defined as initiation of fluoropyrimidine-based adjuvant chemotherapy within eight weeks of surgical resection. The observation strategy is defined as no initiation of adjuvant chemotherapy within eight weeks of surgical resection. Treatment assignment is observational and emulates randomization through adjustment for baseline confounders.
Time Zero
Time zero is defined as the date of curative surgical resection. This corresponds to the clinical decision point at which adjuvant chemotherapy eligibility is determined and avoids immortal time bias that would arise from defining time zero at chemotherapy initiation or at diagnosis.
Follow-Up
Participants are followed from time zero until colon cancer–specific death, administrative censoring at five years, or loss of Medicare enrollment, whichever occurs first.
Outcomes
The primary outcome is colon cancer–specific mortality, ascertained using SEER cause-of-death data. Overall survival is specified a priori as a sensitivity outcome to assess robustness to potential misclassification of cause of death.
Causal Contrast
The primary estimand is the intention-to-treat effect of initiating adjuvant chemotherapy versus observation on five-year colon cancer–specific mortality.
Confounding Control
Baseline Covariates
Confounding control is performed using baseline covariates measured prior to or at the time of surgery. These include age at diagnosis, sex, race and ethnicity, year of diagnosis, tumor T stage, tumor grade, number of lymph nodes examined, presence of obstruction or perforation, tumor location (right versus left colon), marital status, and county-level socioeconomic deprivation indicators.
Variables Not Adjusted For
Post-baseline variables are not adjusted for, including postoperative complications, chemotherapy completion, duration, or dose intensity, and cancer recurrence. These variables lie on the causal pathway or act as colliders, and conditioning on them would introduce bias.
Statistical Analysis
Propensity Score and Weighting
A propensity score for receipt of adjuvant chemotherapy is estimated using logistic regression incorporating all baseline covariates. Stabilized inverse probability of treatment weights are constructed to estimate the marginal intention-to-treat effect.
Balance Diagnostics
Covariate balance between treatment groups is assessed using standardized mean differences, with values below 0.1 indicating acceptable balance. Weight distributions are examined for instability, and weights are truncated at prespecified percentiles to preserve positivity.
Outcome Modeling
Weighted survival analyses are conducted to estimate the effect of treatment strategy on colon cancer–specific mortality. Cumulative incidence and hazard estimates are derived under the weighted pseudo-population.
Sensitivity Analyses
Prespecified sensitivity analyses include alternative chemotherapy initiation windows (for example, six weeks versus eight weeks), exclusion of borderline high-risk cases, and analysis using overall survival as the outcome.
Causal Assumptions and Directed Acyclic Graph
A directed acyclic graph is constructed to encode assumed causal relationships among treatment, outcome, baseline confounders, mediators, and colliders. Adjustment sets are derived based on the graph to block backdoor paths without conditioning on post-treatment variables.
Failure Modes
Key threats to validity include residual confounding due to unmeasured functional status or frailty, misclassification of chemotherapy timing leading to reintroduction of immortal time bias, and stage migration or misclassification of high-risk features due to inadequate lymph node sampling.
Ethical Considerations
This study uses de-identified, publicly available linked registry and claims data and is exempt from institutional review board approval.


