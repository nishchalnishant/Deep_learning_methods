## Language models

- language model learns to predict the probability of a sequence of words.

- There are primarily two types of Language Models:

- Statistical Language Models: These models use traditional statistical techniques like N-grams, Hidden Markov Models (HMM) and certain linguistic rules to learn the probability distribution of words

- Neural Language Models: These are new players in the NLP town and have surpassed the statistical language models in their effectiveness. They use different kinds of Neural Networks to model language

- Transformers -- 2017
- Bert -- 2018
- Elmo -- 2018
- Gpt --2018
- Roberta -- 2019
- Gpt 2 -- 2019
- Albert --2019
- Gpt -3 -- 2020

## Word embeddings

- Learned representation for text where words that have the same meaning have a similar representation.

- Word embeddings are a class techniques where individual words are represented as real valued vectors in a predefined vector space .

- Each word is mapped to one vector and the vector values are learned in a way that resembles a neural network and hence the technique is often lumped into the field of deep learning.

- Embedding layer
- Cbow word2vec -- 2013
- Glove -- 2014
- Fast text -- 2016
- Elmo -- 2018

## Tokenizers

- A tokenizer receives a stream of characters, breaks it up into individual tokens (usually individual words), and outputs a stream of tokens.

- wordPiece -- 2016
- SentencePiece -- 2018

# Attention

- In psychology, attention is the cognitive process of selectively concentrating on one or a few things while ignoring others.

- A neural network is considered to be an effort to mimic human brain actions in a simplified manner. Attention Mechanism is also an attempt to implement the same action of selectively concentrating on a few relevant things, while ignoring others in deep neural networks.

# Transformers

- Transformers are a type of neural network architecture that have several properties that make them effective for modeling data with long-range dependencies.
- They generally feature a combination of multi-headed attention mechanisms, residual connections, layer normalization, feedforward connections, and positional embedidngs.
- The Transformer was proposed in the paper Attention Is All You Need.
