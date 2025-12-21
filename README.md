# Simple GPT-2 esque Transformer

## Overview

This is another educational project aimed to really hone in on my transformer and attention understanding. It features BBPE tokenizing, with a vocabulary size of 5001, and a six decoder layer transformer. The model was trained for five epochs on the wikitext-2 training set with a step size of 10 tokens. 

## Project Structure:

```
simple-gpt-2/
│
├── .venv/ # Virtual environment not trakced in git
├── data/ # Data processing and loading directory
│ └── byte_pair_encoding.py # Tokenizing program
│ └── dataloader.py # Creation of dataset
├── files
│ ├── encoded_train.pt # Encoded training dataset
│ ├── encoded_val.pt # Encoded validation dataset
│ ├── gpt2_model.pt # trained model
│ ├── my_object.pkl # Trained tokenizer object
│
├── models/ Directory for model code
│ └── gpt_impleentation.py # File for the model code
│ └── positional_encodings.py # File for generating positional encodings
│ └── transformer_components.py # Decoder, MLP, Attention layers
│
├── notebooks/
│ └── byte_pair_encoding.ipynb # Training tokenizer
│ └── debugging.ipynb # Debugging each component of the model
│ └── encode_datasets.ipynb # Tokenize inputs
├── training/ # Directory for training the model
│ └── train.py # Training loop
├── .gitignore # Untracked files
├──README.md # Project documentation
└──requirements.txt # Dependencies
```

## Author's Notes

This was a simple mini-project which I used to continue my exploration of transformers. The major insight from this project include understanding how inputs are tokenized for text generation tasks. Furthermore, I felt that the way I carried out this project was in a much more organized fashion, debugging each component of the model as I built it, instead of all at once at the end. Also note that since I do not have access to much compute and all training was done on my MacBook Pro, I only ran the training loop for 5 epochs yielding a relatively high loss.

## Future Work

I will be doing research for Prof. Chin at Dartmouth in the Learning Intelligence and Signal Processing Lab! I'll be studying complex valued neural networks, so I'll likely spend the remaining weeks of my winter break building the fundamentals for that. Expect to see many contributions related to CVNNs in the coming months! (Target: ICML Workshop publication :D). I've been dabbling in many areas of deep learning, and right now interpretability, human-centered applications of AI, and Bio-ML have been catching my eye, so I'll try to get invovled in some open source contributions! I will also start looking into startups / research labs to potentially work for throughout summer of 2026 (please hire me :P).

## About the Author

Benjamin is a first-year undergraduate student at Dartmouth College studying mathematics and computer science. Recently he has been interested in machine learning and has been continuing his passion for competition math by studying for next years Putnam contest. Keep up with his progress on his personal website (currently a work in progress as of 12/21/25).