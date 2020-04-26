# Word2Vec using Skip-Gram Demo

The following example shows the usage of Word2Vec and how a custom
model can be improved. The implementation is based on TenorFlow, Keras, gensim
and can easily be run as a [Colab-Notebook](https://colab.research.google.com/)

How to Test
- Go To [Google Colab](https://colab.research.google.com/)
- Create Gmail/Google Account (or login)
- Open the File via "File" -> "Open Notebook" -> Github
- Open `word2vec.ipynb` in https://github.com/geri-m/word2vec
- "Runtime" -> "Run All"

This sample code is from the tutorial on [Cambridge spark](https://blog.cambridgespark.com/tutorial-build-your-own-embedding-and-use-it-in-a-neural-network-e9cde4a81296).

There is a good pre-read on [towardsdatascience.com](https://towardsdatascience.com/introduction-to-word-embedding-and-word2vec-652d0c2060fa)

# Goal

The Goal of this sample to so tag (= classify) word types of a given text. The model should be able to answer for example the following questions as accuarte as possible.
```
"Is the word 'will' in the sentense 'This is my last will' a noun?"
"Is the word 'will' in the sentense 'I will do that' a verb?"
```

## Background Information

The tags will be applied according to [conll2000](https://www.clips.uantwerpen.be/conll2000/chunking/), (Conference on Computational Natural Language Learning).

## Demonstration

The demo will show that by adding more context to a word (= taking surounding words into consideration), it is more likly to classify the word correctly.


###  Known Issue

If you come across the following Warning, no worries. It is a [known issue](https://github.com/tensorflow/tensorflow/issues/37144)
and does not impact the runtime behaviour of the tutorial.

```
WARNING:tensorflow:AutoGraph could not transform <function Model.make_predict_function.<locals>.predict_function at 0x7f38a8c1bf28> and will run it as-is.
Please report this to the TensorFlow team. When filing the bug, set the verbosity to 10 (on Linux, `export AUTOGRAPH_VERBOSITY=10`) and attach the full output.
Cause: Bad argument number for Name: 4, expecting 3
To silence this warning, decorate the function with @tf.autograph.experimental.do_not_convert
WARNING: AutoGraph could not transform <function Model.make_predict_function.<locals>.predict_function at 0x7f38a8c1bf28> and will run it as-is.
Please report this to the TensorFlow team. When filing the bug, set the verbosity to 10 (on Linux, `export AUTOGRAPH_VERBOSITY=10`) and attach the full output.
Cause: Bad argument number for Name: 4, expecting 3
To silence this warning, decorate the function with @tf.autograph.experimental.do_not_convert
```
