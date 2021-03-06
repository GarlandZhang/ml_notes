## debugging learning algorithm

what to try next:

![steps](https://i.gyazo.com/474c2e024735d816b7a249111bca3475.png)

to deterine best choice, use a **machien learning diagnostic**: test to gain insight what is/isn't working and gain guidance on next best choice

## evaluating hypothesis

use training/test sets (see validation sets in the section below) to measure test set error:

![tse](https://i.gyazo.com/8e74c6fa3a39837b0f4e7f4d1b461e08.png)

## model selection

suppose you had to select a model from different degrees of polynomial functions. 

**idea**: Train each model and select the model with the lowest test set error 
**problem**: the chosen model will be an overestimate of the true generalization error as we chose the model that performed the best on the test set error (this is cheating!).
**solution**: This motivates the need for **validiation** sets. So we examine for cross validation error instead.

![cost summary](https://i.gyazo.com/1b055c0275ca6a0fd25377cd11756409.png)


## neural networks and overfitting

![small_vs_large](https://i.gyazo.com/008496cf9fd2dbf8b41cf82e1493c95e.png)

## train/dev/test sets
- make sure they come from same distribution
- with big data, we could have 98/1/1 split
