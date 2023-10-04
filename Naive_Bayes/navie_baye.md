#   Naive Bayes Algorithm


# What is the Naive Bayes Algorithm ?

It is a probabilistic machine learning model that is used for classification problems. The core of the classifier depends on the Bayes theorem with an assumption of independence among predictors. That means changing the value of a feature doesn’t change the value of another feature


# Why is it called Naive?

It is called Naive because of the assumption that 2 variables are independent when they may not be


#  What are concepts that Naive depend on ?

it is depend on Conditional probability and  Bayes’ theorem


#  What is Conditional probability ?

Conditional probability is defined as the likelihood of an event or outcome occurring, based on the occurrence of a previous event or outcome. Conditional probability is calculated by multiplying the probability of the preceding event by the updated probability of the succeeding, or conditional, event.


Mathematically, the conditional probability of event A given event B has already happened is given by:
![image](https://editor.analyticsvidhya.com/uploads/530437.1.png)

Mathematically Bayes’ theorem can be stated as: 

![image](https://editor.analyticsvidhya.com/uploads/947042.png)

- Basically, we are trying to find the probability of event A, given event B is true.

- Here P(B) is called prior probability which means it is the probability of an event before the evidence

- P(B|A) is called the posterior probability i.e., Probability of an event after the evidence is seen.

![image](https://editor.analyticsvidhya.com/uploads/374484.png)


#  What is Naive Bayes?

Bayes’ rule provides us with the formula for the probability of Y given some feature X. In real-world problems, we hardly find any case where there is only one feature.
When the features are independent, we can extend Bayes’ rule to what is called Naive Bayes which assumes that the features are independent that means changing the value of one feature doesn’t influence the values of other variables and this is why we call this algorithm “NAIVE”

![image](https://editor.analyticsvidhya.com/uploads/984945.png)

![image](https://editor.analyticsvidhya.com/uploads/244777.png)


# Examble about Naive Bayes with Discrete Data ?

![image]9https://editor.analyticsvidhya.com/uploads/615408.png)


Assumptions of Naive Bayes :

1-  All the variables are independent. That is if the animal is Dog that doesn’t mean that Size will be Medium

2- All the features have equal importance.


We should try to apply the Naive Bayes formula on the above dataset however before that, we need to do some precomputations on our dataset.

We need to find P(xi|yj) for each xi in X and each yj in Y. All these calculations have been demonstrated below:

![image](https://editor.analyticsvidhya.com/uploads/7674811.png)
!image](https://editor.analyticsvidhya.com/uploads/7612312.PNG)

** Now if we send our test data, suppose test = (Cow, Medium, Black)**

![image](https://editor.analyticsvidhya.com/uploads/3661813.png)
![image](https://editor.analyticsvidhya.com/uploads/9839014.png)
![image](https://editor.analyticsvidhya.com/uploads/3836615.png)
![image](https://editor.analyticsvidhya.com/uploads/7098816.png)
![image](https://editor.analyticsvidhya.com/uploads/4529317.png)



# What is Gaussian Naive Bayes ?

So far, we have discussed how to predict probabilities if the predictors take up discrete values. But what if they are continuous? For this, we need to make some more assumptions regarding the distribution of each feature. The different naive Bayes classifiers differ mainly by the assumptions they make regarding the distribution of P(xi | y). Here we’ll discuss Gaussian Naïve Bayes.

![image](https://editor.analyticsvidhya.com/uploads/4919118.png)






















