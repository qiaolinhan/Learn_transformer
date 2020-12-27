# Sequence to sequence learning and attention #
* Paper ['attention is all you need'](https://papers.nips.cc/paper/2017/file/3f5ee243547dee91fbd053c1c4a845aa-Paper.pdf)  
* Seq2Seq is a neural net that transforms a given sequence or element, (such as the sequecne of words in a scentence), into another sequence.  
* Seq2Seq is particularly goood at  translation. A popular choice for this type of model is __LSTM__-based models.
* Seq2Seq models consist of Encoder and Decoder. The Encoder takes the input sequence and map it into a higher dimentional space (_n_-dimentional vector). The abstract vector is feed into the Decoder which turns it into an output sequence.  

![transformer](https://miro.medium.com/max/2880/1*BHzGVskWGS_3jEcYYi6miQ.png){width=20%}
