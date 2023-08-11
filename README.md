# CASSANDRAretro

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

| ID   | Name                       | Description                                                  | Completeness |
| :--- | :------------------------- | :----------------------------------------------------------- | :----------- |
| 0    | meta_case_id [Primary Key] | The identifier of the case                                   | 100 %        |
| 1    | meta_patient_id            | The identifier of the patient of the case                    | 99.85 %      |
| 2    | meta_surgery_id            | The identifier of the index surgery of the case              | 100 %        |
| 3    | meta_year                  | The year of the index surgery of the case                    | 100 %        |
| 4    | meta_system                | The system of the index surgery of the case                  | 99.51 %      |
| 5    | meta_ops                   | The ops of the index surgery of the case                     | 98.6 %       |
| 6    | meta_campus                | The campus where the index surgery of the case was performed | 99.38 %      |
| 7    | meta_admission_ts          | The admission timestamp of the case                          | 99.65 %      |
| 8    | meta_discharge_ts          | The discharge timestamp of the case                          | 99.65 %      |
| 9    | meta_incision_ts           | The incision timestamp of the index surgery of the case      | 100 %        |
| 10   | meta_suture_ts             | The suture timestamp of the index surgery of the case        | 100 %        |
| 11   | meta_icu_admission_ts      | The primary icu stay admission timestamp of the case         | 65.26 %      |
| 12   | meta_icu_discharge_ts      | The primary icu stay discharge timestamp of the case         | 65.26 %      |
| 13   | meta_follow_up_ts          | The follow up timestamp of the case                          | 99.85 %      |

### Features

| ID   | Name                                  | Description                                                                          | Completeness |
| :--- | :------------------------------------ | :----------------------------------------------------------------------------------- | :----------- |
| 14   | gender                                | The gender of the patient of the case                                                | 99.85 %      |
| 15   | age                                   | The age of the patient of the case                                                   | 99.85 %      |
| 16   | height                                | The height of the patient of the case                                                | 83.17 %      |
| 17   | weight                                | The weight of the patient of the case                                                | 85.42 %      |
| 18   | bmi                                   | The bmi of the patient of the case                                                   | 83.17 %      |
| 19   | asa                                   | The asa score of the patient of the case                                             | 89.6 %       |
| 20   | jones                                 | The jones score of the patient of the case                                           | 77.41 %      |
| 21   | ecog                                  | The ecog score of the patient of the case                                            | 77.41 %      |
| 22   | functional_status                     | The functional status of the patient of the case                                     | 77.41 %      |
| 23   | charlson_comorbidity_score            | The charlson comorbidity score of the patient of the case                            | 99.85 %      |
| 24   | condition_myocardial_infarction       | The information whether the patient of the case had suffered a heart attack          | 100 %        |
| 25   | condition_congestive_heart_failure    | The information whether the patient of the case has congestive heart failure         | 100 %        |
| 26   | condition_peripheral_vascular_disease | The information whether the patient of the case has peripheral vascular disease      | 100 %        |
| 27   | condition_cerebrovascular_disease     | The information whether the patient of the case suffers from cerebrovascular disease | 100 %        |
| 28   | condition_dementia                    | The information whether the patient of the case is suffering from dementia           | 100 %        |
| 29   | condition_chronic_pulmonary_disease   | The information whether the patient of the case has a chronic pulmonary disease      | 100 %        |
| 30   | condition_rheumatic_disease           | The information whether the patient of the case has a rheumatic disease              | 100 %        |
| 31   | condition_peptic_ulcer_disease        | The information whether the patient of the case has a peptic ulcer disease           | 100 %        |










