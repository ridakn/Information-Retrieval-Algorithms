# Information-Retrieval-Algorithms
Assessed and implemented information retrieval algorithms using the Lemur Toolkit.

## Introduction

<p align = "justify">
In this project, we were supposed assess and implement information retrieval algorithms using the Lemur Toolkit. There were four algorithms that were to be implemented: RawTF, RawTFIDF, LogTFIDF and Okapi. Four text configurations were used: Keep stopwords and No stemming, Keep stopwords and Do stemming, Remove stopwords and No stemming and Remove stopwords and Do stemming. </p>

## Results

### Experiment 1 

In experiment 1, the performance of the retrieval algorithm "RawTF" was tested with all four types of configurations on the text data.

<p align = "justify">
There was a significant increase in performance when stopwords were removed. Since, RawTF doesn't take into count the varied importance of words i.e. gives equal importance to all words, removing stopwords greatly improves the precision value. However, using stemming didn't improve the R-precision value as well. Therefore, when using RawTF, the best performance was removing stopwords and not using stemming. </p>

### Experiment 2

<p align = "justify">
For the second experiment, the other three algorithms were implemented for all four text data configurations. </p>
 
<p align = "justify">
The results of the implementations of all four algorithms showcase that the worst performing model was RawTF. This can be due to the simplicity of the model as it only takes into account the term frequency and gives equal importance to all terms. The best performing model was Okapi model. This is expected as firstly Okapi model gives importance to rare terms and lessens the importance of frequent terms, it also focuses on scaling and works well for the text data. </p>
  
<p align = "justify">
The worst performing configuration was not doing any processing on the text data i.e. keep all stopwords and not doing stemming. This makes sense as processing text data seems to be an important step in information retrieval. The best performing configuration was doing both processing techniques i.e. removing the stopwords using the stopwords list as well as doing stemming on the text data. This ensures important (rare) terms are prioritizes and consequently higher number of relevant documents are returned. </p>
  
<p align = "justify">
The best performing combination of model and processing technique was removing stopwords, doing stemming and using the Okapi model. This provided the highest R-precision value of 0.3813. </p>

### Experiment 3

<p align = "justify">
For the third experiment, I implemented the same algorithms but with a different stemmer (krovetz instead of porter). Krovetz seemed to worsen the performance when compared to Porter. However, the above analysis still held i.e. the worst performing model remained RawTF. Okapi and LogTFIDF are popular algorithms and their performance here validates this fact. </p>
