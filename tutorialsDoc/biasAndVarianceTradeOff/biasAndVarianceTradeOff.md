# Bias and Variance Tradeoff

Goal is to describe the bias-variance tradeoff in a friendly way without much mathematically speaking.
I will explain mathematically in the next tutorial.

1. terminalogy
   1. tradeoff
   2. bias
   3. variance
   4. overfited
   5. underfitted
   6. fit
   7. regression-> fiting a model to the data
   8. what is statistical model? => friendly speaking is to find the relation between the data(something that you observe) and the objetive (what you want to infer ontop of those observation)
   9. training and testing dataset when doing machine learning
2. How to choose the training data?
3. Quick overview of machine learning aproach vs tranditional programing aproach
4. In machine learning, you always come accros the term bias-variance tradeoff. The are many explaination more or less mathematically speaking.
5. the attention or the performance of the model to the data while :
   1. training
   2. testing
6. what is the process of machine learning?
   1. collect the data, preprocess it and shuffle it
   2. split the data into test and train set
   3. train the model with the training data
      1. it is the job of the algorithm to do something. For example in regression problem, the algorithm try to find the model(estimate the parametors in case of the parametrics model)
   4. test the model with the testing data
7. How to define a good model? the model that perform well with the testing data.
   1. performance metric
      1. error (ex. MSE for regression)
      2. score (ex. in RL)
   2. we assume that the training and testing data come from the same distribution.
8. Simplicity of a model
   1. simple model (to the data on which it is trained) : too simple => can not capture the underlying trend or structure of the data.
   2. complex model (to the data on which it is trained)
9. Simple or complex model is depend on the data
10. Why test the model? => to check if the model can be generalized to the unseen data.
11. relationship between the obervation and inference, but we don't know the relation. We use machine learning algorithm to approximate that relationship(mathematical realtionship).
12. bias: the inability of the machine learning model to capture the true relationship of the training data.
13. variance: the inability of the machine learning model to capture the true relationship of the testing data(for generalization).
14. It is hard to tell how the overfited model also well perform with future detaset. It might do well sometimes and other time it mights do teribly.
15. We can control wheather a model is more likely to overfitted or underfitted by altering its **capacity**. Model with low capacity may struggle to fit the training data. Models with high capacity can overfit by **memorizing properties** of the training set that do not serve them well on the test set.
16. The capacity of a model is not only by the choice of the model but also the learning algorithm.
17. **Learning algorithm**:" A computer program is said to **learn** from experience E with respect to some class of tasks T and performance measure P, if its performance at tasks in T, as measured by P,improves with experience E."
18. Training Error vs Generalization error
19. The central challenge in machine learning is that we must perform well on new, previously unseen inputs—not just those on which our model was trained. The ability to perform well on previously unobserved inputs is called generalization.
20.
