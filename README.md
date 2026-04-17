# Math Library Project

A simple mathematical functions library implemented in Python.

## Features

This library provides basic mathematical operations:

- **add(a, b)** - Addition of two numbers
- **sub(a, b)** - Subtraction of two numbers  
- **mul(a, b)** - Multiplication of two numbers
- **div(a, b)** - Division of two numbers (with zero division check)
- **power(a, b)** - Exponentiation (a to the power of b)
- **modulus(a, b)** - Modulo operation
- **average(a, b)** - Average of two numbers
- **square(a)** - Square of a number

## Installation

```bash
# Clone the repository
git clone https://github.com/Pooja-S-2006/math-lib-project.git
cd math-lib-project

# No additional dependencies required
```

## Usage

```python
from calc import add, sub, mul, div, power, modulus, average, square

# Basic operations
result1 = add(5, 3)        # Returns 8
result2 = sub(10, 4)       # Returns 6
result3 = mul(3, 7)        # Returns 21
result4 = div(15, 3)       # Returns 5.0
result5 = power(2, 3)       # Returns 8
result6 = modulus(10, 3)     # Returns 1
result7 = average(4, 8)      # Returns 6.0
result8 = square(5)          # Returns 25

# Example with error handling
try:
    result = div(10, 0)
    print(result)  # Returns "Cannot divide by zero"
except:
    print("An error occurred")
```

## Functions Documentation

### add(a, b)
Adds two numbers together.
- **Parameters**: a (number), b (number)
- **Returns**: Sum of a and b

### sub(a, b)
Subtracts b from a.
- **Parameters**: a (number), b (number)
- **Returns**: Difference of a and b

### mul(a, b)
Multiplies two numbers.
- **Parameters**: a (number), b (number)
- **Returns**: Product of a and b

### div(a, b)
Divides a by b with zero division protection.
- **Parameters**: a (number), b (number)
- **Returns**: Quotient of a and b, or error message if b is zero

### power(a, b)
Raises a to the power of b.
- **Parameters**: a (number), b (number)
- **Returns**: a raised to the power of b

### modulus(a, b)
Returns the remainder of division of a by b.
- **Parameters**: a (number), b (number)
- **Returns**: Remainder when a is divided by b

### average(a, b)
Calculates the average of two numbers.
- **Parameters**: a (number), b (number)
- **Returns**: Average of a and b

### square(a)
Calculates the square of a number.
- **Parameters**: a (number)
- **Returns**: Square of a

## Testing

```bash
# Run basic tests
python -c "
from calc import *
print('Testing add:', add(2, 3) == 5)
print('Testing sub:', sub(5, 2) == 3)
print('Testing mul:', mul(4, 3) == 12)
print('Testing div:', div(10, 2) == 5.0)
print('Testing power:', power(2, 3) == 8)
print('Testing modulus:', modulus(10, 3) == 1)
print('Testing average:', average(4, 6) == 5.0)
print('Testing square:', square(5) == 25)
"
```

## Error Handling

The library includes basic error handling:
- Division by zero returns a descriptive error message
- All functions expect numeric inputs

## License

This project is licensed under the MIT License.

## Author

Created by Pooja S - 2006
