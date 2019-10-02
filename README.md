# An Attention-based Seq2seq Neural Network Chatbot

## Info
A Generative word-level chatbot on PyTorch trained on [Microsoft's MetaLWOz data](https://www.microsoft.com/en-us/research/project/metalwoz/), hacked in a few days.

Code is documented along with really illustrative comments in the `pytorch-seq2seq-chatbook.ipynb` notebook. 

You can view and run it step-by-step. Care, training time depends on the size of your data and your neural net/hardware configuration.
## Sample Output
![Sample Output](https://i.imgur.com/TTCfFTE.png "Sample Output")

## Technologies
- Python 3
- PyTorch
- json/glob packages

-------
### Different versions
Before PyTorch, **I also tried a char-level Keras model and a word-level TensorFlow model** on the unfiltered dataset, which struggled a lot with memory usage causing multiple out-of-memory (OOM) problems, even on a Tesla K80 GPU. 

You can find them on the appropriate `different-versions` folder. 

Some workaround ideas:
- removing sentences with a high number of words
- train on a high-end GPU
- reducing hidden dimensions, units, etc
-------

## Future Work:
- Importing pre-trained embeddings like Glove
- Use SOTA Transformers like BERT
- Use early stopping on a validation set