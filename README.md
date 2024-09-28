# Summer-Research-Project 
### Project Name - Large Language Models for Clinical Note Analysis Across Medical Specialties

# Overview
This repository contains the work done during my summer research project at IIT Roorkee under the supervision of Prof. Aparajita Khan. The project focuses on classifying medical questions into one of 16 predefined categories using three models: BERT base uncased, GPT-2, and ClinicalBERT. We employed a medical question-answer dataset with a focus on building robust machine learning pipelines to explore different learning paradigms for the task of question classification.
# Dataset
The dataset used for this project is a medical question-answer-based dataset, where each question is assigned to one of 16 categories. The dataset was preprocessed to clean and organize the data for optimal model performance. Each row consists of:

* #### Question: The medical question posed.
* #### Answer: Corresponding medical answer.
* #### Question Type: The categorical label indicating the type of question (16 total categories).
# Project Structure
The project consists of three models, each implemented through three distinct pipelines:

* #### BERT base uncased
* #### GPT-2
* #### ClinicalBERT
Each model has three pipelines, which are described below:
## Pipelines
* ### Pipeline 1: Embedding Extraction + ANN Classification
  * In this pipeline, embeddings for the medical questions are extracted using the pre-trained models (BERT, GPT-2, ClinicalBERT). These embeddings are then fed into an Artificial Neural Network 
    (ANN) for classifying the questions into one of 16 categories.
* ### Pipeline 2: Zero-Shot Learning
  * The second pipeline applies zero-shot learning. Here, the pre-trained models directly classify the questions without any task-specific training. This allows the models to make predictions based     on their prior knowledge without additional labeled data.
* ### Pipeline 3: Few-Shot Learning
  * In this pipeline, only the final two layers of the models are fine-tuned on the dataset, using a few-shot learning approach. This allows the models to adapt to the specific task of question     
    classification without retraining the entire model.
# Evaluation Metrics
To assess the performance of the models and pipelines, we used various metrics, including:

* #### Accuracy
* #### Precision
* #### Recall
* #### F1-Score
In addition, a confusion matrix was generated for each pipeline to provide a visual representation of the classification results, allowing for a detailed comparison of model performance.
# Results
After comparing the results from all three pipelines for each model, we found significant insights into how these models perform across different learning paradigms, such as zero-shot, few-shot, and fine-tuning approaches.
# Acknowledgments
I would like to express my gratitude to Prof. Aparajita Khan, CSE Dept., IIT Roorkee, for her guidance and support throughout this project.
