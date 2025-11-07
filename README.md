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
    
    # Use an iterative approach for calculation
    result = 1
    for i in range(1, n + 1):
        result *= i
    return result

# Example usage and basic test
if __name__ == "__main__":
    try:
        # Example 1: Standard input
        number = 5
        print(f"The factorial of {number} is: {calculate_factorial(number)}") # Expected: 120

        # Example 2: Zero
        number_zero = 0
        print(f"The factorial of {number_zero} is: {calculate_factorial(number_zero)}") # Expected: 1

        # Example 3: Negative input (will raise an error)
        # print(calculate_factorial(-5)) 
    
    except ValueError as e:
        print(f"Error encountered: {e}")
