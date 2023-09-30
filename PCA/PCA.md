## Dimensionality Reduction: Principal Component Analysis
![image](https://miro.medium.com/v2/resize:fit:1400/1*T7CqlFV5aRm6MxO5nJt7Qw.gif)

 # what is PCA ?

PCA is a linear dimensionality reduction technique which converts a set of correlated features in the high dimensional space into a series of uncorrelated features in the low dimensional space , These uncorrelated features are also called principal components

#  How PCA works ?

It transforms the data in such a way that the first component tries to explain maximum variance from the original data

# PCA is Supervised or Unsupervised Machine Learning Model ?

It is an unsupervised algorithm i.e. it does not take into consideration the class labels.

Describe Two Cases : 

**Case 1**

![image](https://miro.medium.com/v2/resize:fit:1100/format:webp/1*0zaNT5b09jGpIPCeciYw0w.png)

The above figure shows two features F1 and F2 plotted in a two-dimensional space. As we can see from the plot above, the variance on feature F2 is much higher than the variance on feature F1 which means


**Result** : 
we need to drop one feature. We know that feature F1 preserves much less information than F2, so we can safely drop feature F1 and use feature F2 as our final feature without using "PCA"


**Case 2**

![image](https://miro.medium.com/v2/resize:fit:1100/format:webp/1*FOboyOo3_ALuBJ2GSWR4mA.png)

Here, the variance on feature F2 is equal to the variance on feature F1 which means

**Information preserved by F2 = information preserved by F1**

**Result : **

now if we want to reduce the dimensions of the data from 2D to 1D we cannot drop one feature as we lose a lot of information.

Now : PCA performs linear orthogonal transformation on the data to find features F1’ and F2’ such that the variance on F1’ >> variance on F2’.


# What does linear orthogonal transformation mean?

To find these new features, all PCA does is, rotate the original axes in such a way that we get maximum spread (variance) on the new axes after projecting the data points on them. These new axes are a linear combination of the original axes and they are always perpendicular to each other.

These new sets of features are called principal components. Here, F1’ is the first principal component which gives the direction of maximum variance, and F2' is the second principal component which gives the second direction with most variance. F1’ and F2’ are unit vectors and they are perpendicular to each other. Since F1’ and F2’ are our new set of features we can safely drop F2’ as F1’ preserves maximum information.

![image](https://miro.medium.com/v2/resize:fit:1198/format:webp/1*T-X74b1jeCrJooXaS9lmYQ.png)

![image](https://miro.medium.com/v2/resize:fit:1100/format:webp/1*lfOCE9OIGEREJ9VHf_bQMg.png)
