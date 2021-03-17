# FusionPredictiveModel
## Pre-processing <br />
### Demographics: <br />
  one row per patient, features as columns<br />
### CPT:<br />
  select popular CPTs as features<br />
  2 rows per patient: row 1 contains feature values (CPT counts) from current interval, row 2 contains feature values (CPT counts) from history interval<br />
### ICD:<br />
  ICD groups based on hierarchical structure of coding as features<br />
  2 rows per patient: row 1 contains feature values (counts of ICD from the group) from current interval, row 2 contains feature values (counts of ICD from the group) from       history interval<br />
### Medicines:<br />
  Frequent medicines are grouped based on their function; each group is a feature<br />
  2 rows per patient: row 1 contains feature values (counts of Iedicines from the group) from current interval, row 2 contains feature values (counts of medicines from the group) from history interval<br />
### Labs:<br />
  Selct relevant labs as features  
  2 rows per patient: row 1 contains feature values (lab value coded as Normal/Abnormal/Unknown) from current interval, row 2 contains feature values (lab value coded as Normal/Abnormal/Unknown) from history interval
  
## Normalization  
Part of code file; all values between 0 and 1

## Fusion  
Ealry, Late, and Middle Fusion
