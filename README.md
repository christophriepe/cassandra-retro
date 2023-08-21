# CASSANDRA retro

This is the documentation for the CASSANDRA retro dataset. The dataset consists of a pre-, intra- and postoperative component.

## Contact
If you have any questions about this dataset itself or its processing, feel free to contact me via eMail:

[christoph.riepe@charite.de](mailto:christoph.riepe@charite.de)

## Inclusion Criteria
Inclusion criteria were defined based on the following three characteristics. A more detailed description of the included values of these characteristics follows in the further course.

- Year
- System
- OPS

### Years
All cases in which the index surgery was performed in one of the following eight years were included. 

| ID   | Year |
| :--- | :--- |
| 0    | 2014 |
| 1    | 2015 |
| 2    | 2016 |
| 3    | 2017 |
| 4    | 2018 |
| 5    | 2019 |
| 6    | 2020 |
| 7    | 2021 |


### Systems
All cases in which the index surgery was performed on one of the following five organ systems were included.

| ID   | System    |
| :--- | :---      |
| 0    | Esophagus |
| 1    | Stomach   |
| 2    | Intestine |
| 3    | Liver     |
| 4    | Pancreas  |

### OPS
All cases in which the index surgery was defined by one of the following OPS were included.

| ID   | OPS   | System | Description                                                                                |
| :--- | :---- | :----- | :----------------------------------------------------------------------------------------- |
| 0    | 5-423 | 0      | Partielle Ösophagusresektion ohne Wiederherstellung der Kontinuität                        |
| 1    | 5-424 | 0      | Partielle Ösophagusresektion mit Wiederherstellung der Kontinuität                         |
| 2    | 5-425 | 0      | (Totale) Ösophagektomie ohne Wiederherstellung der Kontinuität                             |
| 3    | 5-426 | 0      | (Totale) Ösophagektomie mit Wiederherstellung der Kontinuität                              |
| 4    | 5-427 | 0      | Rekonstruktion der Ösophaguspassage (als selbständiger Eingriff)                           |
| 5    | 5-434 | 1      | Atypische partielle Magenresektion                                                         |
| 6    | 5-435 | 1      | Partielle Magenresektion (2/3-Resektion)                                                   |
| 7    | 5-436 | 1      | Subtotale Magenresektion (4/5-Resektion)                                                   |
| 8    | 5-437 | 1      | (Totale) Gastrektomie                                                                      |
| 9    | 5-438 | 1      | (Totale) Gastrektomie mit Ösophagusresektion                                               |
| 10   | 5-454 | 2      | Resektion des Dünndarmes                                                                   |
| 11   | 5-455 | 2      | Partielle Resektion des Dickdarmes                                                         |
| 12   | 5-456 | 2      | (Totale) Kolektomie und Proktokolektomie                                                   |
| 13   | 5-465 | 2      | Rückverlagerung eines doppelläufigen Enterostomas                                          |
| 14   | 5-466 | 2      | Wiederherstellung der Kontinuität des Darmes bei endständigen Enterostomata                |
| 15   | 5-484 | 2      | Rektumresektion unter Sphinktererhaltung                                                   |
| 16   | 5-485 | 2      | Rektumresektion ohne Sphinktererhaltung                                                    |
| 17   | 5-501 | 3      | Lokale Exzision und Destruktion von erkranktem Gewebe der Leber (atypische Leberresektion) |
| 18   | 5-502 | 3      | Anatomische (typische) Leberresektion                                                      |
| 19   | 5-524 | 4      | Partielle Resektion des Pankreas                                                           |
| 20   | 5-525 | 4      | (Totale) Pankreatektomie                                                                   |

## preOP

The preoperative data set, which accurately represents the condition of patients before their index surgery. The dataset consists of a total of 90 variables or 144 variables after one hot encoding.

### Meta

The meta variables of the dataset.

