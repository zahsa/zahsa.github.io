## Validation
- We cannot use the test set for the purpose of tweaking parameters, since the model will overfit to the data
- We split training data into train and validation data.
## Cross-validation
- Instead of randomly choosing the validation set, iterate over the whole train data and choose different validation sets and average the performance across these sets.
- Example: 5-fold cross-validation: Split the train data into 5 folds, use 4 folds for training and 1 for validation. Finally average the performance across these folds

- In practice, people prefer to avoid cross-validation because it's computationally expensive. People prefer a single validation split.
