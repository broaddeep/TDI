# TDI
Textual Difficulty Identification dataset

TDI(Textual Difficulty Identification) dataset aims to train the neural network model to distinguish textual difficulty of english sentences.

- For each topic, 5 sentences are labeled as 1 (Normal Wikipedia), while the other 5 sentences are labeled as 0(Simple Wikipedia).
- Each topic consists of 10 sentences.
- The format of the files are the same as in GLUE SST-2 (except the column 'title')


## Note

- Collected text data dump from the both of the sources.
- Extracted the text and eliminated any control / xml characters and normalized unicode.
- Filtering conditions are minimal to prevent possible human bias which can affect model performance.
  - First, sentence length should be between 70 and 210
  - Second, every topic should have at least five sentences to be included in the dataset)
- Randomly selected five sentences from each source.
- Labeled as written above.


## Citation

You can cite the paper as follows:
```
@unpublished{Park2019MTD,
author  = {Dongjun Park},
title   = {Transformer: Measuring the Textual Difficulty of English Sentences},
year    = {2019},
note    = {unpublished},
}
```
