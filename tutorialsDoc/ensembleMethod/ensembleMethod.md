# Ensemble Method

1. Ensemble methods is a machine learning technique that combines several base models in order to produce one optimal/more robust/ more accurate predictive model.
2. The idea of ensemble methods is to try reducing \*_bias and/or variance_ of such weak learners by combining several of them together in order to create a strong learner (or ensemble model) that achieves better performances. Each base model could has high variance or hight baias (tradeoff).
3. Type of ensemble methods:
   - **BAGGing, or Bootstrap AGGregating**
   - Random Forest (can be considered as BAGGing): random Forest models decide where to split based on a random selection of features
4. Rather than making one model and hoping this model is the best/most accurate predictor we can make, ensemble methods take a myriad of models into account, and average those models to produce one final model.
5. Some well-known notions:
   - bootstraping
   - bagging
   - random forest
   - boosting : adaptive boosting, gradient boosting
   - stacking
6. ensemble model is:
   - homogenous: the combination of the same base model (weak learner)
   - heterogenous: the combination of differnt wek learners
7. Choice of aggreation methods:
   - if base model has low bias and high variance => the aggreation method shoud be the one who tend to **_reduce the variance_**
   - else: => the aggreation method shoud be the one who tend to **_reduce the bias_**
8. Bagging, boosting and stacking

   - **bagging**:that often considers homogeneous weak learners, learns them independently from each other **in parallel** and combines them following some kind of deterministic averaging process.

   - **boosting**: that often considers homogeneous weak learners, learns them sequentially in a very adaptative way (a base model depends on the previous ones) and combines them following a deterministic strategy

   - **stacking**: that often considers heterogeneous weak learners, learns them in parallel and combines them by training a meta-model to output a prediction based on the different weak models predictions

9. **Bootstraping**:statistical technique consists in generating samples of size B (called bootstrap samples) from an initial dataset of size N by randomly drawing with replacement B .

10. Bootstrap sample are approximately i.i.d:
    - approximately representative
    - approximately independent
11. Aggregation methods:
    - regression: by averaging
    - classification: by voting
      - hard voting: the most vote win
      - soft voting: average the probability

[TODO]

- finish the reading in the reference

# **Reference**

1. https://towardsdatascience.com/ensemble-methods-bagging-boosting-and-stacking-c9214a10a205
