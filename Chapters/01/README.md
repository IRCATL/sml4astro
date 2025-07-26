# Chapter 01 : Preface and Overview
This chapter provides an introduction to the book’s goals, scope, and the importance of statistical machine learning in modern astronomy, setting the stage for the concepts and methods discussed in later chapters.

## Notes
Researchers often learn specific techniques for particular prob-
lems — ```clustering for galaxy classification```, ```regression for stellar parameter estimation```, or ```neural networks for image analysis``` — without understanding the underlying statistical principles that connect these methods. This piecemeal approach not only limits the effective application of these techniques but also perpetuates the perception that machine learning is merely a collection of tools without theoretical depth like physics provides.

Every machine learning method incorporates what we call inductive bias — the set of assumptions that guide learning when data alone is insufficient to determine a unique solution. When we perform linear regression, we assume relationships follow hyperplanes. When we choose kernel functions for Gaussian Processes, we encode beliefs about function smoothness. When we design convolutional neural network architectures, we assume translation invariance in images. These biases are not limitations but necessities: without them,learning from finite data would be impossible.

Practical tutorials were released on [GitHub](https://github.com/tingyuansen/statml)

**Machine Learning** is best understood as an extension of statistical inference rather than as a separate discipline.

**Supervised Learning** involves mapping inputs to known outputs, learning relationships between variables when we have examples of both.

**Unsupervised Learning** seeks to find patterns in data without known target outputs, discovering hidden structure rather than learning input-output relationships.

The transition to computational methods (Chapters 12-13) acknowledges that as models become more complex, analytical solutions become unavailable and **sampling methods become necessary** (Monte Carlo methods and Markov Chain Monte Carlo).

Without understanding the theoretical foundations, it becomes impossible to evaluate when methods are appropriate, how they might fail, or how they connect to the broader framework of statistical inference.

The connection between **Principal Component Analysis and autoencoders** shows how neural networks can extend classical dimension reduction techniques. These connections help readers develop intuition about when different approaches might be appropriate.

At the mathematical level, you will be comfortable with the derivations and analysis of key algorithms. This includes understanding **how maximum likelihood estimation leads to specific loss functions**, **how regularization emerges from Bayesian priors**, and **how optimization algorithms like expectation-maximization provide practical solutions to complex inference problems**.

The future of astronomical research will undoubtedly involve increasingly sophisticated statistical techniques applied to increasingly complex datasets. Success in this environment will require not just familiarity with specific algorithms but the kind of deep statistical understanding that enables rapid adaptation to new challenges and opportunities.

