# What are Sensitivity and Specificity?

1- Sensitivity / True Positive Rate / Recall 

 Sensitivity tells us what proportion of the positive class got correctly classified.
![image](https://cdn.analyticsvidhya.com/wp-content/uploads/2020/06/sensitivity.gif)

2- Specificity / True Negative Rate

Specificity tells us what proportion of the negative class got correctly classified.
![image](https://cdn.analyticsvidhya.com/wp-content/uploads/2020/06/Specificity.gif)

3- False Positive Rate

FPR tells us what proportion of the negative class got incorrectly classified by the classifier.
![image](https://cdn.analyticsvidhya.com/wp-content/uploads/2020/06/FPR.gif)


# What is the AUC-ROC Curve?
is like a graph that shows how well a classification model performs. It helps us see how the model makes decisions at different levels of certainty. The curve has two lines: one for how often the model correctly identifies positive cases (true positives) and another for how often it mistakenly identifies negative cases as positive (false positives) .


 (ROC) curve is an evaluation metric for **binary classification problems**. It is a probability curve that plots the TPR against FPR at various threshold values and essentially separates the ‘signal’ from the ‘noise.’ In other words, it shows the performance of a classification model at all classification thresholds.

The Area Under the Curve (AUC) is the measure of the ability of a binary classifier to distinguish between classes and is used as a summary of the ROC curve.


- When AUC = 1, the classifier can correctly distinguish between all the Positive and the Negative class points

- the AUC had been 0, then the classifier would predict all Negatives as Positives and all Positives as Negatives.

- When 0.5<AUC<1, there is a high chance that the classifier will be able to distinguish the positive class values from the negative ones

 - When AUC=0.5, then the classifier is not able to distinguish between Positive and Negative class points



# How Does the AUC-ROC Curve Work?
a higher X-axis value indicates a higher number of False positives than True negatives. While a higher Y-axis value indicates a higher number of True positives than False negatives.

- the choice of the threshold depends on the ability to balance False positives and False negatives.
- 
![AUC-ROC-curve57453](https://github.com/Mostafa-ammer/Machine_Learning_Models/assets/73859325/c0e2a845-3589-4317-9608-b85a316b5d33)












