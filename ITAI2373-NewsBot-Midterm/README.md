# NewsBot Intelligence System

**ITAI 2373 - Midterm Project**
**Student:** Star Yarbrough
**Instructor:** Professor Ganti

## Project Overview

NewsBot Intelligence System is a Natural Language Processing (NLP) project designed to analyze, classify, and extract useful information from news articles. The system integrates text preprocessing, TF-IDF feature extraction, part-of-speech tagging, syntactic analysis, sentiment analysis, named entity recognition, and machine learning classification.

The project demonstrates how multiple NLP techniques can work together to transform unstructured news articles into organized, actionable information.

## Dataset

The project uses the BBC News Train dataset, containing articles across five categories:

- Business
- Entertainment
- Politics
- Sports
- Technology

The original dataset contained 1,490 articles. After removing 50 duplicate articles, 1,440 unique articles remained for analysis.

## Technologies Used

- Python and Google Colab
- Pandas and NumPy
- NLTK and spaCy
- Scikit-learn
- Matplotlib and Seaborn
- TF-IDF Vectorization
- VADER Sentiment Analysis

## System Features

**Text Preprocessing:** Cleans articles, removes unnecessary characters and stopwords, and performs tokenization and lemmatization.

**Text Representation:** Uses TF-IDF to transform article text into numerical features for machine learning.

**Linguistic Analysis:** Examines grammatical patterns, part-of-speech distributions, and syntactic structures.

**News Classification:** Trains and compares Naive Bayes, Logistic Regression, and Support Vector Machine classifiers.

**Sentiment Analysis:** Evaluates positive, negative, and neutral sentiment in news articles.

**Named Entity Recognition:** Identifies people, organizations, locations, dates, and other important entities.

**NewsBot Integration:** Combines classification, sentiment analysis, and entity extraction into one article-processing system.

## Results

| Model                  | Test Accuracy |
| ---------------------- | ------------- |
| Naive Bayes            | 94.79%        |
| Logistic Regression    | 95.49%        |
| Support Vector Machine | 94.79%        |

Naive Bayes was selected for the integrated NewsBot because it achieved the highest cross-validation accuracy, approximately 96.79%.

The system also extracted 40,803 named-entity mentions across the dataset.

## Limitations

The system performs well on the BBC dataset but has limitations. Articles covering multiple subjects may receive lower classification confidence. Sentiment analysis can misinterpret complex language, and named entity recognition may occasionally identify incorrect entity boundaries.

The dataset also does not provide publication dates, limiting time-based analysis.

## Running the Project

1. Open the Jupyter notebook in Google Colab.
2. Upload `BBC News Train.csv` to the Colab Files sidebar.
3. Install the required Python libraries and NLP resources using the notebook's setup cells.
4. Run the notebook cells in order.
5. Review the generated analyses, visualizations, model evaluations, and NewsBot test results.

## Individual Contributions

This project was completed individually. My work included preparing the dataset, implementing and integrating the NLP components, evaluating machine learning models, examining the results, and testing the completed NewsBot system.

## Future Improvements

Future development could include newer news datasets, more advanced language models, improved sentiment detection, enhanced entity recognition, and a user-friendly interface for analyzing articles.

## Project Purpose

This project was completed as part of ITAI 2373 to demonstrate practical NLP techniques and their potential applications in real-world artificial intelligence systems.
