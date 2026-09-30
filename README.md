# Task 14: NumPy Matrix Operations

**Track:** AI & ML Track  
**Student:** Ayush  

## Project Objective
The purpose of this project is to understand and implement fundamental matrix operations essential for machine learning algorithms using the Python `NumPy` library.

## Covered Operations
- **Matrix Creation:** Generating multi-dimensional structures using `np.array()`.
- **Addition:** Element-wise addition of two matrices.
- **Subtraction:** Element-wise subtraction of two matrices.
- **Matrix Multiplication:** Calculating the dot product using the `@` operator.
- **Transpose:** Flipping a matrix over its diagonal using the `.T` attribute.

## Project Structure
- `matrix_ops.py`: Python script containing the source code implementation.
- `README.md`: Project documentation and short explanation of theory.

## Implementation Code

```python
import numpy as np

# 1. Matrix Creation
matrix_A = np.array([[1, 2], [3, 4]])
matrix_B = np.array([[5, 6], [7, 8]])

print("Matrix A:\n", matrix_A)
print("\nMatrix B:\n", matrix_B)

# 2. Addition
addition_result = matrix_A + matrix_B
print("\n--- Addition Result --- \n", addition_result)

# 3. Subtraction
subtraction_result = matrix_A - matrix_B
print("\n--- Subtraction Result --- \n", subtraction_result)

# 4. Matrix Multiplication
multiplication_result = matrix_A @ matrix_B
print("\n--- Matrix Multiplication Result --- \n", multiplication_result)

# 5. Transpose
transpose_A = matrix_A.T
print("\n--- Transpose of Matrix A --- \n", transpose_A)
```

## Matrix Multiplication Explanation
Unlike element-wise multiplication, matrix multiplication involves taking the dot product of rows from the first matrix and columns from the second matrix. 

For any position $(i, j)$ in the resulting matrix, we multiply each element of row $i$ in Matrix A by the corresponding element of column $j$ in Matrix B, and then sum those products. Because of this structural alignment rule, matrix multiplication requires that the number of columns in the first matrix strictly matches the number of rows in the second matrix.