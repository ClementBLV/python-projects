# AI_605_Assignement_2
## Information Retreival 
AI 605 NLP Assignement 2 

collab : https://colab.research.google.com/drive/1F_9J_6aBjpL7CqZxIjXYqEnw7CRcXqXI?usp=sharing
dataset : SQUAD dataset 

In this project we are testing the different methods of retreiving information form a text and linking the question to its most related context. Firstly we study matically the calcul of similarity and check the property of a distance. 
The tokenizer used is a space tokenizer with lowercasing. 

The following methods for retreiving information have been implemented : 

### Bag Of Word: 
So firstly we implement a bag of word which take a sentence into input and return the index of the most n most similar sentence given in its training. BOW.search("Sentence input", n) = list(idx1 = index of the most similar, idx2 = index of the second most similar ... ) 

### TFIDF: 
With the TFIDF on the recall of finding the proper context related to a question we have much better results than with the bag of words :  
recall TFIDF =  0.7642384105960265
recall BOW   =  0.5043519394512772

### Dense search: 
We use this time 'bert-base-uncased' for the tokenizer and the word embedding. Then we uses dense matric because each word has a vector as embedding and without it it would be to heavy. 

Then we uses this embedding with FAISS 