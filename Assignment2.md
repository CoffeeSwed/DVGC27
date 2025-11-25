# fastai
## What four things do we need to tell fastai to create “DataLoaders”?
- Dataset : Dataset to load data from.
- -splitter : How to split the data.
- -get_y : How to get the label for a "tensor" or data item.
- -item_tfms : How to transform the single items, augmentation or something similar.
- -batch_tfms : How to transform a batch, either augmenation or something similar. 

## What does the “splitter” parameter to “DataBlock” do?
The splitter is used to split the dataset into testing data and validation data.

## How do we ensure a random split always gives the same validation set?
Since the random splitter has a seed input, set the seed to a "constant".

## What does “export” in fastai save?
Export in fastai saves the trained model data so it can be used to run on different test-sets and etc. The save method would save training data also,
increasing effiency of resuming training. 

# Libraries
##  What is the library Pandas used for?
You will find it commonly used for data representation. For example, representing a table for a graph. It uses numpy arrays, making it alot more
performance efficient compared to using normal data representation found in python. 

## What is the library Numpy used for?
Numpy is used to represent arrays and matrices. It's effiency is a result of it being written in C & C++, allowing memory techniques like locality for cpu caches to be used and not needing to intepret all the lines of code working on the data.