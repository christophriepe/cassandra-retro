# CASSANDRA retro

This is the documentation for the CASSANDRA retro dataset, which consists of a preoperative, intraoperative, postoperative and laboratory component. Thus, the dataset describes the entire medical course of 9,466 patients across settings and contains a total of 51,967,074 data points.

## Contact

If you have any questions about this dataset itself or its processing, feel free to contact me via eMail:

[christoph.riepe@charite.de](mailto:christoph.riepe@charite.de)

## Component Level Information

Specific information on the individual components of the overall data set can be found in the respective subfolders.

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

### Age

Only cases that were at least 18 years old at the time of the index operation were included.

## intraOP

The intraoperative data set, which accurately represents the condition of patients during surgery across a variety of different variables. The dataset consists of a total of 12,476,917 data points.

### Types

All types represented in the intraoperative dataset with the corresponding number of recorded events.

| ID   | Name         | Description                                  | N     |
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
| 9    | abg_methb    | ABG: Methemoglobin                           | 202,490   |
| 10   | abg_na       | ABG: Sodium                                  | 202,298   |
| 11   | abg_o2hb     | ABG: Oxyhemoglobin                           | 204,612   |
| 12   | abg_pco2     | ABG: Partial Pressure of Carbon Dioxide      | 201,423   |
| 13   | abg_ph       | ABG: Potential of Hydrogen                   | 203,156   |
| 14   | abg_po2      | ABG: Partial Pressure of Oxygen              | 200,861   |
| 15   | abg_sbe      | ABG: Standard Base Excess                    | 200,245   |
| 16   | abg_so2      | ABG: Oxygen Saturation                       | 204,468   |
| 17   | abg_t        | ABG: Temperature                             | 216,439   |
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

The postoperative data set, which accurately represents the condition of ICU patients across 38 different clinical variables. The dataset consists of a total of 32,320,093 data points. Since the IT system of the Charité has been changed in 2020, the postoperative data set originates from two different sources, COPRA 5 until 2020 and COPRA 6 from 2020 on. Not all clinical variables are available in both exports.

### Types

All types represented in the postoperative dataset with the corresponding number of recorded events.

| ID   | Name         | Description                                   | COPRA 5 | COPRA 6 | N         |
| :--- | :----------- | :-------------------------------------------- | :------ | :------ | :-------- |
| 0    | abg_abe      | Arterial Blood Gas (ABG): Actual Base Excess  | -       | X       | 198,383   |
| 1    | abg_ca       | ABG: Calcium                                  | X       | X       | 414,292   |
| 2    | abg_cl       | ABG: Chloride                                 | -       | X       | 186,076   |
| 3    | abg_cohb     | ABG: Carboxyhemoglobin                        | -       | X       | 196,710   |
| 4    | abg_fio2     | ABG: Fraction of Inspired Oxygen              | -       | X       | 210,218   |
| 5    | abg_glu      | ABG: Glucose                                  | X       | X       | 408,988   |
| 6    | abg_hco3     | ABG: Bicarbonate                              | X       | X       | 207,009   |
| 7    | abg_hct      | ABG: Hematocrit                               | X       | X       | 397,143   |
| 8    | abg_k        | ABG: Potassium                                | X       | X       | 407,536   |
| 9    | abg_lac      | ABG: Lactate                                  | X       | X       | 403,353   |
| 10   | abg_methb    | ABG: Methemoglobin                            | -       | X       | 196,622   |
| 11   | abg_na       | ABG: Sodium                                   | X       | X       | 404,510   |
| 12   | abg_o2hb     | ABG: Oxyhemoglobin                            | -       | X       | 202,575   |
| 13   | abg_pco2     | ABG: Partial Pressure of Carbon Dioxide       | X       | X       | 410,647   |
| 14   | abg_ph       | ABG: Potential of Hydrogen                    | X       | X       | 411,239   |
| 15   | abg_po2      | ABG: Partial Pressure of Oxygen               | X       | X       | 429,474   |
| 16   | abg_rhb      | ABG: Reduced Hemoglobin                       | -       | X       | 2,759     |
| 17   | abg_sbe      | ABG: Standard Base Excess                     | X       | X       | 402,326   |
| 18   | abg_so2      | ABG: Oxygen Saturation                        | X       | X       | 411,284   |
| 19   | abg_t        | ABG: Temperature                              | -       | X       | 215,939   |
| 20   | abg_thb      | ABG: Total Hemoglobin                         | X       | X       | 408,764   |
| 21   | bp_dia       | Blood Pressure: Diastolic                     | X       | X       | 3,839,803 |
| 22   | bp_sys       | Blood Pressure: Systolic                      | X       | X       | 3,839,712 |
| 23   | cvp          | Central Venous Pressure                       | X       | X       | 973,653   |
| 24   | dds          | Delirium Detection Score                      | X       | X       | 88,411    |
| 25   | drainage     | Drainage Output                               | X       | -       | 349,405   |
| 26   | fluid_in     | Fluid Intake                                  | X       | -       | 253,114   |
| 27   | fluid_out    | Fluid Output                                  | X       | -       | 553,899   |
| 28   | gcs          | Glasgow Coma Score                            | X       | X       | 302,316   |
| 29   | hr           | Heart Rate                                    | X       | X       | 3,838,976 |
| 30   | map          | Mean Arterial Pressure                        | X       | -       | 2,185,302 |
| 31   | pap          | Pulmonary Artery Pressure                     | X       | -       | 3,324     |
| 32   | rr           | Respiratory Rate                              | X       | X       | 3,040,922 |
| 33   | sao2         | Arterial Oxygen Saturation                    | X       | X       | 3,528,885 |
| 34   | saps2        | Simplified Acute Physiology Score II          | X       | -       | 58,292    |
| 35   | sofa         | Sepsis related Organ Failure Assessment Score | X       | -       | 58,220    |
| 36   | t            | Temperature                                   | X       | X       | 2,818,984 |
| 37   | tiss28       | Therapeutic Intervention Scoring System 28    | X       | -       | 61,028    |

