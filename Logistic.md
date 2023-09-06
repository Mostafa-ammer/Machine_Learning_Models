# Logistic Regression Model 

Logistic regression is a fundamental and widely used statistical technique in machine learning and statistics for binary and multi-class classification problems. Despite its name, it is a classification algorithm, not a regression algorithm. Logistic regression models the probability that a given input belongs to a particular category or class. It is particularly useful when you need to predict the probability of an event occurring, such as whether an email is spam or not, whether a customer will make a purchase, or whether a patient has a particular medical condition.

# How get sigmoid from Odds 

In logistic regression, we model the odds of an event occurring. The odds of an event happening is defined as the ratio of the probability of the event occurring to the probability of it not occurring. Mathematically, the odds (OR) can be expressed as:

                                                              Odds= P(event)/1−P(event)
                                                                        

To model the relationship between the input features and the log-odds, logistic regression applies a logit transformation. The logit transformation takes the natural logarithm (base e) of the odds
​
                                                             logit(P(event))=ln( P(event) /1−P(event))



 
