## Exploring Deep Learning Libraries and Performing Basic Tensor Operations Using TensorFlow

---

### Aim

To familiarize students with popular deep learning libraries and perform basic tensor creation and mathematical operations using TensorFlow.

---

### Scope

This practical introduces the deep learning software ecosystem and covers the installation of TensorFlow, creation of different types of tensors, basic tensor operations, and comparison of commonly used deep learning libraries.

---

### Dataset

**Not Applicable**

---

### Libraries Used

* TensorFlow
* NumPy

---

### Practical Description

In this practical, students will install TensorFlow, verify the installation, display the installed TensorFlow version, create different types of tensors, perform basic mathematical and matrix operations, reshape tensors, convert NumPy arrays into TensorFlow tensors, and compare TensorFlow with other popular deep learning libraries.

This practical serves as the foundation for subsequent deep learning experiments.

---

## Part A – Installation

### 1. Install TensorFlow

TensorFlow is installed using the Python package manager:

```bash
pip install tensorflow
```

### 2. Verify TensorFlow Installation

The TensorFlow installation is verified by importing the library successfully in Python.

```python
import tensorflow as tf
```

### 3. Display TensorFlow Version

The installed TensorFlow version is displayed using:

```python
print(tf.__version__)
```

---

## Part B – Tensor Creation

TensorFlow supports tensors of different dimensions and shapes.

### 4. Scalar Tensor

A scalar tensor contains a single value.

```python
scalar = tf.constant(10)
print(scalar)
```

### 5. Vector Tensor

A vector tensor is a one-dimensional tensor containing multiple values.

```python
vector = tf.constant([10, 20, 30])
print(vector)
```

### 6. Matrix Tensor

A matrix tensor is a two-dimensional tensor containing rows and columns.

```python
matrix = tf.constant([
    [1, 2, 3],
    [4, 5, 6]
])
print(matrix)
```

### 7. Three-Dimensional Tensor

A three-dimensional tensor contains multiple two-dimensional matrices.

```python
tensor_3d = tf.constant([
    [[1, 2], [3, 4]],
    [[5, 6], [7, 8]]
])
print(tensor_3d)
```

---

## Part C – Tensor Operations

### 8. Tensor Addition

Element-wise addition is performed between two tensors of compatible shapes.

```python
a = tf.constant([1, 2, 3])
b = tf.constant([4, 5, 6])

result = tf.add(a, b)
print(result)
```

### 9. Tensor Subtraction

Element-wise subtraction is performed using TensorFlow.

```python
result = tf.subtract(a, b)
print(result)
```

### 10. Tensor Multiplication

Element-wise multiplication is performed between two tensors.

```python
result = tf.multiply(a, b)
print(result)
```

### 11. Matrix Multiplication

Matrix multiplication is performed using `tf.matmul()`.

```python
matrix_a = tf.constant([
    [1, 2],
    [3, 4]
])

matrix_b = tf.constant([
    [5, 6],
    [7, 8]
])

result = tf.matmul(matrix_a, matrix_b)
print(result)
```

### 12. Reshape an Existing Tensor

An existing tensor can be reshaped into a different compatible shape.

```python
tensor = tf.constant([1, 2, 3, 4, 5, 6])

reshaped_tensor = tf.reshape(tensor, [2, 3])
print(reshaped_tensor)
```

### 13. Convert NumPy Array into TensorFlow Tensor

A NumPy array can be converted into a TensorFlow tensor using `tf.convert_to_tensor()`.

```python
import numpy as np

array = np.array([10, 20, 30])

tensor = tf.convert_to_tensor(array)

print(tensor)
```

---

## Part D – Framework Comparison

### 14. Study of TensorFlow, PyTorch, and Keras

TensorFlow, PyTorch, and Keras are widely used frameworks and libraries in the deep learning ecosystem.

### 15. Comparison of Deep Learning Libraries

| Feature              | TensorFlow                                       | PyTorch                                | Keras                                                                                                              |
| -------------------- | ------------------------------------------------ | -------------------------------------- | ------------------------------------------------------------------------------------------------------------------ |
| Developer            | Google                                           | Meta AI                                | Originally developed by François Chollet; now part of the TensorFlow ecosystem and also supports multiple backends |
| Type                 | Deep Learning Framework                          | Deep Learning Framework                | High-level Deep Learning API                                                                                       |
| Programming Language | Python, C++ and others                           | Python, C++ and others                 | Python                                                                                                             |
| Ease of Use          | Moderate                                         | Easy to Moderate                       | Very Easy                                                                                                          |
| Model Building       | Flexible                                         | Flexible                               | Simple and intuitive                                                                                               |
| Debugging            | Good                                             | Excellent                              | Easy                                                                                                               |
| Deployment           | Strong deployment support                        | Strong deployment support              | Supports deployment through supported backends                                                                     |
| Best Suited For      | Large-scale production and research              | Research and dynamic model development | Rapid prototyping and easy model development                                                                       |
| Applications         | Computer Vision, NLP, Time Series, Generative AI | Computer Vision, NLP, Research         | Classification, Computer Vision, NLP, Prototyping                                                                  |

---

### Advantages and Applications

#### TensorFlow

**Advantages:**

* Suitable for large-scale deep learning applications
* Provides extensive tools for model development and deployment
* Supports CPU, GPU, and specialized hardware
* Offers strong production and deployment capabilities

**Applications:**

* Computer Vision
* Natural Language Processing
* Time-Series Analysis
* Generative AI
* Large-scale Machine Learning Systems

---

#### PyTorch

**Advantages:**

* Easy and intuitive Python-based interface
* Dynamic computation graphs make experimentation easier
* Widely used for deep learning research
* Provides flexible model development and debugging

**Applications:**

* Computer Vision
* Natural Language Processing
* Reinforcement Learning
* Generative AI
* Deep Learning Research

---

#### Keras

**Advantages:**

* Simple and beginner-friendly API
* Makes neural network development easier
* Supports rapid prototyping
* Provides high-level abstractions for building and training models

**Applications:**

* Classification
* Regression
* Computer Vision
* Natural Language Processing
* Rapid Deep Learning Prototyping

---

## Results and Outcome

The practical successfully demonstrated the installation and verification of TensorFlow and the creation of different types of tensors.

The following tensor operations were successfully performed:

* Scalar tensor creation
* Vector tensor creation
* Matrix tensor creation
* Three-dimensional tensor creation
* Tensor addition
* Tensor subtraction
* Element-wise tensor multiplication
* Matrix multiplication
* Tensor reshaping
* NumPy array to TensorFlow tensor conversion

The practical also provided a comparative understanding of **TensorFlow, PyTorch, and Keras**, including their features, advantages, and common applications.

---

## Repository Structure

```text
practical1/
├── tensorflow_operations.ipynb   # Main notebook (Parts A–D)
├── requirements.txt              # Python dependencies
├── README.md                     # This file
└── .gitignore                    # Git ignored files
```

---

## How to Run

```bash
pip install -r requirements.txt
jupyter notebook tensorflow_operations.ipynb
```

---

## Author

*Name:* Navya Manda
*Email:*  navyaspace369@gmail.com
*Course:* B.Tech – Deep Learning Practical
