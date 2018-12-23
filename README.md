# NTM

Ian Goodfellow describes [Deep Learning](https://www.deeplearningbook.org/) as a sequence of steps in a learned algorithm. Each layer acts on the input from the next. I'm fascinated by this line of thought and like to imagine each machine learning model as a way to implement some *programming constructs*. Some weights are such that they let you combine inputs (**arithmetic operations** + and \*). Others are such that they let you **condition** (if else), by having thresholds and activations. Some **constants** are maintained (literals) by having bias terms. **Looping** (for, not while) was hard to come by until RNNs emerged. Memory is needed (**global variables**) so LSTMs and memory augmented networks emerged. For **recursion** as a means to bypass the while loop, you go for Recursive Neural Networks (TreeNN). Recently, **indexing** seems important, i.e. don't just store variables but also store and operate on indexes that you need. For example, in calculating longest increasing subsequence in an array, you need to store which *i* (index) was the last decreasing one. So herein come attention methods that tell you what positions to focus on, not which values.
We're basically just giving tools to our models and letting it come up with an algorithm by itself. As an instance of the same, I achieved 100% accuracy on a counting problem by using RNNs and just 4 parameters. Several constructs are yet to find an equivalent in machine learning terms, for example, the **break** keyword! 

P.S. I'm talking about supervised learning. Unsupervised models like autoencoder, GANs, word2vec, etc. are just model hacks to help you figure out what representation you need. Computer programs don't just take some input, do operations on it and keep it to themselves. They return something (either by value or by reference). That being said, there do exist better (read: *more efficient*) representations that you need in computer programs as well, eg. sorted version of an array, a hash map, a linked list from an array, a queue or stack, a graph from an adjacency matrix, and so on. 

A close line of work is the Neural Turing Machines by [Graves et al. 2014](https://arxiv.org/pdf/1410.5401v2.pdf).
