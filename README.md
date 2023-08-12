# CASSANDRA retro

This is the documentation for the CASSANDRA retro data set. The data set consists of a pre-, intra- and postoperative component.

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

### Meta

| ID   | Name                       | Description                                      | Completeness |
| :--- | :------------------------- | :----------------------------------------------- | :----------- |
| 0    | meta_case_id [Primary Key] | The identifier of the case                       | 100 %        |
| 1    | meta_patient_id            | The identifier of the patient                    | 99.85 %      |
| 2    | meta_surgery_id            | The identifier of the index surgery              | 100 %        |
| 3    | meta_year                  | The year of the index surgery                    | 100 %        |
| 4    | meta_system                | The system of the index surgery                  | 99.51 %      |
| 5    | meta_ops                   | The ops of the index surgery                     | 98.6 %       |
| 6    | meta_campus                | The campus where the index surgery was performed | 99.38 %      |
| 7    | meta_admission_ts          | The admission timestamp of the case              | 99.65 %      |
| 8    | meta_discharge_ts          | The discharge timestamp of the case              | 99.65 %      |
| 9    | meta_incision_ts           | The incision timestamp of the index surgery      | 100 %        |
| 10   | meta_suture_ts             | The suture timestamp of the index surgery        | 100 %        |
| 11   | meta_icu_admission_ts      | The admission timestamp of the primary icu stay  | 65.26 %      |
| 12   | meta_icu_discharge_ts      | The discharge timestamp of the primary icu stay  | 65.26 %      |
| 13   | meta_follow_up_ts          | The follow up timestamp of the case              | 99.85 %      |

### Features

