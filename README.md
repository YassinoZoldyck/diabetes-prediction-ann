# Diabetes Classification Project

This project focuses on predicting diabetes in individuals using machine learning models. The dataset used includes medical and demographic information, such as age, BMI, hypertension status, and blood glucose levels, to classify patients as diabetic or non-diabetic.

## Dataset
The dataset was sourced from Kaggle and contains the following features:
- **Gender**: Biological sex of the individual.
- **Age**: Age of the individual (0-80).
- **Hypertension**: Indicates whether the individual has elevated blood pressure (0 or 1).
- **Heart Disease**: Indicates whether the individual has heart disease (0 or 1).
- **Smoking History**: Categorized as "never," "current," "former," etc.
- **BMI**: Body Mass Index, indicating the individual's weight category.
- **HbA1c Level**: Average blood sugar level over the past 2-3 months.
- **Blood Glucose Level**: Glucose level in the blood at a given time.
- **Diabetes**: Target variable (0 = no diabetes, 1 = diabetes).

## Methodology
### 1. Data Preprocessing
- **Handling Missing Data**: The `smoking_history` column, with many "No Info" values, was dropped.
- **Encoding**: Non-numeric columns like `gender` were one-hot encoded.
- **Scaling**: Numerical columns were scaled using StandardScaler to ensure normalized inputs.

### 2. Models Used
Two models were developed for this project:
1. **Scikit-learn MLPClassifier**: A neural network model with optimized hyperparameters using GridSearchCV.
2. **TensorFlow Keras Model**: A custom neural network built and tuned using KerasTuner's Hyperband method.

### 3. Model Performance
Both models achieved **high accuracy of 97%**, demonstrating strong performance in classifying diabetic and non-diabetic cases. Additionally, metrics like precision and F1-score further validated the reliability of the models.

### 4. Visualizations
The project includes:
- Loss and accuracy curves for both training and validation phases.
- A bar chart comparing performance metrics (Accuracy, Precision, F1-Score, and MCC) between the two models.

## Technologies Used
- **Python**: Core programming language.
- **Pandas**: For data manipulation and preprocessing.
- **Scikit-learn**: For building and tuning the MLPClassifier.
- **TensorFlow/Keras**: For constructing and optimizing the Keras model.
- **Matplotlib & Seaborn**: For data visualization.
