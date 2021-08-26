# Chinese English Machine Translation Tasks
In this work, we introduce how to train the Seq2Seq model for machine translation tasks from Chinese to English. The code is public with the notebook above. After training, the obtained model is able to take as input a Chinese sentence and output an English translation. Examples:

||Input|Output|
|-------|---------|--------|
|1|天气又冷又湿。|The weather was not only cold, but also wet.|
|2|她明年會去美國嗎?|Will she go to america next year?|

Dataset for training and evaluate: CMN [[link]](http://www.manythings.org/anki/)

At this work, I solve machine translation tasks with Encoder-Decoder architecture. In this architecture, the network is partitioned into two parts, the encoder and the decoder. The encoder’s role is encoding the inputs into hidden state, or hidden representation, which often contains several tensors. Then the hidden state is passed into the decoder to generate the outputs.

1. Neural Machine Translation model with GRU layers and Bahdanau Attention.
Some predictions of the model.
![Predict1](https://github.com/ThuanPhong0126/Machine-Translation-Chinese-English/blob/main/img/predict1.png)
![Predict2](https://github.com/ThuanPhong0126/Machine-Translation-Chinese-English/blob/main/img/predict2.png)

# References
* Tensorflow official tutorial: [Neural Machine Translation with Attention](https://www.tensorflow.org/tutorials/text/nmt_with_attention)
* Seq2Seq Learning & [Neural Machine Translation](https://nthu-datalab.github.io/ml/labs/13-1_Seq2Seq-Learning_Neural-Machine-Translation/13-1_Seq2Seq-Learning_Neural-Machine-Translation.html#Checkpoints-(Object-based-saving))
* Bahdanau Attention: [Neural Machine Translation by Jointly Learning to Align and Translate](https://arxiv.org/abs/1409.0473)
