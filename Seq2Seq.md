# Sequence to sequence learning and attention #
* Paper ['attention is all you need'](https://papers.nips.cc/paper/2017/file/3f5ee243547dee91fbd053c1c4a845aa-Paper.pdf)  
* Seq2Seq is a neural net that transforms a given sequence or element, (such as the sequecne of words in a scentence), into another sequence.  
* Seq2Seq is particularly goood at  translation. A popular choice for this type of model is __LSTM__-based models.
* Seq2Seq models consist of Encoder and Decoder. The Encoder takes the input sequence and map it into a higher dimentional space (_n_-dimentional vector). The abstract vector is feed into the Decoder which turns it into an output sequence.  
<img src="https://miro.medium.com/max/2880/1*BHzGVskWGS_3jEcYYi6miQ.png" width="200">|<img src="https://miro.medium.com/max/700/1*ETe4WrKJ1lS1MKDgBPIM0g.png" width="200">  
The Encoder of transformer module consists of a multi-head attention and feed forward layers. - [] slight but important part: positional encoding (Give every word/part in the sequence a relative position since a sequence depends on the order of its elements, since there is no recurrent networks taht can remember how sequecnes are fed into a model.)
$$ \textit{Attention}(Q, K, V) = \textit{softmax}(\frac{QK^T}{\sqrt{d_k}})V $$
where $Q$ is a matrix contains the query (vector represent one word in a sequecne); $K$ are all the keys (vector represents all the words in a sequence); $V$ are the values.  
The values in $V$ are numtiplied and summed with some attention-weights $a$, which are defined by:
$$a = \textit{softmax}(\frac{QK^T}{\sqrt{d_k}})$$
This means that 
