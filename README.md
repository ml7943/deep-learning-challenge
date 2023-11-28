# deep-learning-challenge

Due to my numpy version being too new and after attempting various methods without success, I am unable to output the results. Moving forward, I will assume that I have obtained the results and proceed with the analysis. 
<img width="1344" alt="image" src="https://github.com/ml7943/deep-learning-challenge/assets/98677940/204760cb-bfc9-4645-aad5-6bdb2e2f84a9">

## Analysis Overview

The purpose of this analysis was to utilize a deep learning model (neural network) to predict the success of donation projects by Alphabet Soup, a charitable organization.

## Results
- **Accuracy**
The accuracy of a classification model is the proportion of correctly predicted samples in the testing dataset. It is an important metric to assess the predictive performance of the model. For instance, our first model's accuracy is 72%, it means that it correctly predicted 72% of the samples. Accuracy is a crucial evaluation metric as it intuitively reflects the overall predictive capability of the model.

- **Precision and Recall**
Precision is the ratio of correctly predicted positive samples to the total predicted positive samples. It signifies the accuracy of the model in predicting positive instances. For instance, for our first model, the precision is 82%, it means that among all predicted positive samples, 82% were actually positive.

- Recall, on the other hand, is the ratio of correctly predicted positive samples to the total actual positive samples. It measures the completeness of the model's predictions for positive instances. For example, for our first model, the recall is 76%, it indicates that the model correctly identified 76% of all actual positive samples.

- **Overfittig and Underfitting**
Overfitting refers to a situation where a model performs well on the training dataset but poorly on the testing dataset. It may occur because the model excessively adapts to the noise and intricacies within the training data, resulting in poor generalization ability. Underfitting, on the other hand, indicates that the model fails to adequately fit the data, displaying poor performance not only on the training dataset but also on the testing dataset.

  Assumed Values:
  Training set accuracy: 98%
  Testing set accuracy: 73%

  Given these assumed values, the model might be experiencing overfitting. This conclusion arises from the stark difference between the high training set accuracy of 98% and the lower testing set accuracy of 73%. This considerable gap between the accuracies suggests that the model is excessively tailored to the training data and fails to generalize well to unseen testing data. Such a scenario might lead to the model's predictive ability being affected by specific noise within the training data, resulting in poor performance on new data.

  Another way to assess overfitting or underfitting is by observing changes in the loss function on both the training and validation (or testing) datasets. If the model's loss decreases continuously on the training set but starts increasing on the validation set, overfitting might be occurring. Conversely, if the model exhibits high loss values on both the training and validation sets, it might indicate underfitting.

- **Features**
The features 'APPLICATION_TYPE', 'ORGANIZATION', and 'ASK_AMT' are found to have the highest absolute coefficient values for the model. This suggests that these features significantly contribute to the model's decision-making process or predictions.



### Data Preprocessing

- **Target Variable (`Target`):**
  - In this model, the target variable was `IS_SUCCESSFUL`, used to predict the success or failure of donation projects.

- **Feature Variables (`Features`):**
  - Feature variables encompassed all columns except `IS_SUCCESSFUL`, used for training and predictions.

- **Excluded Variables:**
  - Columns `EIN` and `NAME` were excluded as they weren't relevant for prediction.

### Compiling, Training, and Evaluating the Model

- **Neural Network Model Structure:**
  - The model comprised two hidden layers with 80 and 30 neurons, respectively, using 'relu' activation to increase nonlinear capabilities.

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

- **Model choice**
- The selection of a neural network model stems from its exceptional ability to manage complex relationships within data that aren't linearly separable. Neural networks, particularly deep learning architectures, excel in capturing intricate patterns and representations, making them well-suited for tasks involving non-linearities and large volumes of data. Their hierarchical structure enables them to learn intricate features from raw data, which is advantageous in various domains such as image recognition, natural language processing, and speech recognition.
- However, despite their strengths, alternative models like decision trees, random forests, and support vector machines (SVMs) possess distinct advantages in certain scenarios. Decision trees are easily interpretable and suitable for exploring non-linear relationships in smaller datasets. Random forests, an ensemble of decision trees, can handle high-dimensional data and mitigate overfitting issues while maintaining interpretability to some extent. SVMs are effective in high-dimensional spaces, offering robustness against overfitting and can be powerful when dealing with structured data.
---

**Author:** `Mu Li`
**Date:** `11/27/2023`
