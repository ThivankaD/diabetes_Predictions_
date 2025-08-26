# Diabetes Prediction Model

This repository contains a machine learning model to predict the onset of diabetes based on diagnostic measurements. The model is built using TensorFlow and utilizes a dataset of Pima Indian women.

## Dataset

The dataset used in this project is the Pima Indians Diabetes Database, originally from the National Institute of Diabetes and Digestive and Kidney Diseases. The dataset contains the following columns:

*   `Pregnancies`: Number of times pregnant
*   `Glucose`: Plasma glucose concentration a 2 hours in an oral glucose tolerance test
*   `BloodPressure`: Diastolic blood pressure (mm Hg)
*   `SkinThickness`: Triceps skin fold thickness (mm)
*   `Insulin`: 2-Hour serum insulin (mu U/ml)
*   `BMI`: Body mass index (weight in kg/(height in m)^2)
*   `DiabetesPedigreeFunction`: Diabetes pedigree function
*   `Age`: Age (years)
*   `Outcome`: Class variable (0 or 1)

## Project Structure

The notebook performs the following steps:

1.  **Data Loading and Exploration:** Loads the dataset and displays basic information and visualizations of the features.
2.  **Data Preprocessing:**
    *   Separates features (X) and target (y).
    *   Scales the features using `StandardScaler`.
    *   Addresses class imbalance using `RandomOverSampler`.
3.  **Model Building:** Creates a sequential TensorFlow model with dense layers and ReLU activation, and a sigmoid activation for the output layer.
4.  **Model Compilation:** Configures the model with the Adam optimizer, Binary Crossentropy loss, and accuracy as the metric.
5.  **Model Training:** Trains the model on the training data and validates it on the validation data.
6.  **Model Evaluation:** Evaluates the trained model on the test data.

## Getting Started

To run this notebook, you will need to have Python installed along with the following libraries:

*   pandas
*   numpy
*   matplotlib
*   sklearn
*   imblearn
*   tensorflow

You can install these libraries using pip:

```bash
pip install pandas numpy matplotlib scikit-learn imblearn tensorflow
