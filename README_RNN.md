# Reviews Sentiment Analysis using Recurrent Neural Network (RNN)

## Contributors:
- Krishnendu Adhikary (055022)
- Mohit Agarwal (055024)

## Objective
To design, implement, and evaluate a deep learning-based sentiment analysis model using an RNN architecture. The model classifies movie reviews as positive or negative by leveraging sequential patterns in text data.

## Problem Statement
- Online movie reviews significantly influence public opinion.
- Classifying sentiment is challenging due to language complexity.
- An RNN-based model is used to capture contextual information and classify reviews accordingly.

## Key Features
- **Data Preprocessing**: Sentiment encoding, text normalization, tokenization, and sequence padding.
- **Model Development**: RNN model with an embedding layer, recurrent layer, and dense layer.
- **Training & Evaluation**: Trained on IMDB dataset, tested on Metacritic data, achieving ~86% accuracy on IMDB and ~77% on Metacritic.
- **Managerial Insights**: Business applications include customer sentiment monitoring, brand reputation analysis, and automated review filtering.

## Dataset
- IMDB dataset (50,000 reviews) from Kaggle: [Dataset Link](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews)
- 151 manually scraped Metacritic reviews for additional testing.

## Model Architecture
1. **Embedding Layer**
   - Input dimension: 20,000
   - Output dimension: 128
   - Input length: 400
2. **Recurrent Layer**
   - SimpleRNN with 64 units, Tanh activation, and dropout (0.2).
3. **Fully Connected Layer**
   - Dense layer with 1 neuron, Sigmoid activation (binary classification).

## Training Details
- Dataset split: 80% training, 20% testing (from 40,000 sampled IMDB reviews).
- **Loss Function**: Binary Crossentropy
- **Optimizer**: Adam (learning rate = 0.001)
- **Batch Size**: 32
- **Epochs**: 15 (early stopping after 3 epochs if validation loss does not improve)

## Results & Observations
- Training accuracy reached ~89%, validation accuracy stabilized at ~87%.
- Overfitting was mitigated using dropout and early stopping.
- Generalization was lower on Metacritic data (~77% accuracy), suggesting potential improvements using LSTM.

## Future Improvements
- Implement LSTM/GRU for better long-term dependencies.
- Improve text preprocessing (lemmatization, n-grams, stop-word removal).
- Expand dataset by combining IMDB and Metacritic reviews.
- Deploy real-time sentiment analysis in a dashboard.

## License
This project is licensed under the MIT License.
```
