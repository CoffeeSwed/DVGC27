# Part 1
## What four things do we need to tell fastai to create “DataLoaders”?
- Dataset : Dataset to load data from.
- -splitter : How to split the data.
- -get_y : How to get the label for a "tensor" or data item.
- -item_tfms : How to transform the single items, augmentation or something similar.
- -batch_tfms : How to transform a batch, either augmenation or something similar. 
