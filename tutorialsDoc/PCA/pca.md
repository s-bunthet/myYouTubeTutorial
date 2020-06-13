# Principle Component Analysis

- It is a dimensionality reduction technique.
- PCA find `n` new features (principle components) out of `n` initial features.
- The first component that PCA finds stores the most information(the largest variance) in decreasing level until the last component.
- A principle component = eigence vector of the covariance matrice
- The eigence vector correspond to the largest eigence value of the covariance matrix is the first component, and so on.
- An eigence value of the covariance matrix is proportional to the information that the correspond eigence vector contains.
- Covarriance matrix mesure the correlation between axis (features)
  - positive: correlated
  - negative: not correlated
- we want to keep or find the uncorrelated axis since correlated axis or features give redundant information.
- why large variance = much information? => let imagine a 2D data point that has the same `y` but different `x`. Effectively, the `y` axis can be neglected, only the `x` axis contains the information. We can reason it by seeing that the projection of the points on `y` axis is a point, so has `0` variance. So `compared` to `x` axis, `y` axis does not hold any information.
- How many components to keep? => For each component, we calculate the "information" that it held by deviding the correspoding `eigence value` to the `sum of all eigence value`. For example, if we have 10 component and the first 4 components held already 95% of the information, so we might neglect the 6 remaining component.
- How to project the original data to the new features (components)? => by the matrix mulplication between the data matrix and the new feature matrix (linear projection). The exact formulation is to be discovered by yourself or look on the Internet.

---

- **Note**: before working on the PCA, we need to first standardize the data (transform them to the same scale) so that we can compare the variance correctly (in the same scale).
