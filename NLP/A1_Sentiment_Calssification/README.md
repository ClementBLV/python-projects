# AI_605_Assignement_1
## Text classification 
KAIST first NLP Assignement

Here we implement a RNN from scratch using pytorch for sentiment analysis on the Stanford Sentiment Treebank (SST). 

We use a simple space tokenizer on each sentence and add the PAD and UNK token and we use all the word to generate a vocab with only the word thats occurs more than two times. For the embedding we are simply using a mapping of the word to their index with { all_word : indx } to map each word to a unique index, if the word ins't in the vocab, it is attribute the UNK token. This is a really simple embeding of the sentences with no contextualisation. 

Then there is a really big study on the finding of the right optimizer (SGD, Adam) and the propper parameters (Learning rate, Weight decay) this study was made on the baseline model eg a simple classifier on the sentence (0 = negative and 1 = positive) 

Then a RNN has been implemented to encode the structure of the sentence and finally a LSTM has been tested to encode the past of each word in its embedding. Then word vector of glove have been used to encode the semantic similarity between words. 


Baseline : 
- SGD  best accuracy test 65.92760180995475
- Adam best accuracy test 70.54298642533936

RNN : 
- SGD best accuracy test 63.84615384615385
- Adam best accuracy test 67.51131221719457


LSTM : 
- SGD best accuracy test 59.276018099547514
- Adam best accuracy test 71.71945701357465



