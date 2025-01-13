# Diabetes Classification Project

This project focuses on predicting diabetes in individuals using machine learning models. The task was conducted as part of the **Data Science and Artificial Intelligence (DSAI)** course at **HTL Wiener Neustadt**. The objective was to build and evaluate neural networks for classification, applying different methods to achieve high accuracy and reliable results.

## Task Description
The task required applying neural networks to a classification project from the 4th year using the following steps:
1. **Team Members**: Collaborate as a team to implement the project.
2. **Classification Using Scikit-learn**: 
   - Utilize the `MLPClassifier` and tune hyperparameters with `GridSearchCV`.
   - Visualize learning curves: average loss and accuracy during training and validation across epochs.
3. **Classification Using Keras**:
   - Build and optimize a neural network using Keras with `KerasTuner` and Hyperband.
   - Visualize learning curves for training and validation. Optionally, include TensorBoard visualizations.
4. **Comparison of Models**:
   - Create a comparison table for the new solutions, including models from the 4th year, with metrics such as accuracy, training time, and application time.
   - Discuss and document results thoroughly.
5. Submit a **Jupyter Notebook** and **PDF** as a ZIP file, with necessary input data linked via OneDrive.

## Dataset
The dataset was sourced from Kaggle and includes the following features:
- **Gender**: Biological sex of the individual.
- **Age**: Age of the individual (0-80).
- **Hypertension**: Indicates whether the individual has elevated blood pressure (0 or 1).
- **Heart Disease**: Indicates whether the individual has heart disease (0 or 1).
- **Smoking History**: Categorical values such as "never," "current," "former," etc.
- **BMI**: Body Mass Index indicating weight category.
- **HbA1c Level**: Average blood sugar level over the past 2-3 months.
- **Blood Glucose Level**: Glucose level in the blood at a given time.
- **Diabetes**: Target variable (0 = no diabetes, 1 = diabetes).

## Methodology
### 1. Data Preprocessing
- **Handling Missing Data**: Dropped the `smoking_history` column due to a high proportion of missing values.
- **Encoding**: Converted non-numeric columns like `gender` to numerical features using OneHotEncoding.
- **Scaling**: Normalized numerical columns with StandardScaler for better model performance.

### 2. Models
#### Scikit-learn MLPClassifier
- Used `MLPClassifier` from Scikit-learn with GridSearchCV for hyperparameter tuning.
- Optimized parameters such as hidden layer sizes, activation functions, and learning rates.
- Visualized loss and accuracy curves for both training and validation phases.

#### TensorFlow Keras Model
- Built a neural network using TensorFlow/Keras, tuned with `KerasTuner`'s Hyperband.
- Experimented with different architectures (e.g., 2-3 hidden layers) and learning rates.
- Visualized loss and accuracy curves for both training and validation phases.

### 3. Model Comparison
Both models achieved **high accuracy of 97%**, demonstrating reliable performance. Metrics such as precision, F1-Score, and MCC were also evaluated, highlighting the robustness of the models. A comparison table was created to summarize the results, including metrics from previous implementations in the 4th year.

## Technologies Used
- **Python**: Core programming language.
- **Pandas**: Data manipulation and preprocessing.
- **Scikit-learn**: MLPClassifier implementation and GridSearchCV for hyperparameter tuning.
- **TensorFlow/Keras**: Custom neural network construction and optimization with KerasTuner.
- **Matplotlib & Seaborn**: Data visualization tools.

## How to Run
1. Clone the repository.
2. Install dependencies using:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Jupyter Notebook or Python script to preprocess the data, train models, and evaluate results.

## Results

* **Scikit-learn MLPClassifier**: Achieved 97% accuracy with hyperparameter tuning.
* **TensorFlow Keras Model**: Achieved 97% accuracy with optimized architecture and parameters.
* **Both models demonstrated strong performance**, with highly consistent results across metrics.

## Submission

The project includes:
* A complete Jupyter Notebook documenting all steps, from preprocessing to evaluation.
* A PDF and HTML version of the notebook for easier review.
* Necessary input data provided via an accessible OneDrive link.

## Conclusion

This project successfully demonstrates the application of neural networks for diabetes classification. The models achieved high accuracy and performed robustly across various metrics, showcasing the potential of machine learning in healthcare applications.
