# Preoperative Data

The preoperative data set contains static medical data at the time before the index operation. Data is available from two different and independent clinics so that results can be validated externally. The dataset contains 13,225 individual cases, each with a total of 78 features and 11 potential targets.

## Data Structure

**Type Legend:** 0=numeric, 1=binary / numeric encoded categorial, 2=on-hot encoded categorial

| id   | name                                   | dimension | lower_limit | upper_limit   | type |
| :--- | :------------------------------------- | :-------- | :---------- | :------------ | :--- |
|    0 | identifier_cohort                      | -         | 0           | 1             | 1    |
|    1 | gender                                 | -         | 0           | 1             | 1    |
|    2 | age                                    | yrs       | 18          | 120           | 0    |
|    3 | height                                 | cm        | 100         | 250           | 0    |
|    4 | weight                                 | kg        | 25          | 300           | 0    |
|    5 | bmi                                    | kg / m^2  | 5           | 100           | 0    |
|    6 | asa                                    | -         | 0           | 5             | 1    |
|    7 | ecog                                   | -         | 0           | 5             | 1    |
|    8 | cci                                    | -         | 0           | 24            | 1    |
|    9 | myocardial_infarction                  | -         | 0           | 1             | 1    |
|   10 | congestive_heart_failure               | -         | 0           | 1             | 1    |
|   11 | peripheral_vascular_disease            | -         | 0           | 1             | 1    |
|   12 | cerebrovascular_disease                | -         | 0           | 1             | 1    |
|   13 | dementia                               | -         | 0           | 1             | 1    |
|   14 | chronic_pulmonary_disease              | -         | 0           | 1             | 1    |
|   15 | rheumatic_disease                      | -         | 0           | 1             | 1    |
|   16 | peptic_ulcer_disease                   | -         | 0           | 1             | 1    |
|   17 | liver_disease_mild                     | -         | 0           | 1             | 1    |
|   18 | liver_disease_moderate_to_severe       | -         | 0           | 1             | 1    |
|   19 | diabetes_without_chronic_complications | -         | 0           | 1             | 1    |
|   20 | diabetes_with_chronic_complications    | -         | 0           | 1             | 1    |
|   21 | hemiplegia_or_paraplegia               | -         | 0           | 1             | 1    |
|   22 | renal_disease                          | -         | 0           | 1             | 1    |
|   23 | malignancy                             | -         | 0           | 1             | 1    |
|   24 | metastatic_solid_tumor                 | -         | 0           | 1             | 1    |
|   25 | aids                                   | -         | 0           | 1             | 1    |
|   26 | cardiac_arythmia                       | -         | 0           | 1             | 1    |
|   27 | valvular_disease                       | -         | 0           | 1             | 1    |
|   28 | pulmonary_circulatory_disorder         | -         | 0           | 1             | 1    |
|   29 | arterial_hypertension                  | -         | 0           | 1             | 1    |
|   30 | other_neurological_disorders           | -         | 0           | 1             | 1    |
|   31 | hypothyroidism                         | -         | 0           | 1             | 1    |
|   32 | coagulopathy                           | -         | 0           | 1             | 1    |
|   33 | obesity                                | -         | 0           | 1             | 1    |
|   34 | weight_loss                            | -         | 0           | 1             | 1    |
|   35 | fluid_and_electrolyte_disorders        | -         | 0           | 1             | 1    |
|   36 | blood_loss_anemia                      | -         | 0           | 1             | 1    |
|   37 | deficiency_anemia                      | -         | 0           | 1             | 1    |
|   38 | alcohol_abuse                          | -         | 0           | 1             | 1    |
|   39 | drug_abuse                             | -         | 0           | 1             | 1    |
|   40 | psychoses                              | -         | 0           | 1             | 1    |
|   41 | depression                             | -         | 0           | 1             | 1    |
|   42 | coronary_heart_disease                 | -         | 0           | 1             | 1    |
|   43 | chronic_pancreatitis                   | -         | 0           | 1             | 1    |
|   44 | ulcerative_colitis                     | -         | 0           | 1             | 1    |
|   45 | crohns_disease                         | -         | 0           | 1             | 1    |
|   46 | primary_system                         | -         | -           | -             | 2    |
|   47 | system_esophagus                       | -         | 0           | 1             | 1    |
|   48 | system_stomach                         | -         | 0           | 1             | 1    |
|   49 | system_intestine                       | -         | 0           | 1             | 1    |
|   50 | system_liver                           | -         | 0           | 1             | 1    |
|   51 | system_pancreas                        | -         | 0           | 1             | 1    |
|   52 | system_count                           | -         | 1           | 5             | 0    |
|   53 | urgency                                | -         | 0           | 5             | 1    |
|   54 | resurgery                              | -         | 0           | 1             | 1    |
|   55 | month                                  | -         | 0           | 11            | 1    |
|   56 | weekday                                | -         | 0           | 6             | 1    |
|   57 | daytime                                | -         | 0           | 2             | 1    |
|   58 | hour                                   | -         | 0           | 23            | 1    |
|   59 | mean_monthly_temperature               | °C        | -50         | 50            | 0    |
|   60 | minimum_monthly_temperature            | °C        | -50         | 50            | 0    |
|   61 | maximum_monthly_temperature            | °C        | -50         | 50            | 0    |
|   62 | monthly_precipitation                  | l / m^2   | 0           | 500           | 0    |
|   63 | monthly_sunshine_hours                 | h         | 0           | 744           | 0    |
|   64 | sodium                                 | mmol / l  | 50          | 200           | 0    |
|   65 | potassium                              | mmol / l  | 1           | 10            | 0    |
|   66 | bilirubin                              | mg / dl   | 0           | 50            | 0    |
|   67 | urea                                   | mg / dl   | 0           | 400           | 0    |
|   68 | ggt                                    | U / l     | 0           | 100,000       | 0    |
|   69 | lipase                                 | U / l     | 0           | 50,000        | 0    |
|   70 | crp                                    | mg / l    | 0           | 1,000         | 0    |
|   71 | hemoglobin                             | g / dl    | 0           | 40            | 0    |
|   72 | wbc                                    | / nl      | 0           | 100           | 0    |
|   73 | platelets                              | / nl      | 0           | 16,000,000    | 0    |
|   74 | hematocrit                             | l / l     | 0           | 1             | 0    |
|   75 | inr                                    | -         | 0           | 10            | 0    |
|   76 | aptt                                   | s         | 0           | 500           | 0    |
|   77 | erythrocytes                           | / pl      | 0           | 10            | 0    |
|   78 | creatinine                             | mg / dl   | 0           | 100           | 0    |
|   79 | glucose                                | mg / dl   | 0           | 1,000         | 0    |
|   80 | target_30_day_mortality                | -         | 0           | 1             | 1    |
|   81 | target_90_day_mortality                | -         | 0           | 1             | 1    |

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

Output: 1,286 cases

## Additional Notes

### Identifier Cohort

- **0:** Training Cohort _(Clinic 1: CVK & CCM)_
- **1:** Validation Cohort _(Clinic 2: CBF)_

### Daytime
- **0:** Night _(10pm <= t < 6am)_
- **1:** Morning _(6am <= t < 2pm)_
- **2:** Afternoon _(2pm <= t < 10pm)_