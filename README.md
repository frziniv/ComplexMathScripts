# ComplexMathScripts
# factorial_calculator.py

def calculate_factorial(n):
    """
    Calculates the factorial of a non-negative integer n.
    Raises ValueError for negative inputs or non-integer types.
    """
    if not isinstance(n, int):
        raise ValueError("Input must be an integer.")
    if n < 0:
        raise ValueError("Factorial is not defined for negative numbers.")
    if n == 0:
        return 1
    
   
