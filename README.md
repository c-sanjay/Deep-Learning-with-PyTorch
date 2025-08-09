# PyTorch Basics Exercises

## AIM:
Write a Python program using PyTorch that performs the following tasks:

### Software Required:
- Python 3.x
- PyTorch
- Jupyter Notebook (for interactive development and execution)

## Algorithm:

### Step 1:
Perform standard imports
- Import `torch` and `NumPy`.

```python
import torch
import numpy as np
```

### Step 2:
Set the random seed for NumPy and PyTorch both to `42`.

```python
np.random.seed(42)
torch.manual_seed(42)
```

### Step 3:
Create a NumPy array called `arr` that contains 6 random integers between 0 (inclusive) and 5 (exclusive).

```python
arr = np.random.randint(0,5,6)
print(arr)
```

### Step 4:
Create a tensor `x` from the array above.

```python
x=torch.tensor(arr)
print(x,x.dtype)
```

### Step 5:
Change the dtype of `x` from `int32` to `int64`.

```python
 print(x,x.dtype)
```

### Step 6:
Reshape `x` into a `3x2` tensor.

```python
x=np.reshape(x,(3,2))
print(x)
```

### Step 7:
Return the right-hand column of tensor `x`.

```python
right=print(x[:,1:])
```

### Step 8:
Without changing `x`, return a tensor of square values of `x`.

```python
np.reshape(x**2,(3,2))
```

### Step 9:
Create a tensor `y` with the same number of elements as `x`, that can be matrix-multiplied with `x`.
- Use PyTorch directly (not NumPy) to create a tensor of random integers between 0 (inclusive) and 5 (exclusive).

```python
y=torch.randint(0,5,(2,3))
print(y)
```

### Step 10:
Find the matrix product of `x` and `y`.

```python
print(torch.mm(x,y))
```
## Output:
i) Import and set up PyTorch and NumPy.
ii) Create and manipulate tensors.
iii) Perform matrix operations.

## Result:
Thus, the PyTorch tensor operations, including reshaping, dtype conversion, and matrix multiplication, were successfully performed using the Python program.
