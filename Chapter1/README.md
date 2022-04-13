# Chapter 1

1. **Machine Learning** is the science to design and make programs that have the ability to learn from data. This systems can learn without being explicitly programmed.

2. Four types of problems where Machine Learning shines:
    * Classifying types of flowers or plants.
    * Predicting the stock prices (regression).
    * Make an app that recognizes voices.
    * Mailing spam filter.
    
3. A **labeled training set** is the data used for training the model, which has predefined *labels* (solutions). Each instance has the solution, called *label*. This is used in **Supervised learning**.

4. The two most common supervised tasks are *classification* (spam filter) and *regression* (predict a target numeric value).

5. Unsupervised tasks (unlabeled data):
    * Clustering.
    * Anomaly detection and novelty detection.
    * Visualization and dimensionality reduction.
    * Assosiation rule learning.
    
6. **Reinforcement learning**.

7. A *clustering* algorithm can be used to segment users/customers into multiple groups.

8. Spam detection problem is a *supervised* learning problem, since the training set is *labeled* (each feature is labeled as *spam* or *not spam*). It is a *classification* task.

9. In an online learning system the training can be done sequentially when new data is available, without the need to run all the data from scratch. It can learn *incrementally*.

10. Out-of-core learning is done when the dataset is too big, or cannot fit in the machine's memory. The algorithm loads part of the data, runs a training step on that data, and repeats until the whole data is processed.

11. **Instance-based learning** relies on a *similarity measure*. It learns the training data by heart.

12. An algorithm's hyperparameter controlls the amount of regularization to apply during learning. Unlike a model's parameter, the hyperparameter is a parameter of a learning algorithm, and not of the model.

13. Model-based learning algorithms search for a set of parameters belonging to a specific model. For example, if we are working with a linear model, we have two parameters (slope and intercept). They use a **performance measure** to know which values of the parameters perform best. The predictions are made using (applying) the model function with the new values.

14. Challenges of Machine Learning:
    * Insufficient quantity of training data
    * Nonrepresentative training data
    * Poor-quality data
    * Irrelevant features
    * Overfitting and Underfitting
    
15. When the model performs great on the training data but generalizes poorly to new instances, this is called **overfitting**. One solution is to reduce the number of parameters of the model. Another solution is to gather more training data if possible. A third possible solution is to reduce the noise in the training data (remove outliers, etc).

16. A **test set** is the data used to test the model. When training the model, the test set is not included. This is useful in order to know how well the model will generalize to new cases.

17. The **validation set** is commonly used because if not, the generalization error is measured multiple times on the test set. Hold out part of the training set. This set is used to compare models.

18. The **train-dev set** is used in *data mismatch* cases. The model is trained in the *training* set, and then it is evaluated in the *train-dev* set. If it performs well, then the model is not overfitting. If it performs poorly on the validation set, the problem may be data mismatch.

19. If the hyperparameters are tuned using the test set, the model is improved for that particular set, and it may not generalize well on production (new data).