Data Extraction and Cohort Construction Checklist

This checklist defines required verification steps during cohort construction. No analysis will proceed until all items are explicitly confirmed.

- Data Access Verification

Confirm SEER–Medicare data version and release year

Confirm linkage completeness for tumor registry and claims files

Confirm availability of cause-specific mortality data

- Cohort Entry

Verify incident stage II colon adenocarcinoma cases only

Confirm exclusion of rectal cancers

Confirm diagnosis years restricted to 2006–2018

Verify continuous Medicare Parts A and B enrollment in the 12 months prior to surgery

Confirm exclusion of Medicare Advantage enrollees

- Time Zero Validation

Confirm surgical resection date is available and complete

Verify no deaths occur before time zero

Exclude deaths within 30 days post-surgery

Confirm chemotherapy exposure is assessed strictly after time zero

- Exposure Definition

Verify chemotherapy initiation codes correspond to fluoropyrimidine-based regimens

Confirm chemotherapy initiation window is ≤8 weeks post-surgery

Verify no misclassification of neoadjuvant therapy as adjuvant

Confirm observation group has no chemotherapy claims within the assignment window

- High-Risk Feature Validation

Verify T stage coding and mapping to T4

Confirm obstruction and perforation coding

Verify lymph node count variable and threshold (<12 nodes)

Confirm at least one high-risk feature per patient

- Outcome Ascertainment

Verify colon cancer–specific mortality coding in SEER

Confirm death dates are complete and consistent

Cross-check overall mortality as a backup endpoint

- Covariate Timing

Confirm all baseline covariates are measured prior to or at surgery

Verify no post-baseline variables enter propensity models

Explicitly flag and exclude postoperative complications from adjustment

- Weight Construction Diagnostics

Verify propensity score overlap between treatment groups

Inspect stabilized weight distributions

Document truncation thresholds prior to outcome modeling

- Internal Consistency Checks

Compare unweighted baseline characteristics across groups

Verify expected associations (e.g., older age → lower chemotherapy use)

Confirm no implausible effect estimates in early follow-up

- Sign-Off

Cohort construction completed without unresolved flags

Deviations documented and justified
