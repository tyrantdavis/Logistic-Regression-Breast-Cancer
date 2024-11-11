# Building a Logistic Regression
## Introduction
The goal of this project is to to forecast the nature of tumors, categorizing them as benign (0) or malignant (1) by analyzing various cellular characteristics, including radius, texture, and smoothness. Similar to many datasets encountered in practical applications, the distribution of outcomes is imbalanced, with benign diagnoses occurring more frequently than malignant ones. Additionally, there exists a significant bias regarding the significance of these outcomes, as accurately identifying all malignant cases is critically important. 

This examination will allow classifying patients as having or not having cancer.

This project will scope, analyze, prepare, plot data, and seek to explain the findings from the analysis.

Here are a couple of questions that this project seeks to answer:

- What feature contributes most to the diagnosis of cancer?      
- What factor contributes least to the diagnosis of least cancer? 



### Scenario
You are employed in the Medical department at a state college, where an upcoming lecture will delve into epidemiology and the analysis of breast cancer. The department aims to educate students about the various factors that may contribute to developing cancer. Rather than simply delivering a traditional lecture and expecting students to absorb the information passively, you intend to encourage them to draw their own conclusions and validate those insights through practical engagement. To achieve this, you plan to develop a machine learning model that will facilitate this exploration. Utilizing a real-world dataset containing diverse statistics about cancer patients, the model will classify whether each individual has cancer. Your goal is for students to input their own data to see their hypothetical outcomes. This interactive approach is designed to enhance the lecture's relevance and provide an enjoyable academic experience. While you aim to improve the user interface of the machine learning model in the future, your immediate focus is on establishing the foundational code.

**Data Sources:**

- [Wisconsin Breast Cancer Dataset](https://scikit-learn.org/dev/modules/generated/sklearn.datasets.load_breast_cancer.html)
- [UCI ML Breast Cancer Wisconsin](https://archive.ics.uci.edu/dataset/17/breast+cancer+wisconsin+diagnostic)
  

## Project Goals
The objective is to forecast breast cancer and educate students about the various factors that may contribute to the onset of the disease. Instead of merely presenting a conventional lecture and anticipating that students will passively receive the information, the intention is to motivate them to formulate their own conclusions and substantiate those understandings through active participation. 

Several questions will be asked:

- What feature contributes most to the diagnosis of breast cancer?      
- What factor contributes least to the diagnosis of breast cancer? 



#### Why use a logistc regression algorithm to predict the outcome?
Logistic regression proves to be highly effective in classifying data, which aligns well with the objectives of this project. A data example is something, and simultaneously is not something else. This form of regression produces an output that represents a classification probability ranging from 0 to 1. Logistic regression is therefore appropriate for addressing classification issues in situations where traditional linear regression is inadequate.


## Data
An anonymized dataset that can be used to train the machine-learning model has been found. It is a CSV file containing 569 medical records. 


## Conclusions

TBD...

- What feature contributes most to the diagnosis of breast cancer?      
- What factor contributes least to the diagnosis of breast cancer? 