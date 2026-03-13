Here is a **clean README.md** you can use for your project (for GitHub or submission).

---

# Diabetes Progression Prediction using Artificial Neural Network (ANN)

## Project Overview

This project focuses on predicting **diabetes disease progression** using the Diabetes dataset from the **scikit-learn library**. An **Artificial Neural Network (ANN)** model was developed to learn patterns from medical features and predict the progression of the disease.

The project includes **data exploration, visualization, model development, evaluation, and model improvement** through experimentation with different neural network architectures and hyperparameters.

---

## Dataset

The dataset used in this project is the **Diabetes dataset from scikit-learn**.

**Dataset characteristics:**

* **Number of samples:** 442
* **Number of features:** 10
* **Target:** A quantitative measure of diabetes disease progression after one year

**Features include:**

* age
* sex
* bmi (Body Mass Index)
* bp (blood pressure)
* s1, s2, s3, s4, s5, s6 (various blood serum measurements)

---

## Project Workflow

### 1. Data Loading and Preprocessing

* Loaded the diabetes dataset using `sklearn.datasets`
* Converted the dataset into a Pandas DataFrame
* Performed exploratory data analysis

### 2. Data Visualization

Several visualizations were created to understand relationships between variables:

* Scatter plots (e.g., BMI vs target)
* Feature distribution plots
* Correlation heatmap
* Feature-target relationship analysis

### 3. Model Development

A baseline **Artificial Neural Network (ANN)** model was built using TensorFlow/Keras.

**Baseline Architecture**

* Dense layer (16 neurons, ReLU)
* Dropout layer (0.2)
* Dense layer (8 neurons, ReLU)
* Dropout layer (0.2)
* Output layer (1 neuron, Linear)

---

### 4. Model Evaluation

The model was evaluated using:

* **Mean Squared Error (MSE)**
* **R² Score**

Baseline performance:

* **MSE:** 0.488
* **R² Score:** 0.453

---

### 5. Model Improvement

Several improvements were tested:

* Increased number of neurons
* Different activation functions
* Increased training epochs
* Use of dropout to prevent overfitting

**Improved Architecture**

* Dense layer (32 neurons, ReLU)
* Dropout layer (0.2)
* Dense layer (16 neurons, ReLU)
* Dropout layer (0.2)
* Output layer (1 neuron, Linear)

Improved model performance:

* **MSE:** 0.443
* **R² Score:** 0.504

The improved model shows better predictive performance compared to the baseline model.

---

## Visualization of Results

An **Actual vs Predicted Values plot** was generated to visually compare model predictions with true target values. The scatter points close to the diagonal line indicate good predictive performance.

---

## Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn
* TensorFlow / Keras

---

## Conclusion

The Artificial Neural Network model successfully learned patterns in the diabetes dataset and achieved reasonable predictive performance. After experimenting with different architectures and training parameters, the improved model achieved an **R² score of approximately 0.50**, demonstrating better prediction accuracy.

---
