# Greek BERT model for Text Classification downstream task

This repository contains Colaboratory notebooks where you can observe the use of the BERT model for Text classification.

## What is BERT?

BERT is a method of pre-training language representations, meaning that we train a general-purpose "language understanding" model on a large text corpus (like Wikipedia), and then use that model for downstream NLP tasks that we care about (like text classification). BERT outperforms previous methods because it is the first unsupervised, deeply bidirectional system for pre-training NLP.

Unsupervised means that BERT was trained using only a plain text corpus, which is important because an enormous amount of plain text data is publicly available on the web in many languages.

BERT was built upon recent work in pre-training contextual representations. Contextual models generate a representation of each word that is based on the other words in the sentence. For example, in the sentence `I made a bank deposit` BERT represents "bank" using both its left and right context — `I made a ... deposit` — starting from the very bottom of a deep neural network, so it is deeply bidirectional. BERT uses a simple approach for this: We mask out 15% of the words in the input, run the entire sequence through a deep bidirectional [Transformer encoder](https://arxiv.org/abs/1706.03762), and then predict only the masked words.


