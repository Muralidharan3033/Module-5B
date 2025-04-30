# 🧪 Pandas Program: Join Two DataFrames Along Rows

## 🎯 AIM

To write a Python program using Pandas to **join two DataFrames along rows** (row-wise concatenation) and assign all data to a new DataFrame.

---

## 🧠 ALGORITHM

1. **Import Libraries**: Import the `pandas` library.
2. **Create First DataFrame**: Use a dictionary to create `student_data1`.
3. **Create Second DataFrame**: Use another dictionary to create `student_data2`.
4. **Concatenate DataFrames**: Use `pd.concat()` with `axis=0` to concatenate both DataFrames row-wise.
5. **Display Result**: Print the new combined DataFrame.

---

## 💻 Program

```
import pandas as pd

# Create First DataFrame
student_data1 = {
    'name': ['John', 'Anna', 'Peter'],
    'score': [88, 92, 85],
    'attempts': [1, 3, 2]
}

# Create Second DataFrame
student_data2 = {
    'name': ['Linda', 'James', 'Laura'],
    'score': [79, 93, 80],
    'attempts': [1, 1, 2]
}

# Create DataFrames
df1 = pd.DataFrame(student_data1)
df2 = pd.DataFrame(student_data2)

# Concatenate DataFrames row-wise
combined_df = pd.concat([df1, df2], axis=0)

# Display Result
print(combined_df)
```

## Output
![image](https://github.com/user-attachments/assets/a555bef2-0e6b-496e-ad94-c9bbfedd7c21)


## Result
Thus the program is sucessfully executed.
