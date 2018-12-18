# Session 3

## 5. First Step with TF

### Bried Introduction
- Toolkit [introduction](https://developers.google.com/machine-learning/crash-course/first-steps-with-tensorflow/toolkit)
- Hierarchy:
  - ![Alt text](https://developers.google.com/machine-learning/crash-course/images/TFHierarchy.svg "Tensorflow Hierarchy")

### Tensorflow Components
1. a [graph protocol buffer](https://www.tensorflow.org/guide/extend/model_files#protocol_buffers)
2. a runtime that executes the (distributed) graph
- start with the highest-level API first

### Sample Code
```python
import tensorflow as tf

# Set up a linear classifier.
classifier = tf.estimator.LinearClassifier(feature_columns)

# Train the model on some example data.
classifier.train(input_fn=train_input_fn, steps=2000)

# Use it to predict.
predictions = classifier.predict(input_fn=predict_input_fn)
```

- Note that `tf.estimator` is compatible with the `scikit-learn` API

### Model Construction Tips
1. [Gradient clipping](https://developers.google.com/machine-learning/glossary/#gradient_clipping)
2. Be sure to set `num_epochs`
3. Randomize through `shuffle`
4. Working with [Dataset API](https://www.tensorflow.org/guide/datasets)
