There are many algorithms available to solve a classification problem. In this blog, I will describe the Bayes Classifier. 

The key idea of the Bayes Classifier is to assign each observation to the most likely class given its predictor values (Input). In other words, for each input x, we will have probability for each class j, which can be written as a conditional probability as the following

![image](https://user-images.githubusercontent.com/61811515/93031838-d8bbbc80-f5fb-11ea-93a9-2a5b36e6bcd9.png)

The label would be the one has the maximal probability. 

As one of the examples, assume we have class 1 and class 2. 

![image](https://user-images.githubusercontent.com/61811515/93032020-02291800-f5fd-11ea-88a2-74dc6d3b3826.png)


As you can see in the graph, there are two shaded region which refers the group that is classified in the model if a sample falls in the corresponding region. The purpose dashed line represents the points where the probability equals 50%. The line is also called Bayes decision boundary. 
Bayes classifier produces the lowest possible test error rate, called Bayes error rate. Since every time, Bayes classifier chooses the class with the largest probability, we have probability of 1 - max_{j} P(Y=j | X=x) to get the error. Overall, we will have the following Bayes error rate formulation: 
![image](https://user-images.githubusercontent.com/61811515/93032253-8af48380-f5fe-11ea-9fc4-ce6ed85f00c4.png)

where the expectation averages the probability over all possible values of input X. 

The Bayes error rate is analogous to the irreducible error. 






Reference
James, G., Witten, D., Hastie, T. and Tibshirani, R., n.d. An Introduction To Statistical Learning.



