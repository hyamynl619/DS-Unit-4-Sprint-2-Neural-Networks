<title> Implementing a Perceptron from Scratch </title>
```
#Establish training data
import numpy as np

np.random.seed(812)
inputs = np.array([
          [0,0,1];
          [1,1,1],
          [1,0,1],
          [0,1,1]
          ])
correct_outputs = [[0],[1],[1],[0]]
```

```
#Sigmoid activation func & its updating weights

def sigmoid(x):
  return 1/(1+np.exp(-x)

def sigmoid_derivative(x):
  sx = sigmoid(x)
  return sx * (1-sx)
```

```
#Update Weights

weights = 2 * np.random.random((3,1))-1

#Calculate weighted sum of inputs & weights

weighted_sum = np.dot(inputs, weights)
weighted_sum
```

