# ComplexMathScripts
# factorial_calculator.py

def calculate_factorial(n):
    """
    Calculates the factorial of a non-negative integer n.
Add initial Python task scheduling script
import time
import datetime

def perform_task():
    """Simulates performing a scheduled task."""
    print(f"Task executed at: {current_time} - Status: OK")

def main():
    """Main loop for the simple task scheduler."""
    print("Starting Simple Task Scheduler...")
    print("Task execution interval set to 10 seconds.") # <--- خط اضافه شده
    try:
        while True:
            perform_task()
            # Wait for 10 seconds before the next task execution # <--- تغییر زمان از 5 به 10
            time.sleep(10)
    except KeyboardInterrupt:
        print("\nScheduler stopped manually.")

if __name__ == "__main__":
    main()    """
    if not isinstance(n, int):
        raise ValueError("Input must be an integer.")
    if n < 0:
# factorial_calculator.py

# --- Iterative Method (Original) ---
def calculate_factorial_iterative(n):
    """
    Calculates the factorial of a non-negative integer n using an iterative method.
    Raises ValueError for negative inputs or non-integer types.
    """
    if not isinstance(n, int):
        raise ValueError("Input must be an integer.")
    if n < 0:
        raise ValueError("Factorial is not defined for negative numbers.")
    if n == 0:
        return 1
    
    result = 1
    for i in range(1, n + 1):
        result *= i
    return result

# --- Recursive Method (New Addition) ---
def calculate_factorial_recursive(n):
    """
    Calculates the factorial of a non-negative integer n using a recursive method.
    Assumes n is a non-negative integer (error checking is handled by main caller).
    """
    if n == 0:
        return 1
    return n * calculate_factorial_recursive(n - 1)

# Example usage and basic test
if __name__ == "__main__":
    try:
        test_number = 6 # Changed input for testing both methods

        # Test Iterative Method
        iterative_result = calculate_factorial_iterative(test_number)
        print(f"Iterative Factorial of {test_number} is: {iterative_result}") # Expected: 720

        # Test Recursive Method
        recursive_result = calculate_factorial_recursive(test_number)
        print(f"Recursive Factorial of {test_number} is: {recursive_result}") # Expected: 720

        # Example of error checking
        # print(calculate_factorial_iterative(-6)) 
    
    except ValueError as e:
        print(f"Error encountered: {e}")    if n == 0:
        return 1
    
   
