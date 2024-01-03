# Postoperative Data

The postoperative data set, which accurately represents the condition of ICU patients across 38 different clinical variables. The dataset consists of a total of 32,320,093 data points. Since the IT system of the Charité has been changed in 2020, the postoperative data set originates from two different sources, COPRA 5 until 2020 and COPRA 6 from 2020 on. Not all clinical variables are available in both exports.

## Types

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