## Lab Data

The laboratory dataset consists of 6,145,072 data points across 95 different laboratory values, accurately representing the laboratory medical aspect of the included case population over the entire hospital course.

### Types

An overview of the different laboratory values represented in the data set together with important key figures.

| ID   | Name      | Description                               | Dimension | N       |
| :--- | :-------- | :---------------------------------------- | :-------- | :------ |
| 0    | alat      | Alanin Aminotransferase                   | U/l       | 64,906  |
| 1    | alb       | Albumin                                   | g/l       | 25,953  |
| 2    | alp       | Alkaline Phosphatase                      | U/l       | 53,271  |
| 3    | ams       | Amylase                                   | U/l       | 1,856   |
| 4    | aptt      | Partial Thromboplastin Time               | sec       | 67,210  |
| 5    | asat      | Aspartate Aminotransferase                | U/l       | 66,266  |
| 6    | at        | Antithrombin                              | %         | 15,353  |
| 7    | baso      | Basophils                                 | /nl       | 15,358  |
| 8    | baso_rel  | Basophils Relative                        | %         | 15,421  |
| 9    | be        | Base Excess                               | mmol/l    | 328,758 |
| 10   | ca        | Calcium                                   | mmol/l    | 192,286 |
| 11   | ck        | Creatine Kinase                           | U/l       | 7,680   |
| 12   | ck_mb     | Creatine Kinase MB                        | U/l       | 4,494   |
| 13   | cl        | Chloride                                  | mmol/l    | 170,816 |
| 14   | cohb      | Carboxyhemoglobin                         | %         | 170,559 |
| 15   | cr        | Creatinine                                | mg/dl     | 82,413  |
| 16   | crp       | C Reactive Protein                        | mg/l      | 74,973  |
| 17   | cys_c     | Cystatin C                                | mg/l      | 761     |
| 18   | d_dim     | D Dimer                                   | mg/l      | 1,540   |
| 19   | dbil      | Direct Bilirubin                          | mg/dl     | 8,152   |
| 20   | ebl       | Erythroblasts                             | /nl       | 17,909  |
| 21   | ebl_rel   | Erythroblasts Relative                    | %         | 1,501   |
| 22   | eos       | Eosinophils                               | /nl       | 15,360  |
| 23   | eos_rel   | Eosinophils Relative                      | %         | 15,425  |
| 24   | fe        | Iron                                      | µmol/l    | 772     |
| 25   | fer       | Ferritin                                  | µg/l      | 1,238   |
| 26   | fg        | Fibrinogen                                | g/l       | 16,774  |
| 27   | fio2      | Fraction of Inspired Oxygen               | %         | 192,621 |
| 28   | gdh       | Glutamate Dehydrogenase                   | U/l       | 3,877   |
| 29   | ggt       | Gamma Glutamyltransferase                 | U/l       | 63,307  |
| 30   | glu       | Glucose                                   | mg/dl     | 219,035 |
| 31   | hb        | Hemoglobin                                | g/dl      | 274,925 |
| 32   | hba1c     | Glycated Hemoglobin                       | %         | 434     |
| 33   | hco3      | Bicarbonate                               | mmol/l    | 349,183 |
| 34   | hct       | Hematocrit                                | %         | 179,607 |
| 35   | hdl       | High Density Lipoprotein                  | mg/dl     | 563     |
| 36   | hhb       | Deoxyhemoglobin                           | %         | 120,952 |
| 37   | hp        | Haptoglobin                               | g/l       | 898     |
| 38   | ibil      | Indirect Bilirubin                        | mg/dl     | 3,471   |
| 39   | ig        | Immature Granulocytes                     | /nl       | 15,353  |
| 40   | ig_rel    | Immature Granulocytes Relative            | %         | 12,469  |
| 41   | iga       | Immunoglobulin A                          | g/l       | 546     |
| 42   | ige       | Immunoglobulin E                          | kU/l      | 38      |
| 43   | igg       | Immunoglobulin G                          | g/l       | 644     |
| 44   | igm       | Immunoglobulin M                          | g/l       | 552     |
| 45   | inr       | International Normalized Ratio            | -         | 82,166  |
| 46   | it_ratio  | I/T Ratio                                 | -         | 13,932  |
| 47   | k         | Potassium                                 | mmol/l    | 226,024 |
| 48   | lac       | Lactate                                   | mg/dl     | 179,682 |
| 49   | ldh       | Lactate Dehydrogenase                     | U/l       | 9,561   |
| 50   | ldl       | Low Density Lipoprotein                   | mg/dl     | 558     |
| 51   | lps       | Lipase                                    | U/l       | 52,896  |
| 52   | lym       | Lymphocytes                               | /nl       | 15,571  |
| 53   | lym_rel   | Lymphocytes Relative                      | %         | 15,676  |
| 54   | mb        | Myoglobin                                 | µg/l      | 3,051   |
| 55   | mch       | Mean Corpuscular Hemoglobin               | pg        | 92,828  |
| 56   | mchc      | Mean Corpuscular Hemoglobin Concentration | g/dl      | 92,828  |
| 57   | mcv       | Mean Corpuscular Volume                   | fl        | 92,866  |
| 58   | methb     | Methemoglobin                             | %         | 170,922 |
| 59   | mg        | Magnesium                                 | mmol/l    | 10,938  |
| 60   | mono      | Monocytes                                 | /nl       | 15,570  |
| 61   | mono_rel  | Monocytes Relative                        | %         | 15,684  |
| 62   | mpv       | Mean Platelet Volume                      | fl        | 89,408  |
| 63   | myelo     | Myelocytes                                | %         | 1,419   |
| 64   | na        | Sodium                                    | mmol/l    | 222,408 |
| 65   | nh3       | Ammonia                                   | µmol/l    | 1,176   |
| 66   | nt_probnp | N Terminal Pro B Type Natriuretic Peptide | ng/l      | 2,458   |
| 67   | o2hb      | Oxyhemoglobin                             | %         | 180,937 |
| 68   | pche      | Pseudocholinesterase                      | kU/l      | 4,038   |
| 69   | pco2      | Carbon Dioxide Partial Pressure           | mmHg      | 179,029 |
| 70   | pct       | Procalcitonin                             | µg/l      | 20,848  |
| 71   | ph        | Potential of Hydrogen                     | -         | 183,701 |
| 72   | plt       | Platelets                                 | /nl       | 92,906  |
| 73   | pmn       | Neutrophils                               | /nl       | 15,349  |
| 74   | pmn_rel   | Neutrophils Relative                      | %         | 12,467  |
| 75   | po2       | Oxygen Partial Pressure                   | mmHg      | 179,158 |
| 76   | po4       | Phosphate                                 | mmol/l    | 20,165  |
| 77   | pro       | Protein                                   | g/l       | 6,186   |
| 78   | quick     | Quick Value                               | %         | 82,252  |
| 79   | rbc       | Erythrocytes                              | /pl       | 92,824  |
| 80   | rdw       | Red Cell Distribution Width               | %         | 92,534  |
| 81   | rtic      | Reticulocytes                             | /nl       | 10,620  |
| 82   | schisto   | Schistocytes                              | %         | 775     |
| 83   | so2       | Oxygen Saturation                         | %         | 182,775 |
| 84   | t         | Temperature                               | °C        | 195,461 |
| 85   | tbil      | Total Bilirubin                           | mg/dl     | 127,374 |
| 86   | tc        | Total Cholesterol                         | mg/dl     | 1,158   |
| 87   | tg        | Total Triglycerides                       | mg/dl     | 2,694   |
| 88   | trans     | Transferrin                               | g/l       | 814     |
| 89   | ts        | Transferrin Saturation                    | %         | 657     |
| 90   | tsh       | Thyroid Stimulating Hormone               | mU/l      | 6,244   |
| 91   | ua        | Uric Acid                                 | mg/dl     | 2,735   |
| 92   | urea      | Urea                                      | mg/dl     | 75,074  |
| 93   | vd25      | 25 OH Vitamin D3                          | nmol/l    | 333     |
| 94   | wbc       | Leukocytes                                | /nl       | 92,862  |
