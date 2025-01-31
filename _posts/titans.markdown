---
layout: post
title:  "Titans: Learning to Memorize at Test Time"
categories: blog
tags: arxiv whitepaper ai rnn transformers
---
A recently published (whitepaper)[https://arxiv.org/abs/2501.00663] from Google Research introduces Titans, a Transformer-based architecture distinguished from its predecessors by the implementation of a neural long-term memory module.

In general, neural networks are loosely based on the neuroscience of the human brain. Research on neural networks spans almost eighty years, enduring periods of dismissal and revival. In particular, "deep learning," galvanized by improvements in computing and the explosive proliferation of digital data, has enjoyed a contemporary renewal.  GANs (generative adversarial networks), diffusion models, and LLMs (large language models), which power mainstream consumer products such as Stable Diffusion and ChatGPT, fall into this category.

Transformers are descendents of RNNs, or recurrent neural networks. Recurrent neural networks were the first to introduce the concept of working memory into their architecture, utilizing past input to modify current input at each time step. However, it quickly emerged that RNNs were plagued by a significant problem: availability bias.

The holy grail of artifical intelligence is to achieve AGI--artificial general intelligence. This type of intelligence would be indistiguishable from human intelligence. But human intelligence is fallible. Humans make use of heuristics and biases to optimize performance in time and computation.

LSTMs (long short-term memory) models attempted to address the "vanishing gradient" problem that emerged in RNNs by implementing a <i>longer</i> short-term memory. It achieved this by implementing "forget gates" at each unit, which added the crucial context of the relevance of new information.

What distinguishes Transformers from their contemporary counterparts is the concept of attention, memory, and forgetting--crucial components of human learning. 

Motivated by findings in neuropsychology<sup>[1]</sup>, the development of the neural long-term memory module is

In "The Myth of Artificial Intelligence"
