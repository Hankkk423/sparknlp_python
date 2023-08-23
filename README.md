# Spark NLP: Tweet Classification | Named Entity Recognition with BERT

This repository contains two distinct projects that leverage the power of Spark NLP to perform tweet classification and named entity recognition (NER) using BERT embeddings. Spark NLP is a powerful library that enables natural language processing tasks at scale within the Apache Spark framework. The two projects are outlined below:


## Project 1: Tweet Classification
In the first project, we employ Spark NLP to tackle the task of tweet classification. We utilize a dataset of tweets containing text data and corresponding target labels indicating whether a tweet is related to a real disaster (target=1) or not (target=0). The project is structured as follows:

### Data Loading and Preprocessing
- We use the Spark framework to load and preprocess the tweet dataset from CSV format. (Link: https://www.kaggle.com/datasets/vstepanenko/disaster-tweets)
- Data is split into training and testing sets, ensuring robust model evaluation.

### Text Classification Model
- We construct a pipeline that includes a DocumentAssembler, Universal Sentence Encoder, and ClassifierDLApproach stages.
- The pipeline processes text data, extracts sentence embeddings, and trains a text classification model to predict tweet labels.

### Model Training and Evaluation
- The pipeline is fit to the training data, and the trained model is evaluated using the testing data.
- We compute various metrics like accuracy, precision, recall, and F1-score to assess the model's performance.

### Result Analysis
- The project showcases how Spark NLP enables efficient text classification, even on large-scale datasets.
- Model insights and performance metrics are provided to gain a comprehensive understanding of the classification task.


## Project 2: Named Entity Recognition with BERT
The second project focuses on named entity recognition (NER) using BERT embeddings within the Spark NLP framework. NER involves identifying entities like names, dates, and organizations within text. Here's an overview:

### Data and BERT Embeddings
- We work with text data and leverage the BERT word embeddings provided by Spark NLP.
- These embeddings capture rich semantic information, making them ideal for NER tasks.

### NER Model Setup
- The pipeline is structured with stages such as DocumentAssembler, Tokenizer, BertEmbeddings, NerDLModel, and NerConverter.
- Each stage contributes to the NER pipeline, from tokenization to prediction and conversion.

### Named Entity Recognition
- The pipeline processes text to identify entities like persons, locations, dates, and more.
- The NER predictions are presented both in token-level format and in more understandable chunks.

### Insights and Applications
- The second project demonstrates how Spark NLP, coupled with BERT embeddings, can accurately extract named entities from text.
- The resulting NER chunks provide a human-readable representation of entities, facilitating information extraction.



## Installation

Both notebooks are working on Google Colab.

## Usage

1. Clone this repository to your local machine.
2. Upload notebooks to Google Colab and run it.

## Contributing

Contributions to this project are welcome! If you'd like to contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and test thoroughly.
4. Commit your changes and push them to your fork.
5. Create a pull request to the original repository.

## License

This project is licensed under the MIT License. You can find more details in the LICENSE file.
