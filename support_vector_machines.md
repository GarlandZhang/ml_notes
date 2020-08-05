a supervised learning algorithm

## logistic regression vs SVM

![log](https://i.gyazo.com/25895625df381983386e7befbca61d11.png)

![SVM](https://i.gyazo.com/6df78e650d3286de57f69b617179b93a.png)
  - derived from logistic regression with slightly different format (the theta solution is just a linear equation difference of the theta for logistic regression)
  - C = 1 / lambda
  - cost fn is sigmoid (w/ margin calcualted in?)
  
SVMs are also called **large margin classifiers**:
  - logistic reg
  ![log](https://i.gyazo.com/ac10ce747eabe6ca34815d6d78f749e0.png)
  
  - SVM (so we require the theta'X to be much larger in magnitude, hence the large margin
  ![SVM](https://i.gyazo.com/8bfb3fc98e5b5b7008eae84a61d5f029.png)
  
### SVM decision boundary
why are SVMs superior to logistic regression? Not only does it do what logistic regression does (find a boundary to split the positive and negative examples), it finds the **most optimal** boundary

![ex](https://i.gyazo.com/0932c33c80008a96a97f75fa2f01af51.png)
  - this is possible because we require our internal cost functions more strict to also being larger in magnitude to them argin:
  ![cfn](https://i.gyazo.com/258d5a97eade3e4de0cb058e373be934.png)
  
### outliers
- recall that C = 1 /lambda and acts inversely to lambda
- therefore if C is large, then lambda is small, so the model will overfit the training data
- but if C is not too large, then lambda is not small, so the model will not overfit the training data

![lmi](https://i.gyazo.com/976feedee58a5ed23ea95641496dfa48.png)
