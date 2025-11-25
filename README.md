Hybrid Deep Learning Model — Airline Tweet Sentiment Analysis

Embeddings + Bi-LSTM + Numeric Metadata | Multi-Class NLP Classification

A hybrid neural network that combines text-based sentiment extraction with numerical airline metadata features to classify tweets into Positive, Negative, and Neutral.
This model outperforms standalone text-only architectures and delivers state-of-the-art multi-class accuracy on the popular Twitter US Airline Sentiment dataset.

**Key Features**
-Hybrid architecture → merges text embeddings + Bi-LSTM with numeric airline metadata (e.g., airline name, tweet length, user stats).
-Multi-class classification → predicts Positive / Negative / Neutral.
-Custom preprocessing pipeline for text cleaning, tokenization, and metadata preparation.
-Regularization using Dropout + EarlyStopping.
-Includes Confusion Matrix, Classification Report, and performance benchmarking.
-Outperforms baseline text-only deep learning models.

**Model Architecture
Text Branch**
-Tokenizer → Sequence Padding
-Embedding Layer
-Bidirectional LSTM
-Dropout

**Metadata Branch**
-Numerical airline features (e.g., airline ID, tweet length, user metrics)
-Dense layers + ReLU

**Fusion**
-Concatenation of LSTM output + metadata vector
-Dense layers
-Softmax (3 classes)
