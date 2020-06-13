# Support Vector Machine

1. SVM : used for classification problem
2. Margin: is the distance from the threshold(hyperplan for multidimentional data) to the nearest point of two class.
3. Maximum Margin Classfifier(MMC): is the classfier that use a threshold that maximize the magin.
4. MMC work well if the data has no outlier or no the data between two class are overlapped. In constrast,it is **_sensitive to outlier_** it is a pretty bad classifier when the previous case happen. It classifer the training data perfectly (low bias) but has high variance. So, instead of using MMC,we use **Soft Magin Classifer(SMC)**.
5. SoftMargin
6. SMC allows misclassification while trainig, so it does not maximize the margin but roburst to outlier => higher bias but lower variance (advantageof SMC).
7. Soft Margin classifier = Support Vector Classifier
8. Limitation of SMC:
   1. it is a linear classifier => does not classfiy well when the data is **_not linearly seperable_**.
9. SVM = SVC + kernel_function
10. kernel_function map the features to a high dimensional space to make them linearly semperable.
11. Populer kernel function in SVM:
    1. Polynomial kernel (d: degree of the polynomial, finite dimension)
    2. Radial Basis Function kernel (RBF)
       1. find SVC in **_infinite dimension_**
12. How SVM choose d for Polynomial kernel:
    1. by increasing d: 1,2,3,.. and choosing d by **cross validation**.
13. Kernel function only calculate the relationships between every pair of points _as if_ they are in the dimension; they don't _actually_ do the transformation.This **trick** calculate the high-dimensional relationships without acutally transofmring the data to the higher dimension. It is call **The Kernel Trick**.
14. Kernel trick:
    1. **reduce amount of computation**: by avoiding the math the transform the data from low to high dimensison
    2. **make calculating relationships in the infinite dimensions used by the RBF possible**.
