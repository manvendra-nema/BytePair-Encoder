# BytePair Tokenizer Project

## Overview

This project involves creating a tokenizer based on the BytePair Encoding (BPE) algorithm from scratch. The tokenizer is implemented in Python without using any external libraries like NLTK, HuggingFace, Spacy, or TextBlob. The primary goal is to develop a `Tokenizer` class with the following functionalities:

- **Learning the vocabulary and split rules** based on a given corpus and a specified number of merges.
- **Tokenizing a given input sample** based on the learned rules.

## Files

The project includes the following files:

- `tokenizer.py`: Contains the implementation of the `Tokenizer` class.
- `vocabulary.txt`: A file listing all possible tokens in the vocabulary after a specified number of merges.
- `merge_rules.txt`: A file listing all the merge rules learned after learning the vocabulary for the specified number of merges.
- `tokenized_samples.txt`: A file containing the split tokens after tokenizing a set of test samples.

## Tokenizer Class

### Methods

#### `learn_vocabulary(corpus: List[str], num_merges: int) -> None`

This method learns the split rules and frequencies from the given corpus based on the specified number of merges. It updates the vocabulary and merge rules accordingly.

#### `tokenize(sample: str) -> List[str]`

This method tokenizes the given input sample based on the learned split rules and returns the list of tokens.
