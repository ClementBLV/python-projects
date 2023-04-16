# AI_605_Assignement_3
## Transformer 
KAIST AI605 thrid assignement

goal : implement an encodeur decodeur tranformer from scratch for spelling correction 

In this project we have implemented the  The Annotated Transformer ( http://nlp.seas.harvard.edu/annotated-transformer/) 

### Task 1 : Encoder Decoder
A simple task to encode a vectore and decode it correctly. It can be an efficiant way to store information in a compact way 

### Task 2 : Spelling correction : word 
We take the vocab of Squad dataset we infise it with noise, eg mistakes in the words, it can be insertion, deletion , substitution of a charater at the level of the word. We randomly choose the token which will be corrupted. 

### Task 3 : Spelling correction : Sentence 
We take the same process but this time at the sentence level. We randomly corrupt some word randomly choose in the sentence. 