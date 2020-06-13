# Information Theory

1. Information Theory:
   1. quantify how much information is presented in a signal.
   2. characterize probability distribution
   3. quantify similarity between distributions
2. Intuition about information theory:
   1. likely event should have low information content than less likely event.
   2. Independent events should have additive infromation
3. Information Content
4. self information of an event $X=x$ is $I(x)=-\log{P(x)}$. The unit of $I(x)$ is **nats**
5. One **nat** is the amount of information gained by **observing** an event of probability of $\frac{1}{e}$. Others use the base $2$ logarithms and the units is called "**bit**" or "**shanon**". Information mesures in **_bit_** is just the rescaling of that mesured in **_nat_**.
6. **Self Information** deals only with **_single_** outcome.
7. We can quantify the amount of uncertainty in an entire probability distribution using the _**Shannon entropy**_ : $H(X)=H(P)=\mathop{\mathbb{E}}_{X\sim P}[I(x)]=-\mathop{\mathbb{E}}_{X\sim P}[\log{P(x)}]$.
8. The Shannon entropy of a distribution is the expected amount of information in an event drawn from that distribution. It gives a lower bound on the number of bits (if the logarithm is base 2, otherwise the units are different) needed on average to encode symbols drawn from a distribution P.
9. When $x$ is continuous, the Shannon entropy is known as the **differential entropy**.
10. We can mesure how different two distributions using **Kullback-Leibler(KL) divergence**: $D_{KL}(P||Q)=\mathop{\mathbb{E}}_{X\sim P}[\log{\frac{P(x)}{Q(x)}}]=\mathop{\mathbb{E}}_{X\sim P}[\log{P(x)}-\log{Q(x)}]$.
11. Adjective to describe the similarity between two distributions:
    1. same (discret random variable)
    2. same almost everywhere (continue random variable)
12. Property of KL divergence:
    1. non-negative
    2. non-symmetric : $D_{KL}(P||Q) \neq D_{KL}(Q||P)$
13. Since KL divergence mesures the similarity between distribution, so it is kind of **distance**. Howevery it is not because it is asymetric.
14. **Cross-entropy**: $H(P,Q) = H(P)+D_{KL}(Q||P)=-\mathop{\mathbb{E}}_{X\sim P}\log{Q(x)}$
