# deep-learning-challenge

## Analysis Overview

The purpose of this analysis was to utilize a deep learning model (neural network) to predict the success of donation projects by Alphabet Soup, a charitable organization.

## Results

### Data Preprocessing

- **Target Variable (`Target`):**
  - In this model, the target variable was `IS_SUCCESSFUL`, used to predict the success or failure of donation projects.

- **Feature Variables (`Features`):**
  - Feature variables encompassed all columns except `IS_SUCCESSFUL`, used for training and predictions.

- **Excluded Variables:**
  - Columns `EIN` and `NAME` were excluded as they weren't relevant for prediction.

### Compiling, Training, and Evaluating the Model

- **Neural Network Model Structure:**
  - The model comprised two hidden layers with 100 and 50 neurons, respectively, using 'relu' activation to increase nonlinear capabilities. Additionally, a third hidden layer with 40 neurons was added.

- **Achievement of Target Model Performance:**
  - Different neural network structures and optimizers were experimented with during the model optimization process to enhance performance.

- **Steps to Improve Model Performance:**
  - Adjustments were made to the number of neurons and hidden layers, experimenting with various activation functions, optimizers, and increasing the number of training epochs to enhance model performance.

### Summary

The deep learning model exhibited a reasonable predictive capability, yet there is room for improvement to meet the target performance. Potential avenues for enhancement include:

- **Model Structural Changes:**
  - Experimenting with deeper or wider model structures may better capture complex patterns within the data.

- **Feature Engineering Optimization:**
  - Further analyzing and selectively adding, removing, or transforming features could enhance model performance.

- **Exploring Different Model Types:**
  - Trying alternative machine learning models (e.g., random forests, gradient boosting) may yield different results and potentially better performance for this classification problem.

---

**Author:** `Mu Li`

**Date:** `11/27/2023`
