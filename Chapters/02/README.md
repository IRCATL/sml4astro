# Chapter 02 : Bayesian Inference
This chapter introduces the fundamental probability theory underlying Bayesian inference, laying the groundwork for developing machine learning methods that rigorously quantify and reason about uncertainty in astronomical data analysis.

### Why Bayesian Inference ?
A central insight from Thomas Bayes — one that revolutionized statistical thinking — was that ***both observations and model parameters should be treated as random variables***. This perspective, which we’ll explore in depth, forms the mathematical basis for all subsequent chapters.
While treating observational data as random variables seems intuitive (our measurements always have uncertainty), extending this treatment to model parameters might initially seem counterintuitive.
After all, physical constants like the gravitational constant or the mass of a galaxy should have definite values. ***Yet our knowledge of these values is inherently uncertain, and Bayesian inference provides a mathematically consistent framework for updating this knowledge as we gather more observations***.

This Bayesian perspective is particularly valuable in astronomy, where many phenomena cannot be repeated under controlled conditions. Unlike laboratory experiments where 0we can run multiple trials, astronomers often study unique events. By treating model parameters as random variables, Bayesian inference allows us to make principled statements about uncertainty even when we have limited data.

Why ***methods from linear regression to neural networks can all be understood as extensions of Bayesian principles*** ? Each technique, in its own way, implements ***the core Bayesian idea of updating our beliefs about model parameters based on observed data***. Understanding this connection provides not just practical tools for data analysis but also a deeper appreciation for how machine learning methods relate to the principles of scientific inference.

### Deterministic vs Random Variables : A Key Distinction, but Why ?
We’ll start by distinguishing between deterministic and random variables — ***a distinction that clarifies why treating model parameters as random variables makes sense***. To understand why scientific inference requires a probabilistic approach, we must first distinguish between these two different types of quantities :
* **Deterministic Variables :** are quantities that, given the same conditions, always yield the same value. For example, the orbital period of a planet around a star of known mass at a known distance follows deterministic physical laws.
* **Random Variables :** in contrast, are quantities whose values are subject to uncertainty or variation. Even when all known conditions are specified, we can only predict probabilities of different outcomes, not the exact outcome itself. In real astronomical observations, even though the true orbital period of a planet is a deterministic quantity, our measurement of it becomes a random variable. When we measure that orbital period $P$ ,we make multiple observations of the star’s radial velocity or the planet’s transit, and each measurement has some uncertainty due to instrumental noise and atmospheric effects. Our final estimate of $P$ comes with an uncertainty, often expressed as $P ± σ_P$. Random variables come in two main forms :
   * **Inherently Random :** Some quantities in nature appear to be fundamentally probabilistic, such as quantum phenomena. Examples include :
      * The exact time of decay of a radioactive atom
      * The spin measurement of an electron in a superposition state
   * **Incomplete Knowledge or Measurement Uncertainty :** Many astronomical quantities appear random not because they are inherently probabilistic, but due to practical limitations.

We represent this uncertainty through a probability distribution that reflects our current state of knowledge. As we gather more data, this distribution will narrow, becoming more concentrated around the true value, but some uncertainty will always remain.

[till 2.2]
