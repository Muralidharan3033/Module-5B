# Pandas Program: Create and Display a DataFrame with Custom Index Labels

## 🎯 Aim

To create and display a **DataFrame** using the **Pandas** library in Python from a given dictionary, and apply specific index labels to the rows.

---

## 🧠 Algorithm

1. **Import Libraries**: Import the required libraries – `pandas` and `numpy`.
2. **Create Dictionary**: Define a dictionary `exam_data` with keys: `'name'`, `'score'`, `'attempts'`, and `'qualify'`.
3. **Index Labels**: Create a list of custom index labels called `labels`.
4. **Create DataFrame**: Use `pd.DataFrame()` to create the DataFrame by passing the dictionary and index labels.
5. **Display Output**: Display the DataFrame using `print()` or by simply calling the DataFrame variable.

---

## 💻 Program
```
import pandas as pd
import numpy as np

# Create Dictionary
exam_data = {
    'name': ['John', 'Anna', 'Peter', 'Linda'],
    'score': [88, 92, 85, 79],
    'attempts': [1, 3, 2, 1],
    'qualify': ['yes', 'yes', 'no', 'yes']
}

# Index Labels
labels = ['a', 'b', 'c', 'd']

# Create DataFrame
df = pd.DataFrame(exam_data, index=labels)

# Display Output
print(df)
```

## Output
![image](https://github.com/user-attachments/assets/bb560a76-54e4-4631-981a-535424e56db9)

## Result
Thus the program is sucessfully executed.
