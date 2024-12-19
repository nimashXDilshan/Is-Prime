Prime Number Checker
This is a Python function to check if a given number is a prime number. It uses an efficient method to determine primality by checking divisibility from 2 up to the square root of the given number.

Function: is_prime(n)
Parameters:
n (int): The number to check for primality.
Returns:
True if the number n is a prime number.
False if the number n is not a prime number.
Description:
A prime number is a natural number greater than 1 that has no positive divisors other than 1 and itself. The function is_prime(n) checks if n is prime by dividing n by all numbers from 2 to the square root of n. If any of the numbers divide n evenly, the function returns False. If no divisors are found, it returns True.

Example Usage:
python
Copy code
def is_prime(n):
    if n <= 1:
        return False
    for i in range(2, int(n ** 0.5) + 1):
        if n % i == 0:
            return False
    return True

# Example usage
print(is_prime(11))  # Output: True
Time Complexity:
The time complexity of this algorithm is O(√n), which is efficient for checking primality compared to testing divisibility up to n-1.
