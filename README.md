# Sentiment-Analysis-using-Bi-LSTM

Done for partial fulfillment of the course Information Retrieval (CS F469) at BITS Pilani. 

In the traditional recurrent neural network model and LSTM model, information can only be propagated in forward direction. BiLSTM which combines bidirectional recurrent neural network
(BiRNN) models and LSTM units is used to capture the context information in both directions. Our embeddings are an amalgamation of Word2Vec vectors, TF-IDF scores and sentiment scores
obtained with the help of English sentiment dictionary WordNet. These embeddings are fed into the BiLSTM model, which classifies the compressed vector representations into Positive/Negative
sentiments.

For our experiments, we use [Sentiment140 dataset]([url](https://www.kaggle.com/kazanova/sentiment140)) with 1.6 million tweets. After training the two models, we save their weights and perform tests on the testing dataset. This
test dataset is a set of sentences the model has never seen before. We evaluate the Precision, Recall and F1-score for both model on positve Sentiment data, negative sentiment data and the entire
dataset. We use Tkinter (a Python library) to create the GUI for the sentiment detection in a sentence.