| ID   | Name                  | Description                                      | Completeness | Note        |
| :--- | :-------------------- | :----------------------------------------------- | :----------- | :---------- |
| 0    | meta_case_id          | The identifier of the case                       | 100 %        | Primary Key |
| 1    | meta_patient_id       | The identifier of the patient                    | 99.85 %      |             |
| 2    | meta_surgery_id       | The identifier of the index surgery              | 100 %        |             |
| 3    | meta_year             | The year of the index surgery                    | 100 %        |             |
| 4    | meta_system           | The system of the index surgery                  | 99.51 %      |             |
| 5    | meta_ops              | The ops of the index surgery                     | 98.6 %       |             |
| 6    | meta_campus           | The campus where the index surgery was performed | 99.38 %      |             |
| 7    | meta_admission_ts     | The admission timestamp of the case              | 99.65 %      |             |
| 8    | meta_discharge_ts     | The discharge timestamp of the case              | 99.65 %      |             |
| 9    | meta_incision_ts      | The incision timestamp of the index surgery      | 100 %        |             |
| 10   | meta_suture_ts        | The suture timestamp of the index surgery        | 100 %        |             |
| 11   | meta_icu_admission_ts | The admission timestamp of the primary icu stay  | 65.26 %      |             |
| 12   | meta_icu_discharge_ts | The discharge timestamp of the primary icu stay  | 65.26 %      |             |
| 13   | meta_follow_up_ts     | The follow up timestamp of the case              | 99.85 %      |             |

### Features

The preoperative variables of the dataset which can be used as features.

