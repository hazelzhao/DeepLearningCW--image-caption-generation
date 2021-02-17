# Image Caption Generation

## CNN-LSTM & CNN-RNN

## Motivaiton
   
   1. Understand the principles of text pre-processing and text embeddings

   2. Gain experience working with an image to text model

   3. Compare the performance and usage of RNNs versus LSTMs as sequence generators

### Dataset - Flickr8k

### 1. Text preparation

The first step is to build a vocabulary. The vocabulary consists of all the possible words which can be used - both as input into the model, and as an output prediction. To build the vocabulary:

a. Parse the lines variable in the starter code, splitting the image ID from the caption text.

b. Split the caption text into words and trim any trailing whitespaces.

c. Convert all words into lowercase by calling word.lower().

d. Remove any punctuation (periods, commas, etc.).

e. Since the vocabulary size affects the embedding layer dimensions, it is better to remove the very infrequently used words from the vocabulary. Remove any words which appear 3 times or less; this should leave you with a vocabulary size of roughly 3440 (plus or minus some is fine).

f. Add all the remaining words to an instance of the Vocabulary() object provided.

### 2. Encoder network -- CNN

### 3. BLEU for evaluation
One common way of comparing a generated text to a reference text is using BLEU.

The Python ntlk package for natural language processing provides a function
sentence_bleu() which computes this score given one or more reference texts and a
hypothesis.


### Discussion

1. Lemmatization?

2. Compare RNN and LSTM

