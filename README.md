# Building a Logistic Regression - KNN

#### Additionally
- _Optimize the Logistic Regression model with GridSearch_

- _Implement a K-Nearest Neighbor_ model

---

## Introduction
The goal of this project is to to forecast the nature of tumors, categorizing them as **benign (0)** or **malignant (1)** by analyzing various cellular characteristics, including radius, texture, and smoothness. Similar to many datasets encountered in practical applications, the distribution of outcomes is imbalanced, with benign diagnoses occurring more frequently than malignant ones. Additionally, there exists a significant bias regarding the significance of these outcomes, as accurately identifying all malignant cases is critically important. 

This examination will allow classifying patients as having or not having cancer.

This project will scope, analyze, prepare, plot data, and seek to explain the findings from the analysis.

Here are a couple of questions that this project seeks to answer:

- What was the strongest indicator of cancer diagnosis? 
- How many patients were deemed to have cancer?      
- What factor contributes least to the diagnosis of least cancer?
- Which model performs the best and why it performs the best? 



### Scenario
You are employed in the Medical department at a state college, where an upcoming lecture will delve into epidemiology and the analysis of breast cancer. The department aims to educate students about the various factors that may contribute to developing cancer. Rather than simply delivering a traditional lecture and expecting students to absorb the information passively, you intend to encourage them to draw their own conclusions and validate those insights through practical engagement. To achieve this, you plan to develop a machine learning model that will facilitate this exploration. Utilizing a real-world dataset containing diverse statistics about cancer patients, the model will classify whether each individual has cancer. Your goal is for students to input their own data to see their hypothetical outcomes. This interactive approach is designed to enhance the lecture's relevance and provide an enjoyable academic experience. While you aim to improve the user interface of the machine learning model in the future, your immediate focus is on establishing the foundational code.

**Data Sources:**

- [Wisconsin Breast Cancer Dataset](https://scikit-learn.org/dev/modules/generated/sklearn.datasets.load_breast_cancer.html)
- [UCI ML Breast Cancer Wisconsin](https://archive.ics.uci.edu/dataset/17/breast+cancer+wisconsin+diagnostic)
  

## Project Goals
The objective is to forecast breast cancer and educate students about the various factors that may contribute to the onset of the disease. Instead of merely presenting a conventional lecture and anticipating that students will passively receive the information, the intention is to motivate them to formulate their own conclusions and substantiate those understandings through active participation. 

Several questions will be asked:

- What was the strongest indicator of cancer diagnosis?
- How many patients were deemed to have cancer?
- What was the strongest correlation to radius_mean?
- What factor contributes least to the diagnosis of breast cancer? 



#### Why use a logistic regression algorithm to predict the outcome?
Logistic regression proves to be highly effective in classifying data, which aligns well with the objectives of this project. A data example is something, and simultaneously is not something else. This form of regression produces an output that represents a classification probability ranging from 0 to 1. Logistic regression is therefore appropriate for addressing classification issues in situations where traditional linear regression is inadequate. This project will also optimize the logistic regression using GridSearch and implement K Nearest Neighbor.


## Data
An anonymized dataset that can be used to train the machine-learning model has been found. It is a CSV file containing 569 medical records. 


## Conclusions

- What was the strongest indicator of cancer diagnosis?
    - **concave_points_worst**
- What were the subsequent two strongest indicators of cancer diagnosis, ranked by their level of impact?
    - **perimeter_mean, radius_mean**
- What was the strongest correlation to radius_mean?
    - **area_mean**
- What factor contributes least to the diagnosis of breast cancer?
    - **fractal_dimension_mean**
- What was the most effective logistic regression model for diagnosing cancer.
    - **stratified sampling model**
- Which confusion matrix threshold was most accurate
    -**Threshold**: 75% 
    - How many patients did it accurately predict?
    - **Patients Predicted**: 163 
    - How many patients were deemed to have cancer?
        - **Diagnosed Cancer**: 55
- Which model performs the best and why it performs the best?
  - The **KNN classification model consistently underperformed** compared to the logistic regression model **across all evaluated metrics**.
  - The **k-nearest neighbor model achieved a score of 92%**, which is slightly **inferior to the performance of the logistic regression model at 94%**; therefore, the logistic regression model will be prioritized for further evaluation and tuning.
  - The performance of **optimized model is inferior** to that of non-optimized logistic regression model. There is a **decline in True Positives** and a **rise in False Negatives**. This outcome is certainly counterproductive, despite the small numerical difference, as the objective is to minimize the misclassification of malignant cells as benign.