| ID   | Name                                             | Description                                                                                      | Completeness | Note          |
| :--- | :----------------------------------------------- | :----------------------------------------------------------------------------------------------- | :----------- | :------------ |
| 14   | gender                                           | The gender of the patient                                                                        | 99.85 %      |               |
| 15   | age                                              | The age of the patient                                                                           | 99.85 %      |               |
| 16   | height                                           | The height of the patient                                                                        | 83.17 %      |               |
| 17   | weight                                           | The weight of the patient                                                                        | 85.42 %      |               |
| 18   | bmi                                              | The body mass index of the patient                                                               | 83.17 %      |               |
| 19   | asa                                              | The asa score of the patient                                                                     | 89.6 %       |               |
| 20   | jones                                            | The jones score of the patient                                                                   | 77.41 %      |               |
| 21   | ecog                                             | The ecog score of the patient                                                                    | 77.41 %      |               |
| 22   | functional_status                                | The functional status of the patient                                                             | 77.41 %      |               |
| 23   | charlson_comorbidity_score                       | The charlson comorbidity score of the patient                                                    | 99.85 %      |               |
| 24   | condition_myocardial_infarction                  | The information whether the patient had suffered a myocardial infarction                         | 100 %        |               |
| 25   | condition_congestive_heart_failure               | The information whether the patient has congestive heart failure                                 | 100 %        |               |
| 26   | condition_peripheral_vascular_disease            | The information whether the patient has peripheral vascular disease                              | 100 %        |               |
| 27   | condition_cerebrovascular_disease                | The information whether the patient has cerebrovascular disease                                  | 100 %        |               |
| 28   | condition_dementia                               | The information whether the patient has dementia                                                 | 100 %        |               |
| 29   | condition_chronic_pulmonary_disease              | The information whether the patient has a chronic pulmonary disease                              | 100 %        |               |
| 30   | condition_rheumatic_disease                      | The information whether the patient has a rheumatic disease                                      | 100 %        |               |
| 31   | condition_peptic_ulcer_disease                   | The information whether the patient has a peptic ulcer disease                                   | 100 %        |               |
| 32   | condition_liver_disease_mild                     | The information whether the patient has a mild liver disease                                     | 100 %        |               |
| 33   | condition_liver_disease_moderate_to_severe       | The information whether the patient has a moderate to severe liver disease                       | 100 %        |               |
| 34   | condition_diabetes_without_chronic_complications | The information whether the patient has a diabetes without chronic complications                 | 100 %        |               |
| 35   | condition_diabetes_with_chronic_complications    | The information whether the patient has a diabetes with chronic complications                    | 100 %        |               |
| 36   | condition_renal_disease_mild_to_moderate         | The information whether the patient has a mild to moderate renal disease                         | 100 %        |               |
| 37   | condition_renal_disease_severe                   | The information whether the patient has a severe renal disease                                   | 100 %        |               |
| 38   | condition_hemiplegia_or_paraplegia               | The information whether the patient has a hemiplegia or paraplegia                               | 100 %        |               |
| 39   | condition_malignancy                             | The information whether the patient has any malignancy                                           | 100 %        |               |
| 40   | condition_metastatic_solid_tumor                 | The information whether the patient has a metastatic solid tumor                                 | 100 %        |               |
| 41   | condition_hiv_without_aids                       | The information whether the patient has HIV without AIDS                                         | 100 %        |               |
| 42   | condition_aids                                   | The information whether the patient has AIDS                                                     | 100 %        |               |
| 43   | surgery_year                                     | The year of the index surgery                                                                    | 100 %        |               |
| 44   | surgery_system                                   | The system of the index surgery                                                                  | 99.51 %      | One Hot (x5)  |
| 45   | surgery_ops                                      | The ops of the index surgery                                                                     | 98.6 %       | One Hot (x20) |
| 46   | surgery_urgency                                  | The urgency of the index surgery                                                                 | 99.87 %      |               |
| 47   | surgery_approach                                 | The approach of the index surgery                                                                | 57.05 %      | One Hot (x3)  |
| 48   | surgery_pancreatic_resection                     | The information whether a pancreatic resection was performed during index surgery                | 100 %        | One Hot (x4)  |
| 49   | surgery_pancreatic_reconstruction                | The information whether a pancreatic reconstruction was performed during index surgery           | 100 %        |               |
| 50   | surgery_liver_resection                          | The information whether a liver resection was performed during index surgery                     | 100 %        | One Hot (x2)  |
| 51   | surgery_esophageal_resection                     | The information whether an esophageal resection was performed during index surgery               | 100 %        | One Hot (x3)  |
| 52   | surgery_esophageal_anastomosis                   | The information whether an esophageal anastomosis was performed during index surgery             | 100 %        | One Hot (x4)  |
| 53   | surgery_gastric_resection                        | The information whether a gastric resection was performed during index surgery                   | 100 %        | One Hot (x3)  |
| 54   | surgery_gastric_reconstruction                   | The information whether a gastric reconstruction was performed during index surgery              | 100 %        | One Hot (x5)  |
| 55   | surgery_small_intestine_resection                | The information whether a resection of the small intestine was performed during index surgery    | 100 %        | One Hot (x3)  |
| 56   | surgery_small_intestine_anastomosis              | The information whether an anastomosis of the small intestine was performed during index surgery | 100 %        |               |
| 57   | surgery_colon_resection                          | The information whether a colon resection was performed during index surgery                     | 100 %        | One Hot (x9)  |
| 58   | surgery_colon_anastomosis                        | The information whether a colon anastomosis was performed during index surgery                   | 100 %        |               |
| 59   | surgery_rectum_resection                         | The information whether a rectum resection was performed during index surgery                    | 100 %        | One Hot (x3)  |
| 60   | surgery_rectum_anastomosis                       | The information whether a rectum anastomosis was performed during index surgery                  | 100 %        |               |
| 61   | surgery_stoma_relocation                         | The information whether a stoma relocation was performed during index surgery                    | 100 %        |               |
| 62   | surgery_reconnection                             | The information whether a reconnection was performed during index surgery                        | 100 %        |               |
| 63   | surgery_liver_transplantation                    | The information whether a liver transplantation was performed during index surgery               | 100 %        | One Hot (x2)  |
| 64   | surgery_kidney_transplantation                   | The information whether a kidney transplantation was performed during index surger               | 100 %        | One Hot (x2)  |
| 65   | surgery_pancreas_transplantation                 | The information whether a pancreas transplantation was performed during index surgery            | 100 %        |               |
| 66   | surgery_cholecystectomy                          | The information whether a cholecystectomy was performed during index surgery                     | 100 %        |               |
| 67   | surgery_additional_cholecystectomy               | The information whether an additional cholecystectomy was performed during index surgery         | 100 %        |               |
| 68   | surgery_lung_resection                           | The information whether a lung resection was performed during index surgery                      | 100 %        |               |
| 69   | surgery_kidney_resection                         | The information whether a kidney resection was performed during index surgery                    | 100 %        |               |
| 70   | surgery_another_organs_or_delbuking              | The information whether another organ or delbuking was performed during index surgery            | 100 %        |               |
| 71   | surgery_vascular_resection                       | The information whether a vascular resection was performed during index surgery                  | 100 %        |               |
| 72   | surgery_biliodigestive_anastomosis               | The information whether a biliodigestive anastomosis was performed during index surgery          | 100 %        |               |
| 73   | surgery_splenectomy                              | The information whether a splenectomy was performed during index surgery                         | 100 %        |               |
| 74   | surgery_simultaneous_hernia_management           | The information whether a simultaneous hernia management was performed during index surgery      | 100 %        |               |
| 75   | surgery_simultaneous_ablation                    | The information whether a simultaneous ablation was performed during index surgery               | 100 %        |               |
| 76   | surgery_stoma_facility                           | The information whether a stoma facility was performed during index surgery                      | 100 %        |               |
| 77   | surgery_hipec                                    | The information whether hipec was performed during index surgery                                 | 100 %        |               |

