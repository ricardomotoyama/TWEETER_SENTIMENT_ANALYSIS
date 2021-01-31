<img src="https://miro.medium.com/max/875/1*sDa7Oqnh-zRXPPewKZid4g.png" width="900" height="500">

# How data helps to figure out patterns on Tweets

Have you ever ask by yourself why a advertisement showed up on the screen of your notebook, tablet or smartphone if you didin't say anything or didn't type anything about this ad? You just thought about it.

<img src="https://i.gifer.com/5rt.gif" width="500" height="300">



At the same time that is funny it is so strange. Probably, you heard or read this sentence: "Data is the new oil of digital economy." 

At this moment there are a lots of companies are getting a plenty of informations about a video you are watching on YouTube, something you are researching on Google or your posts in some social network like Tweeter. 

Nowadays it is very important to know about people behaviours, what people think about something or about somebody and there are a lots of companies on the World that use it to figure out what kind of things do you like or your preferences.

In this case study we will make some data analysis, choose a classification model and than predict if a tweet refers or don't refer to politics, racism or sexism.



# NLP Techniques

There ae a lots of techniques to process texts into features will be used to develop classification models. We will present you these three techniques:

### 1) Bag-of-Words

Bag of words is a Natural Language Processing technique of text modelling and it is a method of feature extraction from a text data.

Besides that, bag of words is a representation of the frequency of words within a document.It keeps track of word counts and disregard the grammatical details and the word order.

<img src="https://miro.medium.com/max/875/1*xUFlK4ZSu_GQFuRvcoBLRA.png" width="700" height="300">

### 2) Term Frequency - Inverse Document Frequenct (TF-IDF)

<img src="https://mlwhiz.com/images/tfidf.png" width="900" height="500">

### 3) Word2Vec

It is a statistical method standalone word embedding from a text corpus and it is capable of capturing context of a word in a document, semantic and syntactic similarity, relation with other words.

Word2Vec works based on similarity and mathematically it maybe compared with the cosine of the angle between such vectors. If two vectors are very similar so cosine will be close to 1 and the angle between them will be close to 0. 

<img src="https://miro.medium.com/max/871/0*XMW5mf81LSHodnTi.png" width="700" height="500">


Word2Vec uses two methods: Common Bag Of Words (CBOW) or Skip-Gram.

CBOW Model takes the context of each word as an input and tries to predict the word corresponding to the context.


<img src="https://miro.medium.com/max/875/0*3DFDpaXoglalyB4c.png" width="700" height="300">

The input is an one hot encoded vector of size V and hidden layer contains N neurons. The output is again a V length vector with the elements being the softmax values.

<img src="https://miro.medium.com/max/745/0*CCsrTAjN80MqswXG" width="700" height="500">

Skip-Gram uses the target word into the network and the model outputs C probability distributions. For each context position, the model gets C probability distributions of V probabilities, one for each word.

<img src="https://miro.medium.com/max/875/0*Ta3qx5CQsrJloyCA.png" width="500" height="600">

In this case study we will apply Skip-Gram.
