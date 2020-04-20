# Part4
This part mainly works with text, including traditional RNN, self-attention model, transfer learning and seq2seq model.
## Self-Attention  Model
Self-attention is a technique where we score the input sequence hidden states with respect to the final hidden representation we use for classification.<br>
Attention is a very useful technique used in all of deep learning to figure out what parts of the input are more important for producing the output. This helps us use a more relevant feature representation of the input with respect to the end goal. In NLP applications, we typically want to know which words (or tokens) in the input sequence are important for our task.<br>
This [page](https://medium.com/datadriveninvestor/attention-in-rnns-321fbcd64f05) gives a good view about how self-attention model works, or you can also refer to the pytorch [tutorial](https://pytorch.org/tutorials/intermediate/seq2seq_translation_tutorial.html).

![](https://github.com/GuoyaoShen/DeepLearningRepo/blob/master/part4/figs/self_attention_model.png "Self-Attention  Model")


## Seq2Seq Model
Seq2Seq Encoder-Decoder model in this part will take in text and the decoder will generate corresponding summary. Here for seq2seq model, teacher-forcing is also used: when looping the decoder, instead of takingself-output to input to next loop, a random variable is used to decide whether using teacher-forcingin next loop:  input the real word embedding of summary as input of next loop.

![](https://github.com/GuoyaoShen/DeepLearningRepo/blob/master/part4/figs/q6_encoder.png "Seq2Seq Encoder")

![](https://github.com/GuoyaoShen/DeepLearningRepo/blob/master/part4/figs/q6_decoder.png "Seq2Seq Decoder")

Below shows a detail of how seq2seq model works.

![](https://github.com/GuoyaoShen/DeepLearningRepo/blob/master/part4/figs/q6_seq2seq.png "Seq2Seq")

A brief structure of seq2seq model is shown below.

![](https://github.com/GuoyaoShen/DeepLearningRepo/blob/master/part4/figs/q6_seq2seq_v2.png "Seq2Seq Brief")

Below gives out some examples of original review texts, summaries and predicted summaries.

![](https://github.com/GuoyaoShen/DeepLearningRepo/blob/master/part4/figs/q6_result1.png "eg1")
![](https://github.com/GuoyaoShen/DeepLearningRepo/blob/master/part4/figs/q6_result2.png "eg2")
![](https://github.com/GuoyaoShen/DeepLearningRepo/blob/master/part4/figs/q6_result3.png "eg3")
![](https://github.com/GuoyaoShen/DeepLearningRepo/blob/master/part4/figs/q6_result4.png "eg4")
![](https://github.com/GuoyaoShen/DeepLearningRepo/blob/master/part4/figs/q6_result5.png "eg5")
