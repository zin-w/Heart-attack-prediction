# Heart-attack-prediction

A machine learning model that predicts the likelihood of heart attacks based on clinical data. Built for educational and research purposes.

In this project, we'd dive into heart attack prediction, using the data from kaggle

___

## Dataset

- **Source:** https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction
- **Rows:** 1190 observations
  This dataset was created by combining different datasets already available independently but not combined before. In this dataset, 5 heart datasets are combined over 11 common features which makes it the largest heart disease dataset available so far for research purposes. The five datasets used for its curation are:
  1. `Cleveland`: 303 observations,
  2. `Hungarian`: 294 observations,
  3. `Switzerland`: 123 observations,
  4. `Long Beach VA`: 200 observations,
  5. `Stalog (Heart)`: Data Set: 270 observations

  Total: 1190 observations,
  Duplicated: 272 observations

  **Final dataset: 918 observations**
  
- **Categories:**
  1. `Age`: age of the patient [years]
  2. `Sex`: sex of the patient [M: Male, F: Female]
  3. `ChestPainType`: chest pain type [TA: Typical Angina, ATA: Atypical Angina, NAP: Non-Anginal Pain, ASY: Asymptomatic]
  4. `RestingBP`: resting blood pressure [mm Hg]
  5. `Cholesterol`: serum cholesterol [mm/dl]
  6. `FastingBS`: fasting blood sugar [1: if FastingBS > 120 mg/dl, 0: otherwise]
  7. `RestingECG`: resting electrocardiogram results [Normal: Normal, ST: having ST-T wave abnormality (T wave inversions and/or ST elevation or depression of > 0.05 mV), LVH: showing probable or definite left ventricular hypertrophy by Estes' criteria]
  8. `MaxHR`: maximum heart rate achieved [Numeric value between 60 and 202]
  9. `ExerciseAngina`: exercise-induced angina [Y: Yes, N: No]
  10. `Oldpeak`: oldpeak = ST [Numeric value measured in depression]
  11. `ST_Slope`: the slope of the peak exercise ST segment [Up: upsloping, Flat: flat, Down: downsloping]
  12. `HeartDisease`: output class [1: heart disease, 0: Normal]
 
___


## Project structure

- **Data cleaning:** checking for NaN Value, missing data
- **Data Visualization:** constructing plots, charts to weigh the relations between each variables
- **Modeling:** The dataset is split into training and test sets using an 80-20 ratio. This ensures the model can be trained on the majority of the data while reserving a separate subset for evaluating generalization performance. The random state of 42 ensures reproducibility of the results.

___

## Result




