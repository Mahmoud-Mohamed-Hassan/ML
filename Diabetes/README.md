This project uses a Support Vector Machine (SVM) model to predict the likelihood of diabetes in patients based on various medical features.

## Dataset

The dataset used for this project is the Pima Indians Diabetes Database, which contains information about female patients of Pima Indian heritage.

## Features

The dataset includes the following features:

* **Pregnancies:** Number of times pregnant
* **Glucose:** Plasma glucose concentration
* **BloodPressure:** Diastolic blood pressure (mm Hg)
* **SkinThickness:** Triceps skin fold thickness (mm)
* **Insulin:** 2-Hour serum insulin (mu U/ml)
* **BMI:** Body mass index (weight in kg / (height in m)^2)
* **DiabetesPedigreeFunction:** Diabetes pedigree function
* **Age:** Age (years)
* **Outcome:** Class variable (0 or 1) - 0 represents non-diabetic, and 1 represents diabetic.

## Methodology

1. **Data Loading and Exploration:** The dataset is loaded, and initial exploratory data analysis (EDA) is performed, including checking for missing values and summarizing the data.

2. **Data Preprocessing:**
    - The data is standardized using StandardScaler to ensure that all features have a similar range of values, which can improve the performance of the SVM model.
3. **Model Training:**
    - The data is split into training and testing sets using train_test_split.
    - An SVM model with a linear kernel is trained on the training data.

4. **Model Evaluation:**
    - The model's accuracy is evaluated on both the training and testing sets to assess its performance and identify potential overfitting.

5. **Prediction:**
   - The trained model is used to predict the outcome for a given input data instance.
## Usage

The code provided performs the following actions:

- Reads the diabetes dataset from a CSV file.
- Performs exploratory data analysis (EDA) on the dataset.
- Scales the data using StandardScaler
- Splits data into training and testing sets.
- Trains an SVM model.
- Evaluates the model's accuracy on training and testing sets.
- Takes user input for prediction.
- Predicts the outcome for the provided input.

## Requirements

- pandas
- numpy
- matplotlib
- scikit-learn
- seaborn
