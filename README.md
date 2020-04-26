# Word2Vec/Skip-Gram Demo

The following example shows the usage of Word2Vec and how a custom
model can be improved. The implementation is based on `TensorFlow 2 `
and can easily be run as a Colab-Notebook (https://colab.research.google.com/)

How to Test
- Go To [Google Colab](https://colab.research.google.com/)
- Create Gmail/Google Account (or login)
- Open the File via "File" -> "Open Notebook" -> Github
- "Runtime" -> "Run All"

Source for the Example given here: https://blog.cambridgespark.com/tutorial-build-your-own-embedding-and-use-it-in-a-neural-network-e9cde4a81296

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
