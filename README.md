# Text Summarization Project

This project demonstrates the development of a text summarization model using the BART (Bidirectional and Auto-Regressive Transformers) architecture. The project involves data loading, preprocessing, training a model, and generating summaries for given texts.

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Methodology](#methodology)
- [Results](#results)
- [Requirements](#requirements)
- [Usage](#usage)
- [Conclusion](#conclusion)
- [Future Work](#future-work)
- [Acknowledgments](#acknowledgments)

## Introduction
Text summarization is a critical application of natural language processing (NLP) that aims to condense long documents into shorter versions while retaining the essential information. This project utilizes the BART model for generating summaries of news articles.

## Dataset
Three datasets are used in this project:
1. **data.csv**: Contains preprocessed news articles.
2. **rating.csv**: Contains user ratings for the articles.
3. **raw-data.csv**: Contains raw news articles before preprocessing.

These datasets are combined and preprocessed to create a final dataset for training and evaluation.

## Methodology
The project follows these main steps:
1. **Data Loading**: Loading the datasets into Pandas DataFrames.
2. **Data Preprocessing**: Cleaning the text, tokenization, and removing duplicates.
3. **Model Training**: Training the BART model using the prepared dataset.
4. **Prediction**: Generating summaries for new texts using the trained model.
5. **Evaluation**: Comparing the predicted summaries with the actual summaries.

## Results
The model's performance is evaluated by generating summaries for a sample of articles and comparing them with the actual summaries. Visualizations are created to show the length of predicted and actual summaries for comparison.

## Requirements
To run this project, you need to install the following libraries:
- pandas
- requests
- beautifulsoup4
- nltk
- torch
- transformers
- scikit-learn
- matplotlib

You can install these dependencies using pip:

## Usage
1. **Clone the Repository**:
   git clone https://github.com/AVINASH0052/Text-Summarization-Project.git

2. **Navigate to the Project Directory**:
   cd Text-Summarization-Project

3. **Run the Jupyter Notebook**:
   - Open the Jupyter Notebook `summarization.ipynb` and execute the cells to reproduce the results.
   - Follow the steps outlined in the notebook to train the model and generate summaries.

## Conclusion
This project successfully demonstrates the use of BART for text summarization, showcasing skills in data preprocessing, model training, and result visualization. The generated summaries provide a concise representation of the original texts.

## Future Work
Future improvements could include:
- Experimenting with different NLP models and architectures.
- Fine-tuning hyperparameters for better performance.
- Integrating additional features such as sentiment analysis.

## Acknowledgments
Special thanks to the creators of the datasets and the developers of the libraries used in this project.
