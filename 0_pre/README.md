# preOP Data

## Data Structure

|          | ID  | Feature | Completeness (%) | Min | Max |
| -------- | --- | ------- | ---------------- | --- | --- |
| Meta     |     |         |                  |     |     |
|          | 0   | center  | 100              |     |     |
|          | 1   | date    | 100              |     |     |
|          | ... | ...     | ...              |     |     |
| Features |     |         |                  |     |     |
|          | 2   | gender  | 94.61            |     |     |
|          | 3   | age     | 100              |     |     |
|          | 4   | height  | 74.48            |     |     |
|          | 5   | weight  | 85.78            |     |     |
|          | 6   | bmi     | 72.37            |     |     |

## Additional Notes

### Renal Insufficiency

The "renal_insufficiency" feature corresponds to a degree of renal insufficiency and is defined by the GFR (glomerular filtration rate). The following categories are defined:

| ID  | Stadium | GFR (mL/min/1.73 m2) | ICD-10 | Description                             |
| --- | ------- | -------------------- | ------ | --------------------------------------- |
| 0   | 1       | ≥ 90                 | N18.1  | ... with normal kidney function         |
| 1   | 2       | 60 - 89              | N18.2  | ... with mild functional impairment     |
| 2   | 3       | 30 - 59              | N18.3  | ... with moderate functional impairment |
| 3   | 4       | 15 - 29              | N18.4  | ... with severe functional impairment   |
| 4   | 5       | < 15                 | N18.5  | ... with renal failure                  |