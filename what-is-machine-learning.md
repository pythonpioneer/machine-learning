# What is Machine Learning?

In today's era, Machine Learning (ML) has become one of the most popular, influential, and rapidly growing fields. Machine learning (ML) powers everything from personalized song suggestions to reusable rocket launch systems, spam detection, and medical diagnosis. But what is Machine Learning (ML), and how does it work?

In this article, we'll explore the fundamentals of ML, the types of machine learning, how it works, its advantages and benefits, and some real-world applications and challenges associated with this transformative technology.

## Table of Contents

1. Introduction to Machine Learning
2. How Machine Learning works
3. Types of Machine Learning
   - Supervised Machine Learning
   - Unsupervised Machine Learning
   - Reinforcement Machine Learning
4. Real-world applications of Machine Learning
5. Advantages of Machine Learning
6. Disadvantages of Machine Learning
7. Challenges in Machine Learning
8. Conclusion

## 1. Introduction to Machine Learning

Machine Learning is a revolutionizing technology and it has the potential to transmute the future. It enables computers to make data-driven decisions without explicit human interactions. As we know, Machine Learning (ML) is a subset of Artificial Intelligence (AI) that allows computers to learn from data or make decisions or predictions based on that learning. Unlike traditional programming approaches, where a programmer must explicitly define rules for a task, ML systems automatically learn from the data, identify patterns, and make decisions without being explicitly programmed for specific tasks.

![ml-header](./ml-dark.png#gh-dark-mode-only)
![ml-header](./ml-light.png#gh-light-mode-only)

Machine Learning systems usually take place where rule-based programming or traditional programming approaches are too complex or impractical to implement. Such as Image recognition, text recognition, and self-driving cars.

**Formal Definition of Machine Learning**

In technical terms, machine learning refers to the development of algorithms that enable a machine to improve its performance based on past experiences. These experiences are usually presented in the form of data, and the machine learns by analyzing this data to identify trends and patterns.


## 2. How Machine Learning Works

At its core, machine learning relies on various algorithms and data. The process typically starts by creating a model and then we provide data to our model and then the model starts training with the given data, the training will only be successful, if our data is reliable and sufficient to train the model. There are various techniques to judge whether the data is reliable or not, and accuracy is one of those metrics. So, after the training, we check the accuracy of the model, and if everything is as expected then we say the model is dependable. Now, whenever, we pass the fresh input to the model, it will predict or make decisions based on the previous training.

**What happens when the accuracy is not as expected**

In this case, where the accuracy is not as expected, it means that the model is an `underfit model` (where the accuracy is very low) or an `overfit model` (where the accuracy is very high). In both scenarios, the model will be retrained. 

**You might wonder that if we use the same data for retraining, how can we expect a different result? Let's deep dive into this question.**

This is a great question and the answer lies in the training process. How we structure the training process, and how we modify the different aspects of the training to improve the model's performance. If we simply retrain the model using the same approach and the same dataset, the results are likely to be similar. To resolve the issue we have several techniques:

- **Changing the model architecture:** We can modify the model architecture and algorithms. For example, if we are using `classification supervised machine learning` and the dataset is not suitable for this algorithm then we can switch to some other machine learning algorithms like `clustering unsupervised machine learning` or some other suitable machine learning algorithms. It can help us to improve the model's accuracy and performance.
- **Hyperparameter tuning:** It is a critical aspect of machine learning that directly affects the performance of a model. Unlike model parameters (which are learned automatically during training), hyperparameters are set before the training begins and they control how the model learns. It is essential for optimizing the learning process, improving accuracy, and ensuring the model generalizes to unseen and fresh data. Hyperparameters include the `learning rate` (change the model's weights during training), `batch size` (the number of data processed per iteration), `number of epochs` (total times the entire training dataset is passed through the model), `momentum`, and `dropout rate`.
- **Data Cleaning:** Data cleaning is essential for ensuring the quality of the dataset used to train the model. Unclean data, which may contain errors, inconsistencies, missing values, or outliers can significantly impact the model's accuracy. Therefore it's important to clean the data before training.
- **Data Splitting:** If we did everything well and still got an overfit or underfit model, then we need to rethink the dataset splitting. Before training the model, we clean the dataset and then split the dataset into three parts, training set (this portion of the dataset is used to train the model), validation set (this subset of the dataset used to tune the model's hyperparameters), and test set (this portion of dataset is new to the model and used to test the model).

There are other various techniques to improve the performance and accuracy of the model.

## 3. Types of Machine Learning

Machine learning can be broadly categorized into three types: **Supervised Machine Learning**, **Unsupervised Machine Learning**, and **Reinforcement Machine Learning**. Each type serves different purposes and it depends on the type of dataset and the various kinds of problems.

  1. **Supervised Machine Learning:** In supervised learning, the model is trained on a labeled dataset, which means that in the training dataset, each input value has a corresponding output value and the goal for the model is to learn a mapping from the inputs to outputs based on the given labeled data.
     
     Example: let's say we have a dataset in which, a picture of oranges is labeled with the text orange and a picture of mango is labeled with the text mango we have so much input data in the dataset with the variety of images. So, in this scenario, the trained model can identify that the given image is a mango, an orange, or none of them.

  2. **Unsupervised Machine Learning:** In unsupervised learning, the model is trained on an unlabeled dataset, which means that there is no label provided for the input values and the goal of the model is to learn from the structure of the data, identify the patterns in the data and the relationship within the data without any explicit guidance.

     Example: Let's consider the above dataset but without the label, means that we have images of oranges and images of mangoes but there is no label mentioning which one is what type of fruit. In this scenario, the model analyzes the features of the images to discern that they represent different types of fruits. It will cluster the images based on similarities in their visual characteristics and it can identify that this is a different fruit and this one is a different fruit and the other fruit's images will be unidentified.

  3. **Reinforcement Machine Learning:** Reinforcement learning is a type of machine learning where an agent learns to make decisions by interacting with the given environment. Unlike supervised and unsupervised learning where the models learn from the labeled data or by identifying patterns, reinforcement learning focuses on learning through the trial and error method, receiving feedback from its action in the form of penalties and rewards.

     In reinforcement learning, the agent starts the learning from an initial state or state zero and performs an action based on its policy (a policy is a decision-making guide for example a mopping robot can only move forward and to move backward, it has to rotate 180deg and then it can move). The action will result in a new state and feedback. If the feedback is a reward then the performed action is reliable and the agent will update the policy as per the reward. if the feedback is a penalty then the model will think about some other actions. And the goal is to maximize the cumulative reward over time.

     Example: Considering the same dataset, a robot (model) is trying to identify which images of fruits, such as oranges and mangoes. In this scenario, the model will start with a trial-and-error approach and it will be very random, it will take so many fruit names based on the visual features, and as per the name, it gets feedback in the form of rewards or penalties. A reward means that the robot guesses the correct feature or a penalty means the need for improvements. After so many tries, it begins to recognize correct patterns and correlations between the specific visual characteristics and the corresponding fruit names. Over time the iterative learning process enables the model to refine its guessing strategy, leading to more accurate guesses. (Note: this is not a suitable algorithm for this task).








