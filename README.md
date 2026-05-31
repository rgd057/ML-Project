Ml diabets predection project
The prediction is based on medical information such as:

- Glucose level
- Blood pressure
- BMI
- Insulin level
- Age
- Number of pregnancies

The target column is called **Outcome**:

- `0` means the person does not have diabetes
- `1` means the person has diabetes

---

## Dataset

The dataset used in this project is:

```text
diabetes (2).csv
```

The dataset has **768 rows** and **9 columns**.

The columns are:

| Column | Meaning |
|---|---|
| Pregnancies | Number of pregnancies |
| Glucose | Glucose level |
| BloodPressure | Blood pressure |
| SkinThickness | Skin thickness |
| Insulin | Insulin level |
| BMI | Body Mass Index |
| DiabetesPedigreeFunction | Family history of diabetes |
| Age | Age of the person |
| Outcome | Diabetes result: 0 or 1 |

---

## What the Project Does

The project goes through these steps:

1. Load the diabetes dataset.
2. Explore the data.
3. Check for missing values and zero values.
4. Split the data into training and testing sets.
5. Scale the features using StandardScaler.
6. Train different machine learning models.
7. Evaluate the models.
8. Compare the results.
9. Choose the best model.

---

## Models Used

Three machine learning models were used:

1. **Decision Tree**
2. **Support Vector Machine (SVM)**
3. **Random Forest**

---

## Model Results

| Model | Accuracy |
|---|---:|
| SVM | 75.97% |
| Decision Tree | 74.68% |
| Random Forest | 72.08% |

After tuning the models, the results were:

| Model | Tuned Accuracy |
|---|---:|
| Decision Tree | 75.97% |
| Random Forest | 74.03% |
| SVM | 73.38% |

---

## Best Model

The best model after tuning was:

```text
Decision Tree
```

It achieved an accuracy of:

```text
75.97%
```

---

## Important Features

The most important features for predicting diabetes were:

1. Glucose
2. BMI
3. Age

This means these features had the strongest effect on the prediction.

---

## Evaluation Methods

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix
- ROC Curve

These metrics help us understand how well each model predicts diabetes.

---

## How to Run the Project

First, install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

Then follow these steps:

1. Open the notebook file:

```text
ml_project.ipynb
```

2. Make sure the dataset file is in the same folder:

```text
diabetes (2).csv
```

3. Run the notebook cells from top to bottom.

---

## Files

| File | Description |
|---|---|
| `ml_project.ipynb` | The main notebook with the code |
| `diabetes (2).csv` | The dataset |
| `README.md` | Project explanation |

---

## Conclusion

This project compares three machine learning models for diabetes prediction.

The models were trained and tested using the diabetes dataset.

The best model was the **Decision Tree**, with an accuracy of **75.97%**.

Glucose, BMI, and Age were the most important features in predicting diabetes.

---

## Future Improvements

In the future, the project can be improved by:

- Trying more machine learning models
- Cleaning zero values more carefully
- Using a larger dataset
- Improving feature selection
- Creating a simple web app for the model
