# Heart attack prediction

A machine learning project to predict the likelihood of heart attacks using clinical data. Built for educational and research purposes, this project demonstrates the full ML pipeline: data cleaning, exploratory analysis, model training, validation, and explainability.

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

- **Data Cleaning**: Checked for nulls, outliers, and suspicious entries (e.g., Cholesterol = 0)
- **Visualization**: Histograms, boxplots, scatter plots, violin plots, countplots, and pair plots
- **Correlation Analysis**: Identified strong predictors (e.g., ExerciseAngina, Oldpeak, ST_Slope)
- **Model Evaluation**: Accuracy, confusion matrix, precision, recall, and F1-score Observed 100% accuracy — flagged and discussed as possible overfitting
- **Cross-validation**: Verified model consistency across folds
- **SHAP Explainability**: Visualized feature importance for clinical interpretability

___

## Models Used

- Logistic Regression (with and without class balancing)
- Neural Network (using TensorFlow/Keras)
- SMOTE (Synthetic Minority Over-sampling Technique)
- Polynomial feature engineering (interaction terms)
- Cross-validation (5-fold)
- GridSearchCV (Random Forest - on Iris for demonstration)
- SHAP (Explainable AI visualization for model interpretability)

___

## Result

| Model               | Accuracy | Precision | Recall | F-1 score |
|---------------------|----------|-----------|--------|-----------|
| Neural Network      | 95%      | 96%       | 95%    | 95%       |
| Logistic Regression | 95%      | 96%       | 95%    | 95%       |
| Logistic + SMOTE    | 95%      | 95%       | 95%    | 95%       |

___

## Getting Started

**1. Clone the Repository**

`git clone https://github.com/yourusername/heart-attack-prediction.git
cd heart-attack-prediction`

**2. Install Dependencies**

`pip install -r requirements.txt`

Or manually install the main libraries:
`pip install pandas matplotlib seaborn scikit-learn imbalanced-learn shap tensorflow`

**3. Run the Notebook**

Open `heart_attack_prediction.ipynb` in Jupyter or VSCode and run all cells.
___

## Acknowledgments

- Fedesoriano for dataset compilation
- scikit-learn, TensorFlow, and SHAP libraries
- Visualization inspired by Seaborn and Matplotlib
___

## License

MIT License. See LICENSE file for details.
___

## Contact

- Created by Suchada W.
- Email: suchadawongkot1@gmail.com
- GitHub: zin-w

Feel free to fork, raise issues, or submit pull requests!




