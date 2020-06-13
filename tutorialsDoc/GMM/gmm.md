# Gaussian Mixture Model(GMM) 
1. Characteristic of claustering model:
   1. hard clustering method
      1. **_ex_**: K-Means
   2. soft clustering method
      1. **_ex_**: GMM
2. **Gaussian Mixture**: is function that is comprised of serveral Gaussians.Each gaussian has it oun mean anc covariance matrix.The number of Gaussian is equal to the number of clausters($K$). 
3. **Mixing probability$\pi$**: define how big or small the Gaussian function will be. **$\sum_{k=1}^{K} \pi_{k}=1$**.
4. $TheClausterOfANewData =arcmax_{k} \pi_{k}$.
5. The goal is to find the parameters of each Gaussian: $\mu$ and $\sigma$. We find them by MLE(Maximum Loglikihood Estimates) method.  
6. Probability of a data point $x_{n}$ comes from Gaussian k: $p(z_{nk=1|x_{n}})$. $z$ is a **_latent variable_**(the notion come from hidden markov model).
7. $\pi_{k}$ = p(z_{k}=1)
8. $z=\{z_{1},z_{2},z_{3},...,z_{K}\}$. Each $z$ is independent=> $p(z)=\prod_{k=1}^{K} p(z_k=1)^{z_{k}} = \prod_{k=1}^{K} \pi_{k}^{z_{k}}$.
9. **Gaussian Mixture**: $p(x_{n})=\sum_{k=1}^{K}p(x_{n}|z)p(z) = \sum_{k=1}^{K} \pi_{k}\mathcal{N}(x_{n}|\mu_{k},\sum_{k})$.
10. **Likelihood of the model**: $p(X)= \prod_{n=1}^{N}p(x_{n}) = \prod_{n=1}^{N}\sum_{k=1}^{K}\pi_{k}\mathcal{N}(x_{n}|\mu_{k},\sum_{k})$ 