### Targets

The postoperative variables of the dataset which can be used as targets.

| ID   | Name                              | Description                                                                      | Completeness | Note |
| :--- | :-------------------------------- | :------------------------------------------------------------------------------- | :----------- | :--- |
| 78   | target_30_day_mortality           | The information whether the patient died within 30 days                          | 98.48 %      |      |
| 79   | target_90_day_mortality           | The information whether the patient died within 90 days                          | 81.31 %      |      |
| 80   | target_death_within_primary_stay  | The information whether the patient died within the primary stay                 | 99.65 %      |      |
| 81   | target_icu_readmission            | The information whether the patient was admitted back to the icu after discharge | 99.65 %      |      |
| 82   | target_resurgery                  | The information whether the patient had a resurgery during primary stay          | 100 %        |      |
| 83   | target_number_of_surgeries        | The number of surgeries the patient has had during primary stay                  | 100 %        |      |
| 84   | target_discharge_ts               | The discharge timestamp of the case                                              | 99.65%       |      |
| 85   | target_length_of_stay             | The length of the primary stay in nights                                         | 99.65 %      |      |
| 86   | target_number_of_icu_stays        | The number of icu stays the patient has had during primary stay                  | 99.65 %      |      |
| 87   | target_nights_on_primary_icu_stay | The length of the primary icu stay in nights                                     | 99.65 %      |      |
| 88   | target_number_of_icu_readmissions | The number of icu readmissions the patient has had during primary stay           | 99.65 %      |      |
| 89   | target_surgery_duration           | The duration of the index surgery of the case                                    | 100.0 %      |      |

## intraOP

The intraoperative data set, which accurately represents the condition of patients during surgery across a variety of different variables. The dataset consists of a total of 12,476,917 data points.

### Types

All types represented in the intraoperative dataset with the corresponding number of recorded events.

| ID   | Name         | Description                                  | Count     |
| :--- | :----------- | :------------------------------------------  | :-------- |
| 0    | abg_abe      | Arterial Blood Gas (ABG): Actual Base Excess | 200,298   |
| 1    | abg_ca       | ABG: Calcium                                 | 211,676   |
| 2    | abg_cl       | ABG: Chloride                                | 190,786   |
| 3    | abg_cohb     | ABG: Carboxyhemoglobin                       | 202,558   |
| 4    | abg_fio2     | ABG: Fraction of Inspired Oxygen             | 213,099   |
| 5    | abg_glu      | ABG: Glucose                                 | 204,956   |
| 6    | abg_hct      | ABG: Hematocrit                              | 201,470   |
| 7    | abg_k        | ABG: Potassium                               | 204,976   |
| 8    | abg_lac      | ABG: Lactate                                 | 201,436   |
| 9    | abg_met_hb   | ABG: Methemoglobin                           | 202,490   |
| 10   | abg_na       | ABG: Sodium                                  | 202,298   |
| 11   | abg_o2hb     | ABG: Oxyhemoglobin                           | 204,612   |
| 12   | abg_pco2     | ABG: Partial Pressure of Carbon Dioxide      | 201,423   |
| 13   | abg_ph       | ABG: Potential of Hydrogen                   | 203,156   |
| 14   | abg_po2      | ABG: Partial Pressure of Oxygen              | 200,861   |
| 15   | abg_sbe      | ABG: Standard Base Excess                    | 200,245   |
| 16   | abg_so2      | ABG: Oxygen Saturation                       | 204,468   |
| 17   | abg_temp     | ABG: Temperature                             | 216,439   |
| 18   | abg_thb      | ABG: Total Hemoglobin                        | 204,484   |
| 19   | bp_dia       | Blood Pressure: Diastolic                    | 1,839,639 |
| 20   | bp_sys       | Blood Pressure: Systolic                     | 1,840,497 |
| 21   | capno_et_co2 | Capnometry: Endtidal Carbon Dioxide          | 297,967   |
| 22   | cvd          | Central Venous Pressure                      | 322,280   |
| 23   | exp_no       | Expiratory Nitrous Oxide                     | 278,616   |
| 24   | exp_sevo     | Expiratory Sevoflurane                       | 168,519   |
| 25   | fio2         | Fraction of Inspired Oxygen                  | 295,714   |
| 26   | hr           | Heart Rate                                   | 1,011,846 |
| 27   | rmv          | Respiratory Minute Volume                    | 289,975   |
| 28   | rr           | Respiratory Rate                             | 346,573   |
| 29   | sao2         | Arterial Oxygen Saturation                   | 797,748   |
| 30   | sedline      | Sedline                                      | 72,691    |
| 31   | temp         | Temperature                                  | 475,443   |
| 32   | vent_p_peak  | Ventilation: Peak Pressure                   | 285,899   |
| 33   | vent_peep    | Ventilation: Positive Endexpiratory Pressure | 281,779   |

