# Headline Generation Project

## Overview

This project focuses on generating headlines from news articles using three different models: T5, LDA, and LSTM. Each model offers a unique approach to summarizing text documents and generating concise and informative headlines.

## Models Description

### T5 Model

The T5 model utilizes the transformer architecture to generate summaries of text documents. It compares the effectiveness of its generated summaries with those produced by another summarization technique (Sumy's LSA summarizer). The evaluation metric used is the ROUGE score, which assesses the overlap of content between the generated summaries and reference summaries.

### LDA Model

The LDA (Latent Dirichlet Allocation) model takes an article and treats its sentences as documents. It then performs topic modelling on these sentences to extract topics. Using the topic weight matrix, the model calculates dominant topics, from which a subset is selected. For each topic, the model identifies multiple sentences belonging to it. Finally, to generate a headline, the model selects one sentence per topic and concatenates them.

### LSTM Model

The LSTM (Long Short-Term Memory) model is trained on articles as input and highlights as targets. It generates headlines using beam search. LSTM is adept at capturing long-term dependencies within text, making it suitable for understanding complex article contexts and distilling them into headlines.

## Evaluation

Each model's performance is evaluated using appropriate metrics:
- **T5 Model**: ROUGE score for comparing generated and reference summaries.
- **LDA Model**: Evaluation based on the coherence and relevance of generated headlines.
- **LSTM Model**: Assessment of headline quality based on relevance and conciseness.


## Credits

- T5 model implementation adapted from [Hugging Face Transformers](https://huggingface.co/transformers/).
- LDA model implementation inspired by [Gensim](https://radimrehurek.com/gensim/index.html).
- LSTM model implementation built with [TensorFlow](https://www.tensorflow.org/).

## Contribution

The project was executed in the presence of each member being physically available at the time of the execution. Each member provided his value inputs for a given problem and the best approach was finalized after discussion among all the members.

## Team Members:
1. Arsh Jindal - 202103021
2. Aditya Tanna - 202103023
3. Vedant Pandya - 202101063
