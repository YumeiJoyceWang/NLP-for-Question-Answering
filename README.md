# Project Desription
Key-Value Memory Network for Question Answering
This project implements a Key-Value Memory Network to perform fact-based question answering using a simplified version of the Wikipedia biography dataset. The model learns to retrieve answers by associating entity-relation pairs with factual information and leveraging memory-based attention mechanisms.

## Overview
The goal is to answer natural language questions like:

"Where was Barack Obama born?"

by extracting the entity ("Barack Obama") and relation ("place of birth"), and retrieving the correct value from memory.

## Features
Preprocessed a custom dataset to structure it into key-value pairs representing [relation → person].

Built a vocabulary object to tokenize questions and map tokens back to words.

Implemented a Key-Value Memory Network with an attention mechanism in PyTorch.

Used GloVe embeddings to convert questions into bag-of-words vectors for model input.

Extracted entities and relations using simple NLP rules via NLTK.

## Performance
Achieved 60% accuracy on the test set.

Model serves as a baseline for future enhancements such as:

Replacing BoW with contextual embeddings (e.g. BERT)

Improving entity/relation extraction using dependency parsing or NER

Augmenting the dataset or fine-tuning on domain-specific data

## Tech Stack
Python, PyTorch, NLTK

GloVe word embeddings

Custom dataset processing pipeline

## Learning Outcomes
Gained hands-on experience in designing interpretable NLP models

Understood the mechanics of memory networks for reasoning tasks

Explored practical challenges in entity/relation extraction from real-world text
