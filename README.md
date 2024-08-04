# 🔠 BytePair Tokenizer Project

## Overview

Create a tokenizer using the BytePair Encoding (BPE) algorithm from scratch in Python. This project avoids external libraries like NLTK, HuggingFace, Spacy, or TextBlob. The primary goal is to develop a `Tokenizer` class with these functionalities:

- Learn vocabulary and split rules from a corpus with a specified number of merges.
- Tokenize input samples based on learned rules.

## 📂 Files

- `tokenizer.py`: Implements the `Tokenizer` class.
- `vocabulary.txt`: Lists all possible tokens after the specified number of merges.
- `merge_rules.txt`: Lists all learned merge rules after vocabulary learning.
- `tokenized_samples.txt`: Contains split tokens after tokenizing test samples.

## 🏷️ Tokenizer Class

### Methods

- **`learn_vocabulary(corpus: List[str], num_merges: int) -> None`**: Learns split rules and frequencies from the corpus based on the number of merges, updating the vocabulary and merge rules.
- **`tokenize(sample: str) -> List[str]`**: Tokenizes the input sample based on learned split rules and returns a list of tokens.

---
