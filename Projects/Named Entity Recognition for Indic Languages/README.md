# Comparative Analysis of NER Models for Indic Languages

## Project Overview

This project evaluates and compares Named Entity Recognition (NER) models for Indic languages. The focus is on analyzing the performance of IndicBERT and IndicNER models, alongside querying NER results from ChatGPT. The evaluation metrics include precision, recall, and macro F1 scores, with results compared against manually annotated sentences.

## Repository Structure

The repository is organized as follows:

- **Results/**
  - **IndicBERT_for_NER/**: Contains results and performance metrics for the IndicBERT model.
  - **IndicNER_results/**: Contains results and performance metrics for the IndicNER model.
  - **IndicBERT/**: Contains outputs and metrics related to IndicBERT model testing.
  - **IndicNER/**: Contains outputs and metrics related to IndicNER model testing.

- **Notebooks/**
  - `Training_IndicNER.ipynb`: Notebook used to train the IndicNER model.
  - `Training_IndicBERT.ipynb`: Notebook used to train the IndicBERT model.
  - `Testing_IndicNER.ipynb`: Notebook used to test the IndicNER model.
  - `Testing_IndicBERT_for_NER.ipynb`: Notebook used to test the IndicBERT model.

## Dataset

The project uses the Naamapadam corpus for Named Entity Recognition in Indic languages. The dataset is divided into:
- **Training Set (70%)**: Used to fine-tune the models.
- **Validation Set (10%)**: Used to tune model parameters and avoid overfitting.
- **Test Set (20%)**: Used to evaluate the final model performance.

You can access the Naamapadam dataset at [Naamapadam Corpus on Hugging Face](https://huggingface.co/datasets/ai4bharat/naamapadam/tree/main/data).

## Instructions

1. **Explore Results**: Navigate to the `Results` folder to explore the performance metrics and outputs of the models.
   
2. **Run Models**: Use the Jupyter Notebooks in the `Notebooks` folder to train and test the models:
   - `Training_IndicNER.ipynb`: Train the IndicNER model.
   - `Training_IndicBERT.ipynb`: Train the IndicBERT model.
   - `Testing_IndicNER.ipynb`: Test the IndicNER model.
   - `Testing_IndicBERT_for_NER.ipynb`: Test the IndicBERT model.

3. **Evaluation**: Review the performance metrics in the `Results` folder to compare the models. The results include precision, recall, and macro F1 scores for each model.

## Evaluation Metrics

- **Precision**: Measures the accuracy of the model's predictions.
- **Recall**: Measures the model's ability to find all relevant instances.
- **Macro F1 Score**: The average F1 score across all classes, providing a balanced view of performance.



## Contact

For questions or comments, please contact at akashshiv23@iitk.ac.in
