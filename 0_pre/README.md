# Preoperative Data

The preoperative data set contains static medical data at the time before the index operation. Data is available from two different and independent clinics so that results can be validated externally. The dataset contains 13,225 individual cases, each with a total of 79 features and 12 potential targets.

## Data Structure

**Type Legend:** 0=numeric, 1=binary / numeric encoded categorial, 2=on-hot encoded categorial

| id   | name                                   | dimension | lower_limit | upper_limit   | type |
| :--- | :------------------------------------- | :-------- | :---------- | :------------ | :--- |
|    0 | identifier_cohort                      | -         | 0           | 1             | 1    |
|    1 | identifier_organ_system                | -         | 0           | 4             | 1    |
|    2 | gender                                 | -         | 0           | 1             | 1    |
|    3 | age                                    | yrs       | 18          | 120           | 0    |
|    4 | height                                 | cm        | 100         | 250           | 0    |
|    5 | weight                                 | kg        | 25          | 300           | 0    |
|    6 | bmi                                    | kg / m^2  | 5           | 100           | 0    |
|    7 | asa                                    | -         | 0           | 5             | 1    |
|    8 | ecog                                   | -         | 0           | 5             | 1    |
|    9 | cci                                    | -         | 0           | 24            | 1    |
|   10 | myocardial_infarction                  | -         | 0           | 1             | 1    |
|   11 | congestive_heart_failure               | -         | 0           | 1             | 1    |
|   12 | peripheral_vascular_disease            | -         | 0           | 1             | 1    |
|   13 | cerebrovascular_disease                | -         | 0           | 1             | 1    |
|   14 | dementia                               | -         | 0           | 1             | 1    |
|   15 | chronic_pulmonary_disease              | -         | 0           | 1             | 1    |
|   16 | rheumatic_disease                      | -         | 0           | 1             | 1    |
|   17 | peptic_ulcer_disease                   | -         | 0           | 1             | 1    |
|   18 | liver_disease_mild                     | -         | 0           | 1             | 1    |
|   19 | liver_disease_moderate_to_severe       | -         | 0           | 1             | 1    |
|   20 | diabetes_without_chronic_complications | -         | 0           | 1             | 1    |
|   21 | diabetes_with_chronic_complications    | -         | 0           | 1             | 1    |
|   22 | hemiplegia_or_paraplegia               | -         | 0           | 1             | 1    |
|   23 | renal_disease                          | -         | 0           | 1             | 1    |
|   24 | malignancy                             | -         | 0           | 1             | 1    |
|   25 | metastatic_solid_tumor                 | -         | 0           | 1             | 1    |
|   26 | aids                                   | -         | 0           | 1             | 1    |
|   27 | cardiac_arythmia                       | -         | 0           | 1             | 1    |
|   28 | valvular_disease                       | -         | 0           | 1             | 1    |
|   29 | pulmonary_circulatory_disorder         | -         | 0           | 1             | 1    |
|   30 | arterial_hypertension                  | -         | 0           | 1             | 1    |
|   31 | other_neurological_disorders           | -         | 0           | 1             | 1    |
|   32 | hypothyroidism                         | -         | 0           | 1             | 1    |
|   33 | coagulopathy                           | -         | 0           | 1             | 1    |
|   34 | obesity                                | -         | 0           | 1             | 1    |
|   35 | weight_loss                            | -         | 0           | 1             | 1    |
|   36 | fluid_and_electrolyte_disorders        | -         | 0           | 1             | 1    |
|   37 | blood_loss_anemia                      | -         | 0           | 1             | 1    |
|   38 | deficiency_anemia                      | -         | 0           | 1             | 1    |
|   39 | alcohol_abuse                          | -         | 0           | 1             | 1    |
|   40 | drug_abuse                             | -         | 0           | 1             | 1    |
|   41 | psychoses                              | -         | 0           | 1             | 1    |
|   42 | depression                             | -         | 0           | 1             | 1    |
|   43 | coronary_heart_disease                 | -         | 0           | 1             | 1    |
|   44 | chronic_pancreatitis                   | -         | 0           | 1             | 1    |
|   45 | ulcerative_colitis                     | -         | 0           | 1             | 1    |
|   46 | crohns_disease                         | -         | 0           | 1             | 1    |
|   47 | primary_system                         | -         | -           | -             | 2    |
|   48 | system_esophagus                       | -         | 0           | 1             | 1    |
|   49 | system_stomach                         | -         | 0           | 1             | 1    |
|   50 | system_intestine                       | -         | 0           | 1             | 1    |
|   51 | system_liver                           | -         | 0           | 1             | 1    |
|   52 | system_pancreas                        | -         | 0           | 1             | 1    |
|   53 | system_count                           | -         | 1           | 5             | 0    |
|   54 | urgency                                | -         | 0           | 5             | 1    |
|   55 | resurgery                              | -         | 0           | 1             | 1    |
|   56 | month                                  | -         | 0           | 11            | 1    |
|   57 | weekday                                | -         | 0           | 6             | 1    |
|   58 | daytime                                | -         | 0           | 2             | 1    |
|   59 | hour                                   | -         | 0           | 23            | 1    |
|   60 | mean_monthly_temperature               | °C        | -50         | 50            | 0    |
|   61 | minimum_monthly_temperature            | °C        | -50         | 50            | 0    |
|   62 | maximum_monthly_temperature            | °C        | -50         | 50            | 0    |
|   63 | monthly_precipitation                  | l / m^2   | 0           | 500           | 0    |
|   64 | monthly_sunshine_hours                 | h         | 0           | 744           | 0    |
|   65 | sodium                                 | mmol / l  | 50          | 200           | 0    |
|   66 | potassium                              | mmol / l  | 1           | 10            | 0    |
|   67 | bilirubin                              | mg / dl   | 0           | 50            | 0    |
|   68 | urea                                   | mg / dl   | 0           | 400           | 0    |
|   69 | ggt                                    | U / l     | 0           | 100,000       | 0    |
|   70 | lipase                                 | U / l     | 0           | 50,000        | 0    |
|   71 | crp                                    | mg / l    | 0           | 1,000         | 0    |
|   72 | hemoglobin                             | g / dl    | 0           | 40            | 0    |
|   73 | wbc                                    | / nl      | 0           | 100           | 0    |
|   74 | platelets                              | / nl      | 0           | 16,000,000    | 0    |
|   75 | hematocrit                             | l / l     | 0           | 1             | 0    |
|   76 | inr                                    | -         | 0           | 10            | 0    |
|   77 | aptt                                   | s         | 0           | 500           | 0    |
|   78 | erythrocytes                           | / pl      | 0           | 10            | 0    |
|   79 | creatinine                             | mg / dl   | 0           | 100           | 0    |
|   80 | glucose                                | mg / dl   | 0           | 1,000         | 0    |
|   81 | target_30_day_mortality                | -         | 0           | 1             | 1    |
|   82 | target_90_day_mortality                | -         | 0           | 1             | 1    |
|   83 | target_deceased_after_discharge        | -         | 0           | 1             | 1    |
|   84 | target_clavien_dindo_v                 | -         | 0           | 1             | 1    |
|   85 | target_acute_myocardial_infarction     | -         | 0           | 1             | 1    |
|   86 | target_pulmonary_embolism              | -         | 0           | 1             | 1    |
|   87 | target_septic_shock                    | -         | 0           | 1             | 1    |
|   98 | target_pneumonia                       | -         | 0           | 1             | 1    |
|   89 | target_liver_failure                   | -         | 0           | 1             | 1    |
|   90 | target_cardiogenic_shock               | -         | 0           | 1             | 1    |
|   91 | target_acute_pancreatitis              | -         | 0           | 1             | 1    |
|   92 | target_acute_respiratory_failure       | -         | 0           | 1             | 1    |


## Filtered Data Sets

The following exclusion criteria were applied to the following data sets:

### Elective

Exclusion Criteria:
- **meta_urgency:** <= 3
- **target_30_day_mortality:** not available
- **target_90_day_mortality:** not available
- **Completeness:** < 75 %

Output: 7,711 cases

### Emergency

Exclusion Criteria:
- **meta_urgency:** >= 4
- **target_30_day_mortality:** not available
- **target_90_day_mortality:** not available
- **Completeness:** < 50 %

Output: 1,273 cases

## Additional Notes

### Identifier Cohort

- **0:** Training Cohort _(Clinic 1: CVK & CCM)_
- **1:** Validation Cohort _(Clinic 2: CBF)_

### Daytime
- **0:** Night _(10pm <= t < 6am)_
- **1:** Morning _(6am <= t < 2pm)_
- **2:** Afternoon _(2pm <= t < 10pm)_