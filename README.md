## Text-summarization

<img src = "https://github.com/rkv-2401/Text-summarization/assets/59438748/f7a226a8-6bac-494b-ad48-5f3055791cf7" width = 90%>
<p>Actual summaries.</p>
<img src = "https://github.com/rkv-2401/Text-summarization/assets/59438748/2516c7e0-aa0c-4e0c-8354-763634e295cd" width = 90%>
<br />
<p> Predicted summaries.</p>
<img src = "https://github.com/rkv-2401/Text-summarization/assets/59438748/299d14e9-7f3e-4f7f-9905-deaac1edaa98" width = 90%>

### Note - please check out approach 2 for this better performing model.

#### Tried abstractive text summarization using an LSTM model on the medical transcriptions dataset. Many potential improvements left.

#### This was approach #1, inspired by the tutorial at : https://www.analyticsvidhya.com/blog/2019/06/comprehensive-guide-text-summarization-using-deep-learning-python/
#### In this approach, we have an encoder-decoder model connected to a dense layer the size of the text vocabulary. For an output token, the model outputs a vector of probabilities of each of the words and the most probable word is chosen from the vector.
#### This approach is, in my opinion, not the best approach and the results indicate this too.  

#### It seems largely wasteful to try to output a vector that is as long as the entire vocabulary for every token in an output sequence. 
#### There might be 50-100 such tokens in one output sequence and there might be 100 - 10k+ such output sequences generated from a dataset.

##### TODO:

###### Extractive Text Summarization
###### Heuristics approach with a classifier.
###### Comparison of results

###### Upload the GRU model.
###### Section Tagging - Text Analytics
###### Manual TF-IDF Word Tokenization / Utilization of word embedding.
###### Also make a CNN model to see what happens.
###### Extractive text summarization followed by Abstractive.


###### Long-term ideas:
###### Structural compression and structural coverage scores - results
###### Fact correectness evaluation - FAR-ASS
###### Text coherence algorithm
###### Section tagging 
###### Sentence selection importance
###### Beam Search / Vector similarity search
