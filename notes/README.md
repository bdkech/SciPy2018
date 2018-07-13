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

### Open source tools
####
Notes/results for this talk are available here [Open source
tutorial](https://github.com/bdkech/hugs-bdkech)

[Also here](https://jrleeman.github.io/SettingUpOpenSource/)

### Bayesian models
Notebooks are available as part of the repo

Mike potencoat?  He has a blog about bayesian models

kale divergence between two curves for ECDF and CDF 
## Talks
### SciKit build
[Python package life cycle](packaging.python.org)
Refer to the packaging tutorial from SciPy 2018.

Attempts to be a bridge between cmake, existing projects, and the python
ecosystem.  Here the hope is to allow quicker cross-compliation.  

- not meant to reinvent the whl
- its part of the building workflow
- it *is* a drop in replacement 
- has support for developer mode (pip install -e)
[presentation slides](bit.ly/scikit-build-talk)
[project](github.com/scikit-build/scikit-build)
### AutoML
#### Randal OlsonTt
Talked with Randal about autoML and our datasets.  He agreed the data itself is
too wide, and most autoML frameworks would fail to find adequate models.  He
suggested tpot, tpotmdr, and scikit-rebate.  These are made to work on wider
datasets and could be useful.  Also he agreed the approach of finding
coefficients and then using that as a selection criteria could help in the
approaches.

### Apache Ray
#### Rise labs

Man this has come a long way since it originally came out.  I think its worth
looking into how it handles its execute orders and everything.  I'm not sure if
you can get it to plug into actual schedulers and execution engines.  We'll see.
It has matured a great deal over a year.  Pretgitty interesting.

### Tools plenary session
#### NumPy 
I didn't realize this was pronounced Num-pee.  You learn something new everyday.  
Some of the updates do better handling of temporary data.  Other low level stuff
that didn't really impact me

#### Pandas
PARQUET! PARQUET FORMAT WOOOHOO!  Also they're getting S3 support; generally
being extensible for other formats.

Deprecation of ix.

The introduction of the pandas datatypes.  You can define your own array-like
and tell pandas how to work with it.  

Exciting times

#### Matplotlib
Dropping python 2.7!!

v2.2 is going to be the next LTS.  Still supports 2.7; 3.0 requires python 3.x

constrained layout manager, so now it can try and fit everything for you.  

#### Scikit-learn
Lots of new stuff coming in the next release.  

One hot encoder for strings is on the way.  
Column transformer -> lets you convert things to a numpy array/pandas frame and
then a mask to apply transformations on particular columns.

#### Conda
Don't care.

### Apache Arrow
#### Wes McKinney

Gpu support and stuff for arrow:
gpuopenanalytics.com
### CIS interface

communication between models in different langs
reduce complexity of writing models

This is available from pip.  Seems really interesting, yml file that defines
connections/dependencies.  Data goes right between the models, no intermediates.

My thoughts with this revolve around making some computational framework for
people to generate workflows.  Imagine an API that can report models in your
library, what they require, and then the capability to upload a yml file to the
API to handle execution.  There would need to be some quality of life
improvements done.  Combine that with Morgans interactive data tree project and
now you've got an ecosystem where you can easily traverse datasets AND models
WITH an added ability to do complex execute tasks. 


### Later talks to come
## Posters/Lightening talks
Open Ocean??  ---> using docker/"pods" for sharing reporducible research
[githubg - dvid : janelia-flyem](https://github.com/janelia-flyem)
## General chats

[Github project for data
management](https://github.com/Morgan243/InteractiveDataTree)
