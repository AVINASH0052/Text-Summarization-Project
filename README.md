# Text Summarization Project

## Project Overview

This project focuses on developing a text summarization model using a state-of-the-art NLP technique. The model aims to condense long articles into shorter summaries, retaining the key information. This is particularly useful for quickly understanding large volumes of text data.

## Datasets

Three datasets are used in this project:

1. **news_data.csv**: Contains the main content of the articles.
2. **rating.csv**: Includes user ratings for various articles.
3. **raw-data.csv**: Contains raw text data of articles.

Each dataset is preprocessed to remove duplicates and irrelevant columns, and then combined into a single DataFrame for analysis and modeling.

## Project Workflow

### 1. Data Loading

Load the datasets using Pandas and inspect the first few rows to understand the structure and content.

### 2. Data Preprocessing

- **Type Conversion**: Convert the `article_id` column to string type for consistency.
- **Duplicate Removal**: Drop any duplicate rows based on `article_id`.
- **Concatenation**: Merge the datasets on `article_id` and remove duplicate columns.
- **Column Exclusion**: Drop irrelevant columns such as `source_id`, `source_name`, `author`, etc.
- **Handling Missing Values**: Remove any rows or columns with missing values to ensure clean data.

### 3. Text Cleaning and Tokenization

- **Text Cleaning**: Remove HTML tags and non-alphabetic characters, and convert text to lowercase.
- **Tokenization**: Split text into sentences and words.
- **Stopwords Removal**: Remove common English stopwords to reduce noise in the data.

### 4. Model Training

Use a pre-trained BART model for text summarization. The model and tokenizer are loaded using the Hugging Face `transformers` library.

- **Dataset Preparation**: Split the data into training and validation sets.
- **Model Training**: Train the model using a customized dataset class and appropriate training arguments.
- **Evaluation**: Evaluate the model's performance using the validation set.

### 5. Prediction and Visualization

- **Prediction**: Generate summaries for a sample of articles using the trained model.
- **Visualization**: Compare the length of predicted and actual summaries using bar plots.
- **Sample Output**: Display the original articles, predicted summaries, and actual summaries for comparison.

## Instructions to Reproduce the Results

### Prerequisites

Ensure you have the following installed:
- Python 3.6 or higher
- Jupyter Notebook
- Necessary Python libraries (listed below)

### Installation

1. **Clone the Repository**
   ```bash
   git clone <repository_url>
   cd <repository_directory>
