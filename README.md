NLP_Masked_Language_Models
Author
Calvin Harmsen

Course
Natural Language Processing Assignment 10.5

Project Description
This project compares two approaches for masked language modeling:

A manually created prediction model using a local text corpus and word-frequency/context matching.
A pretrained BERT model using the Hugging Face Transformers library.
The goal is to demonstrate how modern transformer-based language models use context to predict missing words and how their performance compares to simpler statistical methods.

Files
masked_prediction_comparison.py - Main Python program
corpus.txt - Training corpus used by the manual prediction model
README.md - Project documentation
Requirements
Install the required libraries:

pip install transformers torch
Test Sentences
The following masked sentences were used for testing:

The cat sat on the [MASK]
I went to the [MASK] to buy food
She deposited money in the [MASK]

Manual Model
The manual prediction model:

Loads text from a local corpus
Preprocesses the text
Builds a context-frequency model
Predicts likely words based on patterns found in the corpus
This approach is limited by the size and quality of the corpus.

BERT Model
The project uses the pretrained:

bert-base-uncased
model through the Hugging Face Transformers library.

BERT predicts masked words using context learned from large-scale language training.

Results Summary
The manual model produced mixed results and often struggled when the required context was not present in the corpus.

The BERT model generally produced more meaningful predictions because it used broader contextual information learned during pretraining.

Both models demonstrated limitations, showing that language models can still generate unexpected or incorrect outputs.

Learning Outcomes
Through this project I learned:

How masked language models work
How to build a simple prediction model
How pretrained transformer models operate
The importance of context in language understanding
The strengths and limitations of modern NLP systems
