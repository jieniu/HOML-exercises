# Chapter 1: The machine Learning Landscape

1. How would you define Machine Learning?

   There are 3 kinds of concepts in ML：

   * Experience：it's about learning from the data.
   * Task: the main task is to predict the new event from the new data.
   * Performance: a method to evaluate the prediction result.

   Or there is another way to define the ML: It let the program to learn from the data.

2. Can you name four types of problems where it shines?

   1. email server knows which email is a spam.
   2. NLP: natural Language procession
   3. Recommandation system in a e-commerce website
   4. Let the computer to recognise handwriting

   answer from the book:

   1. solve the complex problems
   2. replace the long hand-tuned rules
   3. build system that can adapt the fluctuating enviorment
   4. help humans learn(data mining)

3. What is a labeled training set?

   In supervised machine learning algorithm, we need to feed the computer with feature data and the right answer (desired solutions), then it will be trained to output a model, after that we can use this model to predict new data.

4. What are the two most common supervised tasks?

   ~~training the model~~

   ~~testing the model~~

   ~~choose a model~~



   regression and classfication

5. Can you name four common unsupervised tasks?

   1. K-Means
   2. clustering
   3. dimensionality reduction: merge several features into one
   4. visualization
   5. anomaly detection

   another answer from the book:

   * association rule learning

6. What type of Machine Learning algorithm would you use to allow a robot to walk in various unknown terrains?

   1. Reinforcement Leaning

7. What type of algorithm would you use to segment your customers into multiple groups?

   1. unsupervised ML, like clustering. When you don't know how many groups are there.
   2. supervised learning: classification. When you know what groups you would like to have.

8. Would you frame the problem of spam detection as a supervised learning problem or an unsupervised learning problem?

   1. supervised learning: 

9. what is an online learning system?

   1. it can remain training data and update itself all the time .

   answer on the book:

   1. it can rapidly adapt new data
   2. it can train huge data

10. What is out-of-core learing?

    online learning also can be used to train huge data that can not  fit in one machine's main memory.

11. What type of learning algorithm relies on a similarity measure to make predictions?

    instance-based learning

12. What is the difference between a model parameter and a learning algorithm's hyperparameter?

    model parameter: ~~it's the attribute of the data~~ a learning algorithm tries to find optimal values for the model parameters, such that the model generalizes well to new instances.

    hyper parameter: it's the parameters of the algorithm, not the model. when the model has the overfitting problem, we need to use regularization method to solve the problem, and the hyper parameters are parameters of the regularization algorithm.

13. What do model-based learning algorithms search for? What is the most common strategy they use to succeed? How do they make predictions?

    Model based learning algorithms search for **an optimal value** for the model parameters for prediction tasks. The most common strategy they use to succeed is training from data, **use cost function to estimate how bad the model perform**. When we get the model parameters, then when we get new data instances, we plug the data feature into the model, and calculate the prediction.

14. Can you name four of the main challenges in Machine Learning?

    1. Insufficient Quantity of Training Data
    2. sampling bias, nonrepresentative training data
    3. overfitting
    4. underfitting
    5. poor-quality of data
    6. irrelevant features

15. If your model performs great on the training data but generalizes poorly to new instances, what is happening? can you name three possible solutions?

    It may overfitting, or it may testing on the same data sets, the solutions are:

    1. when overfitting, we can use regularization method or dimensional reduction
    2. ~~prepare another varify data set~~
    3. ~~use cross validation~~
    4. get more data

16. What is a test set and why would you want to use it?

    test set can do some test predictions before you launch your model, it's part of the sample data, but without training with it, after test prediction, we know how our model works. 

    the answer from the book:

    The test set is used to estimate the generalization error that a model will make on new instances, before the model is launched in production.

17. What is the purpose of a validation set?

    The main purpose of a validation set is to tune the hyperparameter and **compare models**

18. What can go wrong if you tune hyperparameters using the test set?

    1. If we use test set to tune the hyperparameters, the model may work well on test set, but the correction rate may decrease when it encounters new data.

19. What is cross-validation and why would you prefer it to a validation set?

    it's a technique make it possible to compare models without the need for a separate validation set. This saves the precious training data.

