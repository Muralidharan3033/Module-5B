# # NumPy Program: Find Indices Where Elements in Array x are Greater Than or Equal to Corresponding Elements in Array y

## 🎯 Aim
To write a Python program using **NumPy** that finds the indices where elements in array `x` are greater than or equal to their corresponding elements in array `y`.

## 🧠 Algorithm
1. **Import NumPy**: Import the NumPy library.
2. **Define Arrays**: Define two NumPy arrays, `x` and `y`, with the same shape (i.e., same number of elements).
3. **Use Boolean Indexing**: 
   - `x > y` gives a boolean array where elements of `x` are greater than `y`.
   - `x == y` gives a boolean array where elements of `x` are equal to `y`.
4. **Find Indices**: Use `np.where()` to get the indices where the conditions `x >= y` are satisfied.
5. **Print Indices**: Print the indices where the condition holds true.

## 🧾 Program
```
import numpy as np

# Define Arrays
x = np.array([1, 5, 3, 8, 7])
y = np.array([2, 5, 4, 7, 6])

# Use Boolean Indexing
greater_than = x > y
equal_to = x == y

# Find Indices where condition x >= y is satisfied
indices = np.where(x >= y)

# Print Indices
print("Indices where x >= y:", indices)
```


## Output
![image](https://github.com/user-attachments/assets/11334a78-ae0f-495d-9686-9cfa9a4097c4)


## Result
Thus the program is sucessfully executed.
