[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/ymop5HUw)

# CMPSC 310 Activity 15

## Deadline: April 12 by 9:50am

## Assignment

For this activity follow [Neural machine translation with a Transformer and Keras](https://www.tensorflow.org/text/tutorials/transformer).

## Submission

Submit completed Colab notebook showing generated output.

## Data

The dataset is a set of portugese-english translations. The dataset has 55,000 total examples in it. The data is in pairs of portugese words and english translations. The words are then tokenized to allow for input into the model. This process removes punctuation and sets the text case to be the same.

## Transformer

The tokens created in the data processing step are first embedded in the transformer and turned into vectors. The data then goes through the attention modules which are like dictionary lookups. The center of the transformer is the cross attention layer, which connects the encoder and decoder. Then, there is the global self attention layer that processes the contect sequence. The causal self attention layer is similar to the global layer, but for the output. Broadly, the encoder layer is in the input side and the decoder layer is on the output side. The final transformer has over 10,000,000 parameters.