| ID   | Name                                                      | Description                                                                                      | Completeness |
| :--- | :-------------------------------------------------------- | :----------------------------------------------------------------------------------------------- | :----------- |
| 14   | gender                                                    | The gender of the patient                                                                        | 99.85 %      |
| 15   | age                                                       | The age of the patient                                                                           | 99.85 %      |
| 16   | height                                                    | The height of the patient                                                                        | 83.17 %      |
| 17   | weight                                                    | The weight of the patient                                                                        | 85.42 %      |
| 18   | bmi                                                       | The body mass index of the patient                                                               | 83.17 %      |
| 19   | asa                                                       | The asa score of the patient                                                                     | 89.6 %       |
| 20   | jones                                                     | The jones score of the patient                                                                   | 77.41 %      |
| 21   | ecog                                                      | The ecog score of the patient                                                                    | 77.41 %      |
| 22   | functional_status                                         | The functional status of the patient                                                             | 77.41 %      |
| 23   | charlson_comorbidity_score                                | The charlson comorbidity score of the patient                                                    | 99.85 %      |
| 24   | condition_myocardial_infarction                           | The information whether the patient had suffered a myocardial infarction                         | 100 %        |
| 25   | condition_congestive_heart_failure                        | The information whether the patient has congestive heart failure                                 | 100 %        |
| 26   | condition_peripheral_vascular_disease                     | The information whether the patient has peripheral vascular disease                              | 100 %        |
| 27   | condition_cerebrovascular_disease                         | The information whether the patient has cerebrovascular disease                                  | 100 %        |
| 28   | condition_dementia                                        | The information whether the patient has dementia                                                 | 100 %        |
| 29   | condition_chronic_pulmonary_disease                       | The information whether the patient has a chronic pulmonary disease                              | 100 %        |
| 30   | condition_rheumatic_disease                               | The information whether the patient has a rheumatic disease                                      | 100 %        |
| 31   | condition_peptic_ulcer_disease                            | The information whether the patient has a peptic ulcer disease                                   | 100 %        |
| 32   | condition_liver_disease_mild                              | The information whether the patient has a mild liver disease                                     | 100 %        |
| 33   | condition_liver_disease_moderate_to_severe                | The information whether the patient has a moderate to severe liver disease                       | 100 %        |
| 34   | condition_diabetes_without_chronic_complications          | The information whether the patient has a diabetes without chronic complications                 | 100 %        |
| 35   | condition_diabetes_with_chronic_complications             | The information whether the patient has a diabetes with chronic complications                    | 100 %        |
| 36   | condition_renal_disease_mild_to_moderate                  | The information whether the patient has a mild to moderate renal disease                         | 100 %        |
| 37   | condition_renal_disease_severe                            | The information whether the patient has a severe renal disease                                   | 100 %        |
| 38   | condition_hemiplegia_or_paraplegia                        | The information whether the patient has a hemiplegia or paraplegia                               | 100 %        |
| 39   | condition_malignancy                                      | The information whether the patient has any malignancy                                           | 100 %        |
| 40   | condition_metastatic_solid_tumor                          | The information whether the patient has a metastatic solid tumor                                 | 100 %        |
| 41   | condition_hiv_without_aids                                | The information whether the patient has HIV without AIDS                                         | 100 %        |
| 42   | condition_aids                                            | The information whether the patient has AIDS                                                     | 100 %        |
| 43   | surgery_year                                              | The year of the index surgery                                                                    | 100 %        |
| 44   | surgery_system [One Hot Encoding (x5)]                    | The system of the index surgery                                                                  | 99.51 %      |
| 45   | surgery_ops [One Hot Encoding (x20)]                      | The ops of the index surgery                                                                     | 98.6 %       |
| 46   | surgery_urgency                                           | The urgency of the index surgery                                                                 | 99.87 %      |
| 47   | surgery_approach [One Hot Encoding (x3)]                  | The approach of the index surgery                                                                | 57.05 %      |
| 48   | surgery_pancreatic_resection [One Hot Encoding (x4)]      | The information whether a pancreatic resection was performed during index surgery                | 100 %        |
| 49   | surgery_pancreatic_reconstruction                         | The information whether a pancreatic reconstruction was performed during index surgery           | 100 %        |
| 50   | surgery_liver_resection [One Hot Encoding (x2)]           | The information whether a liver resection was performed during index surgery                     | 100 %        |
| 51   | surgery_esophageal_resection [One Hot Encoding (x3)]      | The information whether an esophageal resection was performed during index surgery               | 100 %        |
| 52   | surgery_esophageal_anastomosis [One Hot Encoding (x4)]    | The information whether an esophageal anastomosis was performed during index surgery             | 100 %        |
| 53   | surgery_gastric_resection [One Hot Encoding (x3)]         | The information whether a gastric resection was performed during index surgery                   | 100 %        |
| 54   | surgery_gastric_reconstruction [One Hot Encoding (x5)]    | The information whether a gastric reconstruction was performed during index surgery              | 100 %        |
| 55   | surgery_small_intestine_resection [One Hot Encoding (x3)] | The information whether a resection of the small intestine was performed during index surgery    | 100 %        |
| 56   | surgery_small_intestine_anastomosis                       | The information whether an anastomosis of the small intestine was performed during index surgery | 100 %        |
| 57   | surgery_colon_resection [One Hot Encoding (x9)]           | The information whether a colon resection was performed during index surgery                     | 100 %        |
| 58   | surgery_colon_anastomosis                                 | The information whether a colon anastomosis was performed during index surgery                   | 100 %        |
| 59   | surgery_rectum_resection [One Hot Encoding (x3)]          | The information whether a rectum resection was performed during index surgery                    | 100 %        |
| 60   | surgery_rectum_anastomosis                                | The information whether a rectum anastomosis was performed during index surgery                  | 100 %        |
| 61   | surgery_stoma_relocation                                  | The information whether a stoma relocation was performed during index surgery                    | 100 %        |
| 62   | surgery_reconnection                                      | The information whether a reconnection was performed during index surgery                        | 100 %        |
| 63   | surgery_liver_transplantation [One Hot Encoding (x2)]     | The information whether a liver transplantation was performed during index surgery               | 100 %        |
| 64   | surgery_kidney_transplantation [One Hot Encoding (x2)]    | The information whether a kidney transplantation was performed during index surger               | 100 %        |
| 65   | surgery_pancreas_transplantation                          | The information whether a pancreas transplantation was performed during index surgery            | 100 %        |
| 66   | surgery_cholecystectomy                                   | The information whether a cholecystectomy was performed during index surgery                     | 100 %        |
| 67   | surgery_additional_cholecystectomy                        | The information whether an additional cholecystectomy was performed during index surgery         | 100 %        |
| 68   | surgery_lung_resection                                    | The information whether a lung resection was performed during index surgery                      | 100 %        |
| 69   | surgery_kidney_resection                                  | The information whether a kidney resection was performed during index surgery                    | 100 %        |
| 70   | surgery_another_organs_or_delbuking                       | The information whether another organ or delbuking was performed during index surgery            | 100 %        |
| 71   | surgery_vascular_resection                                | The information whether a vascular resection was performed during index surgery                  | 100 %        |
| 72   | surgery_biliodigestive_anastomosis                        | The information whether a biliodigestive anastomosis was performed during index surgery          | 100 %        |
| 73   | surgery_splenectomy                                       | The information whether a splenectomy was performed during index surgery                         | 100 %        |
| 74   | surgery_simultaneous_hernia_management                    | The information whether a simultaneous hernia management was performed during index surgery      | 100 %        |
| 75   | surgery_simultaneous_ablation                             | The information whether a simultaneous ablation was performed during index surgery               | 100 %        |
| 76   | surgery_stoma_facility                                    | The information whether a stoma facility was performed during index surgery                      | 100 %        |
| 77   | surgery_hipec                                             | The information whether hipec was performed during index surgery                                 | 100 %        |

### Targets



