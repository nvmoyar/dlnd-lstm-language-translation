# Deep Learning Nanodegree

## Language Translation

[image1]: ./images/language-translation_screenshot.png "Language Translation Screenshot"

### Project Overview

In this project a sequence to sequence model is trained on a custom small dataset of English and French sentences in order to translate new sentences from English to French using TensorFlow. 


![Language Translation Screenshot][image1]


### Install and Requirements

FloydHub is a platform for training and deploying deep learning models in the cloud. It removes the hassle of launching your own cloud instances and configuring the environment. For example, FloydHub will automatically set up an AWS instance with TensorFlow, the entire Python data science toolkit, and a GPU. Then you can run your scripts or Jupyter notebooks on the instance. 
For this project: 

> floyd run --mode jupyter --gpu --env tensorflow-1.0

You can see your instance in the list is running and has ID XXXXXXXXXXXXXXXXXXXXXX. So you can stop this instance with floyd stop XXXXXXXXXXXXXXXXXXXXXX. Also, if you want more information about that instance, use floyd info XXXXXXXXXXXXXXXXXXXXXX

### Environments

FloydHub comes with a bunch of popular deep learning frameworks such as TensorFlow, Keras, Caffe, Torch, etc. You can specify which framework you want to use by setting the environment. Here's the list of environments FloydHub has available, with more to come!

### Output
Often you'll be writing data out, things like TensorFlow checkpoints. Or, updated notebooks. To get these files, you can get links to the data with:

> floyd output run_ID

### Install environment, Test

* [Test](http://localhost:8888/notebooks/dlnd_language_translation.ipynb)
* [Demo](https://www.floydhub.com/nvmoyar/projects/text-translation)