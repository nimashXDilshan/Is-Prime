Here's a more colorful and visually appealing README for the prime number checker problem:

---

# 🌟 Prime Number Checker 🌟

## 🧑‍💻 Overview

This Python function, `is_prime(n)`, checks whether a given number `n` is **prime**. It uses an efficient approach by checking divisibility only up to the square root of `n`.

A **prime number** is a natural number greater than 1 that has no positive divisors other than 1 and itself. This function helps in verifying the primality of numbers quickly!

## 📜 Function: `is_prime(n)`

### 📝 Parameters:
- **`n`** (int): The number to check for primality.

### 🔙 Returns:
- **`True`** if the number `n` is prime.
- **`False`** if the number `n` is not prime.

### ⚙️ How It Works:
The function checks if `n` is divisible by any number between 2 and the square root of `n`. If any divisor is found, it returns `False`. If no divisors are found, it returns `True`, indicating that the number is prime.

### 🎯 Example Usage:

```python
def is_prime(n):
    if n <= 1:
        return False
    for i in range(2, int(n ** 0.5) + 1):
        if n % i == 0:
            return False
    return True

# Example Usage
print(is_prime(11))  # Output: True
print(is_prime(15))  # Output: False
```

---

## 🕹️ Example Outputs:

- **Input**: `is_prime(11)`
  - **Output**: `True` (since 11 is a prime number)

- **Input**: `is_prime(15)`
  - **Output**: `False` (since 15 is divisible by 3 and 5)

---

## ⏳ Time Complexity

The time complexity of the `is_prime(n)` function is **O(√n)**. This is an optimized approach compared to testing divisibility up to `n-1`, significantly improving performance for large numbers.

---

## 🎨 License

This project is open-source and available for you to use and modify. Feel free to create your own version or improvements.

---

### 📌 Key Highlights:

- **Efficient**: Checks divisibility up to √n.
- **Simple**: Easy-to-understand algorithm.
- **Reusable**: Can be integrated into other projects involving prime number checks.

---
