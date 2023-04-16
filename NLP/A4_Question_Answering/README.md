# AI_605_Assignement_4
## Context retreiver - Question answering
KAIST AI605 thrid assignement

dataset : SQUAD 

In this project we uses transformer for machine reading comprehention applied to question answering. The goal is to predict the start and end token of the answer of a question in a context. 

### Fine Tune BERT 
We use bert-base-cased on SQUAD and we just take the element in SQUAD which have an answer. And if there are plausible answer we convert them into answer during the dataset preparation. We use BERT tokeniser and a PAD token for the tokenisation and then we encode each token and we fine tune the model on this task. 
So with bert we get around 60 % of accuracy on the all positions.

### T5 
We do the same process with T5 tranformer and obtain the following result. 
 64.6% of the time the answer and T5 answer are exactly the same. 
And in 71.6% of the time the aswer proposed by T5 is in the real answer, and 76.6% of the time the real answer is in T5 