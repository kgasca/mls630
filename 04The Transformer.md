---
aliases:
topic:
tags:
  - idea
date: 2026-05-01
subset:
---
# The Transformer

Scientists wanted to understand each word in relation to the words around it. In a field that boils down to binary thinking, understanding patterns and word order makes sense. They approached such translation tasks using recurrent [[neural networks]] and mechanisms of attention. 

Traditionally, for these types of computational tasks, most scientists used recurrent neural networks in conjunction with various types of attention mechanisms. A recurrent (or convolutional) network routes each packet of information from one hop to the next hop sequentially. Attention mechanisms review three specific components in an object (for example a sentence) to compute a weighted sum based on relevance of the word compared to the words surrounding it. With the previous models, an entire sentence would have to be processed before an evaluation could be made. This mechanism was made possible by the use of Long Short-Term memory (LSTM) a mechanism which acted like a repeater (amplifier) for a sentence so that the system could keep the entire sentence in memory and then decide what to do with the data. This made a very compute heavy process.

The authors of "Attention is All You Need" introduce an entirely new approach to solving language modeling and machine translation problems - specifically English-to-German and English-to-French translation tasks. They named this new network architecture model *the transformer*. 

The authors used a mechanism called self-attention where each word (symbol) was evaluated individually in relation to every other word around it. The word was processed through a single attention layer (head) which worked in parallel with other layers (multi-head attention). This solution reduced the amount of compute needed and decreased the training time. This model unlocked the true potential of [[large language models]] (LLMs). These models generate content by accurately predicting the next word in a sequence. This architecture is still one of the most heavily used for the popular tools we use today such as ChatGPT and Claude.



