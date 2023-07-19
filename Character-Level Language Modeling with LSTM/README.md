# Language Modeling with LSTM using TensorFlow
## Overview
This project focuses on implementing a character-level language model using Long Short-Term Memory (LSTM) in TensorFlow. The goal is to generate next-text predictions character by character. The model is trained on Shakespeare's texts to learn intricate patterns and generate new text based on the provided seed sequence.

## Methodology
The methodology involves importing necessary libraries such as NumPy and TensorFlow, and utilizing TensorFlow models and layers like LSTM, Dense, Dropout, Activation, etc. The code starts with creating a dictionary to map characters to integer indices. The text is preprocessed by reshaping, normalization, and one-hot encoding. The LSTM layer is added to the model with 512 units, enabling it to capture complex patterns. Regularization techniques like dropout are applied to prevent overfitting. The model is compiled with the categorical crossentropy loss function and trained using the Adam optimizer. After training, the model can generate new text based on a seed sequence.

## Results
The results of text generation using the trained model are impressive. The generated text closely resembles Shakespeare's sonnets, demonstrating the model's ability to capture the linguistic patterns and themes present in the training data. Sample outputs of generated text are included in the project for reference. The trained model achieved a perplexity of 218.24, suggesting good performance.
