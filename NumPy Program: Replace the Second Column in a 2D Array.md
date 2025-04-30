# NumPy Program: Replace the Second Column in a 2D Array

## 🎯 Aim
To write a **NumPy** program that deletes the second column from a given 2D array and inserts a new column at the same position.

## 🧠 Algorithm
1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Get a 2D NumPy array and a new column (as another array) from the user.
3. **Delete Column**: Use `np.delete()` to remove the second column (index 1) from the original array.
4. **Insert Column**: Use `np.insert()` to insert the new column at the second column's original position.
5. **Display Result**: Print the updated array with the replaced column.

## 🧾 Program
```
import numpy as np

# Get Input: Get a 2D NumPy array and a new column (as another array) from the user
rows = int(input("Enter the number of rows: "))
cols = int(input("Enter the number of columns: "))
array = []

for i in range(rows):
    row = list(map(int, input(f"Enter row {i + 1}: ").split()))
    array.append(row)

array = np.array(array)

new_column = list(map(int, input("Enter the new column (same number of rows): ").split()))
new_column = np.array(new_column).reshape(-1, 1)

# Delete Column: Remove the second column (index 1) from the original array
updated_array = np.delete(array, 1, axis=1)

# Insert Column: Insert the new column at the second column's original position
final_array = np.insert(updated_array, 1, new_column, axis=1)

# Display Result: Print the updated array with the replaced column
print("Updated Array with Replaced Column:")
print(final_array)
```

## Output
![image](https://github.com/user-attachments/assets/89acf7d5-eacd-49ee-8219-16aa27390bfe)


## Result
Thus the program is sucessfully executed.
