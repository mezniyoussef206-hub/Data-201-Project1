# Data-201-Project1
## Classification in Practice: Bank Marketing

This project uses a Portuguese bank marketing dataset to predict whether a customer will subscribe to a term deposit.

### Dataset
- 45,211 observations
- Target variable: `y`
- Classes: Yes / No
- The target is imbalanced, with about 88.3% No and 11.7% Yes.

### Predictors Used
- campaign
- poutcome
- pdays
- previous
- loan

### Models Compared
- Logistic Regression
- LDA
- QDA
- KNN

A 30% classification threshold was used because false negatives were considered more costly than false positives. Missing a customer who would subscribe represents a lost opportunity, while a false positive mainly results in an unnecessary marketing call.

### Main Finding
KNN with K = 15 was selected as the final model. It had the highest recall and F1 score among the models tested, which better matched the goal of identifying more potential subscribers.
