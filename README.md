# Mean-Variance-Standard Deviation Calculator

It uses the **NumPy** library to calculate basic statistical measures from a 3 × 3 matrix.

## Features

The program calculates:

* Mean
* Variance
* Standard Deviation
* Maximum
* Minimum
* Sum

The calculations are performed for:

* Each column
* Each row
* The entire matrix

## Project Structure

```text
.
├── mean_var_std.py     # Main solution
├── main.py             # Run and test the program
├── test_module.py      # Unit tests
└── README.md           # Project documentation
```

## Requirements

* Python 3.x
* NumPy

Install NumPy using:

```bash
pip install numpy
```

## Usage

Import the `calculate()` function from `mean_var_std.py`.

```python
from mean_var_std import calculate

print(calculate([0, 1, 2, 3, 4, 5, 6, 7, 8]))
```

## Example Output

```python
{
  'mean': [[3.0, 4.0, 5.0], [1.0, 4.0, 7.0], 4.0],
  'variance': [[6.0, 6.0, 6.0], [0.6666666666666666, 0.6666666666666666, 0.6666666666666666], 6.666666666666667],
  'standard deviation': [[2.449489742783178, 2.449489742783178, 2.449489742783178], [0.816496580927726, 0.816496580927726, 0.816496580927726], 2.581988897471611],
  'max': [[6, 7, 8], [2, 5, 8], 8],
  'min': [[0, 1, 2], [0, 3, 6], 0],
  'sum': [[9, 12, 15], [3, 12, 21], 36]
}
```

## Error Handling

The function expects a list containing exactly **9 numbers**.

Example:

```python
calculate([1, 2, 3])
```

Output:

```text
ValueError: List must contain nine numbers.
```

## How It Works

1. Accepts a list of nine numbers.
2. Converts the list into a 3 × 3 NumPy array.
3. Computes statistical values using NumPy functions.
4. Returns the results as a dictionary containing lists for rows, columns, and the flattened matrix.

## Technologies Used

* Python 3
* NumPy

## Project Status

Completed.