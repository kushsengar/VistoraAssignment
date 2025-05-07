# VistoraAssignment

# NumPy ND-Array Input from User

This project demonstrates how to take n-dimensional array (ND-array) input from the user in Python using NumPy — **without using loops**.

## 📁 Files

- `Task.ipynb` – Jupyter Notebook demonstrating different input techniques.
- `raw_transactions.csv` – Sample CSV file (possibly for data-related tasks, not directly related to ND-array input).
- `README.md` – You're here!

## 📌 Features

- Take list of integers as input using `map()` and `split()` (no loop).
- Accept 2D NumPy arrays from user input.
- Easily adaptable to higher dimensions (3D, 4D, etc.).

## 🧪 Example: 2D Array Input

python
import numpy as np

rows, cols = map(int, input("Enter number of rows and columns: ").split())
arr = np.array(input("Enter the elements: ").split(), dtype=int).reshape(rows, cols)

print(arr)

💬 Sample Input:
yaml
Copy
Edit
Enter number of rows and columns: 2 3
Enter the elements: 1 2 3 4 5 6
✅ Output:
lua
Copy
Edit
[[1 2 3]
 [4 5 6]]
🛠 Requirements
Python 3.x

NumPy

You can install NumPy using pip:

bash
Copy
Edit
pip install numpy
📌 Notes
The code assumes that the number of elements entered matches rows * cols.

The .reshape() method will raise an error if the number of elements does not fit the shape.

This method avoids explicit loops and uses Python's functional features.
