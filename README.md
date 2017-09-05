# dlnd-language-translation

Training a sequence to sequence model on a dataset of English and French sentences that can translate new sentences from English to French. Since translating the whole language of English to French will take lots of time to train, it is provided you with a small portion of the English corpus.

As an experiment different embedding sizes at encoding and decoding are provided as an experiment:

* dlnd_language_translation__embd_enc128_dec_128.html
* dlnd_language_translation__embd_enc256_dec_512.html
* dlnd_language_translation__embd_enc512_dec_512.html

Training this model was difficult due to wrong placing of dropout layer

dlnd_language_translation_dropout_error.html

---

dlnd_language_translation.ipynb is the final version after tune the hyperparameters and amend the dropout layer placing. 

## Requirements

FloydHub is a platform for training and deploying deep learning models in the cloud. It removes the hassle of launching your own cloud instances and configuring the environment. For example, FloydHub will automatically set up an AWS instance with TensorFlow, the entire Python data science toolkit, and a GPU. Then you can run your scripts or Jupyter notebooks on the instance. 
For this project: 

> floyd run --mode jupyter --gpu --env tensorflow-1.0

You can see your instance in the list is running and has ID XXXXXXXXXXXXXXXXXXXXXX. So you can stop this instance with floyd stop XXXXXXXXXXXXXXXXXXXXXX. Also, if you want more information about that instance, use floyd info XXXXXXXXXXXXXXXXXXXXXX

### Environments

FloydHub comes with a bunch of popular deep learning frameworks such as TensorFlow, Keras, Caffe, Torch, etc. You can specify which framework you want to use by setting the environment. Here's the list of environments FloydHub has available, with more to come!

### Output
Often you'll be writing data out, things like TensorFlow checkpoints. Or, updated notebooks. To get these files, you can get links to the data with:

> floyd output run_ID