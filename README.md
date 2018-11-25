# NTM
I'm curious to see how various programming control flows and operations (like indexing, loops, recursion) translate to the continuous space and how could we develop NTMs: **Neural Turing Machines** to this end.

Ian Goodfellow describes [Deep Learning](https://www.deeplearningbook.org/) as a sequence of steps in a learned algorithm. Each layer acts on the input from the next. Some weights are such that they let you add combine inputs (arithmetic operations + and \*). Others are such that they let you condition (if else), by having thresholds and activations. Some constants are maintained (literals) by having bias terms. **Looping** (for, not while) was hard to come by until RNNs emerged. Memory is needed (**global variables**) so LSTMs and memory augmented networks. For **recursion** as a means to bypass the while loop, you go for Recursive Neural Networks (TreeNN). Recently, **indexing** seems important, i.e. don't just store variables but also store and operate on indexes that you need, eg. in calculating longest increasing subsequence in an array, you need to store which i (index) was last decreasing one. So herein comes attention methods that tell you what position to focus on positions, not which values.
We're basically just giving it tools to let it come up with an algorithm by itself. Eg. the way I achieved 100% accuracy on a counting problem by using RNNs and just 4 parameters.

I'm talking about supervised learning btw.  For unsupervised models like autoencoder, GANs, word2vec, etc. those are just model hacks to help you figure out what representation you need. Computer programs don't just take some input, do operations on it and keep it to themselves. They return something (either by value or by reference). There do exist better representations that you need in computer programs as well, eg. sorted version of an array, a hash map, a linked list from an array, a queue or stack, a graph from an adjacency matrix, and so on. 

A close line of work is the Neural Turing Machines by [Graves et al. 2014](https://arxiv.org/pdf/1410.5401v2.pdf).
