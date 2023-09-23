# Decision Tree
is a popular machine learning algorithm used for both classification and regression tasks. It is a supervised learning algorithm that can be used for various types of data analysis and decision-making processes. Decision trees are particularly valuable for their simplicity, interpretability, and versatility.

![image](https://cdn-cashy-static-assets.lucidchart.com/lucidspark/marketing/blog/2020Q4/decision-tree/Decision-tree.png)


# what are the disadvantages of decision tree ?
1- **Overfitting:** Decision trees are prone to overfitting, especially when the tree is deep and captures noise or specific patterns in the training data that may not generalize well to new, unseen data.


2-**Instability:** Decision trees can be sensitive to small variations in the training data. A slight change in the data can result in a completely different tree structure, leading to instability in the model.


# how measure impurity in classification ?
Classification Impurity Measures are :

1- **Gini Impurity (Gini Index):** The Gini impurity measures the probability of misclassifying a randomly chosen element if it were randomly classified based on the distribution of class labels in the node. It ranges from 0 (pure, all elements belong to one class) to 0.5 (impure, equal distribution among classes).

2- **Entropy:** Entropy measures the level of disorder or impurity in a node. It is based on the information theory concept and is used to quantify the uncertainty associated with the class labels. Lower entropy values indicate purer nodes.

![image](https://aiplanet.com/blog/wp-content/uploads/2021/04/Entropy_3.png)


Entropy(D) = -∑(p_i * log2(p_i))


# How measures impurity in regression ?

Variance Impurity Measure

# How to solve the problem of Overfitting ?
Pruning involves removing some branches of the tree that do not contribute significantly to improving its performance on the validation or test data.

# what are the types of pruning ?
1- **pre-pruning :** is a technique used in decision tree construction to prevent the tree from becoming overly complex and overfitting the training data. Unlike post-pruning (pruning after the tree is fully grown), pre-pruning involves setting stopping criteria during the tree-building process.

2-**post-pruning :** is a technique used in decision tree construction to reduce overfitting after the tree has been fully grown

# what are stopping criteria in pre-pruning ?

1- Max Depth 

2-min_sample_leaf

3-min_sample split

4- Minumun information gain

# what are stopping criteria in post-pruning ?

1- cost complexity pruning (cpp_alpha) : make balance between performance in training and validation 




