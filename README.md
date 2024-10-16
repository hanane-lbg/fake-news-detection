# Fake News Detection

## Project Overview
In today's digital age, the spread of misinformation through fake news is a growing problem, affecting public opinion and trust in legitimate news sources. This project tackles the challenge of fake news detection by leveraging deep learning sequence models, specifically Long Short-Term Memory (LSTM) networks and its variations. The goal is to develop a system capable of identifying fake news with high accuracy.

- Word Embeddings with Word2Vec
- LSTM, BiLSTM, GRU, BiGRU models
- Performance evaluation using accuracy, precision, recall, F1-score
- Visualization of training/validation metrics

## Dataset
The dataset used for this project was sourced from [Kaggle's Fake News Detection dataset](https://www.kaggle.com/datasets/jruvika/fake-news-detection). It consists of news articles with three main features:
- **URLs**: The web address of the articles.
- **Body**: The main content of the articles.
- **Headline**: The article headlines.


Data preprocessing involved combining the body and headline for input text, performing text cleaning, tokenization, and padding/truncating to prepare the data for deep learning models.

## Model Architecture
The project explores several deep learning architectures:
- **LSTM** (Long Short-Term Memory)
- **BiLSTM** (Bidirectional LSTM)
- **Stacked LSTM**
- **GRU** (Gated Recurrent Unit)
- **BiGRU** (Bidirectional GRU)
- **ConvLSTM** (Convolutional LSTM)

Among these, the **BiGRU model** achieved the highest performance with an accuracy of 98%.

## Key Features
- **Word Embeddings**: Generated using Gensim's Word2Vec model to capture semantic meaning in the text data.
- **Deep Learning Models**: Multiple architectures were trained and evaluated to compare their performance using accuracy, precision, recall, and F1-score.
- **Visualization**: Plots of model accuracy and loss during training and validation, as well as confusion matrices for the test set results.

## Results
The **BiGRU model** outperformed all other models, achieving a 98% accuracy and an F1-score of 98% for the fake news class. The bidirectional architecture allowed for better context understanding and contributed to its superior performance.
