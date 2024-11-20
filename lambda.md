
# Python Lab Manual: Lambda Functions

---

## **Introduction**
A **lambda function** is a small, anonymous function that can take any number of arguments but has only a single expression. Lambda functions are often used for short-term operations or as arguments to higher-order functions.

---

## **1. Syntax of Lambda Functions**

```python
lambda arguments: expression
```

- The expression is executed, and its result is returned.

---

## **2. Basic Examples**

### Example 1: Adding 10 to a given number
```python
x = lambda a: a + 10
print(x(5))  # Output: 15
```

### Example 2: Multiplying two numbers
```python
x = lambda a, b: a * b
print(x(5, 6))  # Output: 30
```

### Example 3: Summing three numbers
```python
x = lambda a, b, c: a + b + c
print(x(5, 6, 2))  # Output: 13
```

---

## **3. Why Use Lambda Functions?**

- **Simplicity**: They allow concise definition of functions.
- **Anonymous**: They are unnamed and defined inline.
- **Use Inside Other Functions**: Useful as arguments to other functions.

---

## **4. Using Lambda Inside Another Function**

### Example: Doubling a Number
```python
def myfunc(n):
    return lambda a: a * n

mydoubler = myfunc(2)
print(mydoubler(11))  # Output: 22
```

### Example: Tripling a Number
```python
def myfunc(n):
    return lambda a: a * n

mytripler = myfunc(3)
print(mytripler(11))  # Output: 33
```

### Combining Both
```python
def myfunc(n):
    return lambda a: a * n

mydoubler = myfunc(2)
mytripler = myfunc(3)

print(mydoubler(11))  # Output: 22
print(mytripler(11))  # Output: 33
```

---

## **5. Summary**

| **Feature**         | **Details**                                                                 |
|----------------------|-----------------------------------------------------------------------------|
| **Definition**       | Anonymous, inline function defined with `lambda`.                         |
| **Syntax**           | `lambda arguments: expression`                                            |
| **Use Case**         | Best for short-term operations or arguments to other functions.           |
| **Limitations**      | Only a single expression (no multi-line operations).                      |
| **Advantages**       | Concise and can be used within other functions for dynamic operations.    |

---

## **6. Practice Problems**

1. Write a lambda function to calculate the square of a number.
2. Create a function that returns a lambda to calculate the power of a number.
3. Use a lambda function to sort a list of tuples by the second element.

---

**Happy Coding!** 🚀
