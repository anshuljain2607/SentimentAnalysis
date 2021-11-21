# Sentiment Analysis Using Natural Language Processing


### Live Link:  https://sentiment-analysis0001.herokuapp.com/ 

![image](https://user-images.githubusercontent.com/48025630/142765623-5e56e3b5-aa5e-4db8-b868-15001821e23c.png)

Sentiment Analysis refers to detecting the polarity of any comment whether it is having a positive meaning or negative. It has multiple applications for example in checking review of a newly launched movie , for checking sentiment about any movement like kissan andolan and also for automatic feedback classification and many more. 


 ## Flowchart
![enter image description here](https://github.com/ritik-sys/movie-review-analysis-using-NLP/blob/main/Screenshots/Screenshot5.png)

## DATA PREPROCESSING
Text is messy, people love to throw in attempts at expressing themselves more clearly by adding extravagant punctuation and spelling words incorrectly. However, machine learning models can’t cope with text as input, so we need to map the characters and words to numerical representations.
Basic pre-processing for text consists of removing non-alphabetic characters, stop words (a set of very common words like the, a, and, etc.) and changing all words to lowercase.

## Bag of Words

![image](https://user-images.githubusercontent.com/48025630/142765836-9731c34b-e477-4fb6-9019-808590245629.png)


We obtain the vocabulary list from the corpus (whole text dataset). The length of the vocabulary list is equal to the length of the vector that will be output when we apply Bag of Words (BOW). For each item (could be an entry, sentence, line of text), we transform the text into a frequency count in the form of a vector. In this case, we limit it to the top 5000 words to restrict the dimensionality of the data. We code this by setting up a count vectorizer from sklearn’s library, fit it on the training data and then transform both the training and test data.

## Word2Vec

![image](https://user-images.githubusercontent.com/48025630/142765812-4b716a10-4bd5-46c4-90fe-10681621a3a1.png)


Word2vec (Word to Vector) is a two-layer neural net that processes text. Its input is a text corpus and its output is a set of vectors: feature vectors for words in that corpus. The algorithm was created by Google in 2013. The 50-D space can be visualised by using classical projection methods (e.g. PCA) to reduce the vectors to two-dimensional data that can be plotted on a graph.


## Tf-Idf

![image](https://user-images.githubusercontent.com/48025630/142765802-8057b348-7880-413c-aae5-f2bad03c08c2.png)


This is short for Term-frequency-Inverse-Document-Frequency and gives us a measure of how important a word is in the document.
Term frequency (the same as for bag of words):Inverse document frequency measures how rare a term is across all documents (the higher the value, the rarer the word).
We combine these two to get Tf-Idf.To implement this representation, we use the TfidfTransformer function from sklearn’s library. Fitting occurs on the training set and the values for the same words are determined for the test set.


 ## UI/UX
 ### Screenshot-1![enter image description here](https://github.com/ritik-sys/movie-review-analysis-using-NLP/blob/main/Screenshots/Screenshot2.png)
 ### Screenshot-2![enter image description here](https://github.com/ritik-sys/movie-review-analysis-using-NLP/blob/main/Screenshots/screenshot1.png)
 ### Screenshot-3![enter image description here](https://github.com/ritik-sys/movie-review-analysis-using-NLP/blob/main/Screenshots/Screenshot3.png)4
 
## Tech Stack and Tools : Python, Flask, Keras, Tensorflow

## Installation :zap:

 **1. Clone this repo by running the following command :-**
 ```bash
  git clone https://github.com/anshuljain2607/SentimentAnalysis.git
  cd movie-review-analysis-using-NLP
 ```
 
 **2. Now start the  server  by running the following command :-**
 ```bash
 python app.py
 ```
 
 **4.** **🎉  Open your browser and go to  `https://localhost:3000`**
 
## Contributors 🤝
 - [**Anshul Jain**](https://github.com/anshuljain2607)  


