# AdaBoost

1. AdaBoost is commonly used in decision tree and decision forest.
2. In random forest, some trees might be bigger that others, but there is no predetermined maximum depth. In constrast, in a **Forest of Trees** made with **AdaBoost**, the trees are usually just a **node** and two **leaves** (**stump**).
3. Stump is not great at making decision (weak learner), but its combination using AdaBoost could make a powerfull classifier.
4. In a **Random Forest**, each tree has an equal vote on the final classification. With the **Forest of Stumps** made with AdaBoost, some stumps get more **say** in the final classification than others.
5. In a **Random Forest**, each decision tree is made independtly of the others(great for parallel training). In contrast, in a **Forest of Stumps** made with **AdaBoost**, order is important. The **errors** that the first stumps make influence **how the second stumps is made.**
6. **Amount of say**:$Amount of Say = \frac{1}{2}\log(\frac{1-Total Error}{Total Error})$

7. **New Sample Weight**:
   1. For all correctly classified samples (increasing the sample size): $NewSampleWeight=(SampleWeight)\exp(AmountOfSay)$
   2. For all uncorrectly classified samples (decreasing the sample size): $NewSampleWeight=(SampleWeight)\exp(-AmountOfSay)$
8. After finding the newSampleWeights, we normalize them, and we create a new dataset by randomly selected(sample random number between 0 and 1) based on the sample weights.The sample with greater weight has more chance to be selected for the next stumps.
9. Three ideas behind AdaBoost:
   1. AdaBoost combines a lot of **weak learners** to make classification. The weak learners are almost always **stumps**.
   2. Some **stumps** get more "say" in teh classification than others.
   3. Each **stump** is made by taking the previous stump's mistakes into account.
10. If we have a **Weighted Gini Function** then we use it with the **Sample Weights**, otherwise we use the **Sample Weights** to make a new dataset that reflects those weights.
