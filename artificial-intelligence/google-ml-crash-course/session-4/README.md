# Session 4

## 6.Generalization
### Empirically
- Evaluate on test set
- A good indicator only if
    1. The test set is large enough
    2. Don't cheat by using test set over & over

### Basic Assumptions
1. Draw examples independently and identically
2. The distribution is **stationary** (does not change over time)
3. Same distribution

---
## 7. Training and Test Sets

### Notes for Test Set
1. Large enough to yield statistically meaningful results.
2. Representative enough of the data set as a whole.
3. Never train on test set.

---
## 8. Validation
### Workflow

![Alt text](https://developers.google.com/machine-learning/crash-course/images/WorkflowWithTestSet.svg "Tensorflow Hierarchy")
- Overfitting!

### A Better Workflow

![Alt text](https://developers.google.com/machine-learning/crash-course/images/WorkflowWithValidationSet.svg "Tensorflow Hierarchy")
- Create fewer exposures to the test set.