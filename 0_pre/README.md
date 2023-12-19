# preOP Data

## Data Structure

|          | ID  | Feature | Dimension | Completeness (%) | Min | Max |
| -------- | --- | ------- | --------- | ---------------- | --- | --- |
| Meta     |     |         |           |                  |     |     |
|          | 0   | center  |           | 100              |     |     |
|          | 1   | date    |           | 100              |     |     |
|          | ... | ...     |           | ...              |     |     |
| Features |     |         |           |                  |     |     |
|          | 2   | gender  | -         | 94.61            | -   | -   |
|          | 3   | age     |           | 100              | 18  | 120 |
|          | 4   | height  | cm        | 74.48            |     | 250 |
|          | 5   | weight  | kg        | 85.78            |     | 250 |
|          | 6   | bmi     | kg/m²     | 72.37            |     |     |

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

### Summer Day
Meteorologists define a summer day as a day with a maximum temperature of at least 25 degrees Celsius. The average number of summer days is used to characterize the climate. In Central Europe, temperatures above 30 degrees Celsius are referred to as a tropical day or hot day. ~ WetterKontor

### Hot Day
In meteorology, a hot day, also known as a tropical day, is a day on which the air temperature reaches or exceeds 30 degrees Celsius. In Germany, there are relatively few tropical days per year. Berlin, for example, has 6 tropical days per year. This figure is an average value calculated from many years of observation. ~ WetterKontor

### Frost Day
Weather forecasters define frost days as days on which the air temperature at an altitude of 2 meters temporarily drops below 0 degrees Celsius. Such a day is also known as a frost change day. Berlin has an average of 88 frost days per year. The average number of frost days is used to characterize the climate. ~ WetterKontor

### Ice Day
A day with a maximum temperature below freezing point. By definition, the number of ice days is included in the number of frost days, as the lowest air temperature is below 0 degrees Celsius on both an ice day and a frost day. Every ice day is therefore also counted as a frost day. The average number of ice days is used to characterize the climate. ~ WetterKontor

