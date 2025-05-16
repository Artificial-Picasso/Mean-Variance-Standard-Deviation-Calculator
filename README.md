# Mean-Variance-Standard Deviation Calculator

## Description
This project is a Python function that calculates key statistical measures (mean, variance, standard deviation, max, min, and sum) for a 3×3 matrix. The function takes a list of 9 numbers, converts it into a 3×3 matrix, and returns comprehensive statistics for:
- Each row
- Each column 
- The entire flattened matrix

## Features
- Input validation to ensure exactly 9 numbers are provided
- Conversion of list to 3×3 matrix using NumPy
- Calculation of six key statistical measures:
  - Mean
  - Variance
  - Standard deviation
  - Maximum values
  - Minimum values
  - Sums
- Results organized in a clear dictionary structure
- Axis-wise calculations (rows, columns, and flattened matrix)

## Usage
1. Import the function from the notebook/file
2. Call `calculate()` with a list of exactly 9 numbers
3. The function returns a dictionary with all calculated statistics

### Example
```python
result = calculate([0, 1, 2, 3, 4, 5, 6, 7, 8])
print(result)
```

### Sample Output
```python
{
    'mean': [[3.0, 4.0, 5.0], [1.0, 4.0, 7.0], 4.0],
    'variance': [[6.0, 6.0, 6.0], [0.666, 0.666, 0.666], 6.666],
    'standard deviation': [[2.449, 2.449, 2.449], [0.816, 0.816, 0.816], 2.581],
    'max': [[6, 7, 8], [2, 5, 8], 8],
    'min': [[0, 1, 2], [0, 3, 6], 0],
    'sum': [[9, 12, 15], [3, 12, 21], 36]
}
```

## Requirements
- Python 3.x
- NumPy library (`pip install numpy`)

## Error Handling
The function raises a `ValueError` if:
- The input list doesn't contain exactly 9 numbers

## Author
Motlalepula Lawrence Tshabalala  
Date: 2025/05/11

## Notes
- All calculations are performed using NumPy for efficiency and accuracy
- The dictionary structure makes it easy to access specific statistics programmatically
- Results are returned as native Python types (lists and floats) for compatibility
