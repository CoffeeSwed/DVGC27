# fastai
## What four things do we need to tell fastai to create “DataLoaders”?
Sources : FastAI Docs
- DataBlock :
- - blocks :  Input and Output types
- - splitter : How to split the data.
- - get_y : How to get the label for an item.
- - Common
- - - item_tfms : How to transform the single items, "augmentation".
- - - batch_tfms : How to transform a batch, "augmenation". 
- Dataloader
- - path : Where to load data from
## What does the “splitter” parameter to “DataBlock” do?
The splitter is used to split the dataset into testing data and validation data.

## How do we ensure a random split always gives the same validation set?
Since the random splitter has a seed input, set the seed to a "constant".

## What does “export” in fastai save?
Export in fastai saves the Learner so it can be used to run on different test-sets and etc. We can then load the learner in with the load_learner function.

# Libraries
##  What is the library Pandas used for?
You will find it commonly used for data representation. For example, representing a table for a graph. It uses numpy arrays, making it alot more
performance efficient compared to using normal data representation found in python. 

## What is the library Numpy used for?
Numpy is used to represent arrays and matrices. It's effiency is a result of it being written in C & C++, allowing memory techniques like locality for cpu caches to be used and not needing to intepret all the lines of code working on the data.