## postOP

The postoperative data set, which accurately represents the condition of ICU patients across a variety of different variables. The dataset consists of a total of 22,358,778 data points.

### Types

All types represented in the postoperative dataset with the corresponding number of recorded events.

| ID   | Name         | Description                                          | Count     |
| :--- | :----------- | :--------------------------------------------------- | :-------- |
| 0    | abg_ca       | Arterial Blood Gas (ABG): Calcium                    | 205,118   |
| 1    | abg_glu      | ABG: Glucose                                         | 206,429   |
| 2    | abg_hb       | ABG: Hemoglobin                                      | 206,575   |
| 3    | abg_hco3     | ABG: Bicarbonate                                     | 205,728   |
| 4    | abg_hct      | ABG: Hematocrit                                      | 200,578   |
| 9    | abg_k        | ABG: Potassium                                       | 205,543   |
| 5    | abg_lac      | ABG: Lactate                                         | 205,191   |
| 12   | abg_na       | ABG: Sodium                                          | 205,245   |
| 6    | abg_pco2     | ABG: Partial Pressure of Carbon Dioxide              | 208,354   |
| 7    | abg_ph       | ABG: Potential of Hydrogen                           | 209,719   |
| 8    | abg_po2      | ABG: Partial Pressure of Oxygen                      | 231,334   |
| 10   | abg_sbe      | ABG: Standard Base Excess                            | 204,797   |
| 11   | abg_so2      | ABG: Oxygen Saturation                               | 209,468   |
| 13   | bp_dia       | Blood Pressure: Diastolic                            | 2,723,660 |
| 15   | bp_sys       | Blood Pressure: Systolic                             | 2,723,442 |
| 16   | cvp          | Central Venous Pressure                              | 821,441   |
| 17   | drainage     | Drainage Output                                      | 349,405   |
| 18   | fluid_in     | Fluid Intake                                         | 253,114   |
| 19   | fluid_out    | Fluid Output                                         | 553,899   |
| 20   | hr           | Heart Rate                                           | 2,639,607 |
| 14   | map          | Mean Arterial Pressure                               | 2,185,302 |
| 21   | rr           | Respiratory Rate                                     | 2,296,077 |
| 22   | sao2         | Arterial Oxygen Saturation                           | 2,522,500 |
| 23   | score_dds    | Score: Diabetes Distress Scale                       | 84,391    |
| 24   | score_gcs    | Score: Glasgow Coma Score                            | 233,180   |
| 25   | score_saps2  | Score: Simplified Acute Physiology Score II          | 58,292    |
| 26   | score_sofa   | Score: Sepsis related Organ Failure Assessment Score | 58,220    |
| 27   | score_tiss28 | Score: Therapeutic Intervention Scoring System 28    | 61,028    |
| 28   | temp         | Temperature                                          | 2,091,141 |

## Lab Data

The laboratory dataset consists of 6,145,072 data points across 95 different laboratory values, accurately representing the laboratory medical aspect of the included case population over the entire hospital course.

### Types

An overview of the different laboratory values represented in the data set together with important key figures.

| ID   | Name         | Description                    | Dimension | N      |
| :--- | :----------- | :----------------------------- | :-------- | :----- |
| 0    | vd25         | 25 OH Vitamin D3               | nmol/l    | 333    |
| 1    | alat         | Alanin Aminotransferase (ALAT) | U/l       | 64,906 |
| 2    | alb          | Albumin                        | g/l       | 64,906 |
| 3    | alp          | Alkaline Phosphatase           | U/l       | 53,271 |
| 4    | ams          | Amylase                        | U/l       | 1,856  |








