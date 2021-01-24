# RNN for Sentiment Gauging

This repository is to illustrate the use of LSTM based RNNs for sentiment gauging from text.

Dataset: 

Tweets in response to the "The Social Dilemma" documentary on Netflix was used for sentiment gauging. Sentiments were classifed in to 3 classes: Positive, Negative and Neutral. Source: https://www.kaggle.com/kaushiksuresh147/the-social-dilemma-tweets/notebooks

Approach: 

GloveVectors were used to arrive at word vectors and word embeddings. They were used in the embedded layer within an LSTM based RNN. Each word in this process was converted to a 50 D vector and a max length of 40 words was taken for the tweets. Shorter tweets were padded to ensure correct dimension for processing by RNN.

Conclusion: 

1. Although simple in approach and complexity, the model had an accuracy of 92 % on the test dataset. 
2. GloveVectors helps better model contextual meaning of words based on their position in the text. 
3. As word embeddings based on GloveVectors are used, semantic closeness of words can be better detected by this approach.
4. A similar approach can be used to gauge sentiment from any textual data and classify the purpose/intent in to one of the several classes on which the model is trained.
