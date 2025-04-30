# NumPy Program: Column-wise Sorting of a 2D Array

## 🎯 Aim
To write a **NumPy** program that sorts the elements in each column of a given 2D array in ascending order.

## 🧠 Algorithm

1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Accept a 2D NumPy array from the user.
3. **Sort Column-wise**: Use the `np.sort()` function with `axis=0` to sort each column in ascending order.
4. **Store Result**: Store the sorted result in a new array.
5. **Display Output**: Print the original array and the column-wise sorted array.

## 🧾 Program
```
import numpy as np

# Get Input: Accept a 2D NumPy array from the user
rows = int(input("Enter number of rows: "))
cols = int(input("Enter number of columns: "))
array = []

for i in range(rows):
    row = list(map(int, input(f"Enter row {i+1}: ").split()))
    array.append(row)

array = np.array(array)

# Sort Column-wise: Sort each column in ascending order
sorted_array = np.sort(array, axis=0)

# Display Output: Print the original array and the column-wise sorted array
print("Original Array:")
print(array)

print("Column-wise Sorted Array:")
print(sorted_array)
```
## Output
![image](https://github.com/user-attachments/assets/350d5502-7e34-448a-86f1-02a3ba891401)


## Result
Thus the program is sucessfully executed.
