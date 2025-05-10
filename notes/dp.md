## Drop-out
- can be intepreted as sampling a neural network withing the full NN, and only updating the parameters of the sampled network based on input data. The layer drops out a random set of activations in that layer by setting them to zero.
- During testing, there's no drop-out applied
- Dropping out is like a zero mask that sets some of the weights to zero.
- Drop-out makes sure that the network ins't getting too fitted to the training data and helps alleviate the overfitting problem

- ## References
- https://pantelis.github.io/cs677/docs/common/lectures/optimization/regularization/
