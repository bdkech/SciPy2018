# SciPy 2018

## Schedule

## Tutorials
### Getting started with tensorflow v1.9
#### Josh Gordon @random_forests
#### Yash Katariya @yashk2810
#### Amit Patnkar

##### Notes
[workshops](https://github.com/tensorflow/workshops)

[Google crash course on machine learning](https://developers.google.com/machine-learning/crash-course/)

[GANS](https://github.com/tensorflow/tensorflow/tree/master/tensorflow/contrib/eager/python/examples/gan)

[Auto complete drawing](https://magenta.tensorflow.org/)

[Google facets](https://pair-code.github.io/facets/)

[Tensorflow wide and deep](https://www.tensorflow.org/tutorials/wide_and_deep)

[tutorials](https://github.com/tensorflow/models/tree/master/samples/core/tutorials/keras)

Four new API styles with recent release:
- tf.keras
- Eager execution
- Estimators
- Deferred Execution

Notebooks are downloaded and will be in the same directory as this project.

Refer to the regression notebook for good code snippets w/r/t running
models/early stoppage/and classes

"Networks are happiest with data scaled from [-1,1] or [0,1]"

L1 regularization may aid in the testing validation/loss but not the training.  

JS tensorflow allows model interaction from the web now.  [JS
tensorflow](js.tensorflow.org)


May be worth getting the deep learning and python book from manning publications


Man the more of these sessions I sit in, the more I think we should be doing
with these models.  I'm thinking I need to revisit the microarray keras model I
built and test with more layers and normalization.  The expression I feel should
be both fitted to a guassian distribution and rescaled to a 0-1 scale.


###### Eager execution
Must be called immediately after the import.  This doesn't do graph-based
execution and does not need a session.


There is a large performance penalty for using this.  But it makes debugging
easier, and allows the generation of models otherwise impossible

##### Thoughts
Free web based jupyter notebook called [Colab](colab.research.google.com), offered from Google.
A free gpu-accelerated jupyter instance offered by Google.  We've heard of them, right?

Man even tensorflow is using keras.  You can now write your models in Keras and then import them

Literally just said "Because we're google we logged your data"

Last year everyone was having you check out github projects, now it seems like
everyone has some cloud hosted service to work on.

### Introduction to Julia
##### 
##### 

[Login link](https://juliabox.com/up/aipro/AIPRO500K)


I think julia is coming along really well.  My concern currently is that its too
academic. I could really see them benfiting a bit from golangs attitude of
structure.  Some of the syntactical differences look like they could be as
obnoxious as perl to read if you weren't the one writing the code.  I'd like to
see some type of linter/package manager to really help with environment sharing.

Its definitely very R-ish in how many ways you can write your code.  I don't
necessarily mean different ways to do the same function, but how you can
spacially format your code.  I don't like that.  Give me an aggressive format
and linter to keep that stuff in line.

There are libraries for unit testing and CI, but I still feel its just immature
still.  The terniary operators look hideous and I can see being difficult to
read in shared code.  Same with the way anonymous functions are declared...or
more generally function declarations in general.  I suppose I've had too many
time where similar problems in R have come back to bite me.  

I want to keep an eye on it and see the changes that are announced with 0.7
release.  


## Talks

## Posters/Lightening talks
