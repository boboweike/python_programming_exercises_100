# Exercise 2(leve 1)

Hello everyone, welcome back to our Python programming exercise series. Are you ready to dive into another exciting challenge? Let's get started!

Today's task is to write a Python program that can compute the factorial of a given number. The result should be printed on a single line. For example, if we input the number 8, the output should be 40320.

A factorial of a number is the product of all positive integers less than or equal to that number. So, we need to multiply all the numbers from 1 to the given number.

Let's write some Python code to illustrate the solution. We'll provide both a non-recursive and a recursive versions.

Here's the non-recursive version:

```python
def compute_factorial_non_recursive(n):
    # Initialize the result to 1
    result = 1

    # Multiply all numbers from 1 to n
    for i in range(1, n + 1):
        result *= i

    # Return the result
    return result

# Call the function with test input and print the result
print(compute_factorial_non_recursive(8))
```

Let me re-summarize the solution here. In this function, `compute_factorial_non_recursive`, we first initialize the `result` to 1. We then multiply all numbers from 1 to `n` and update the `result`. Finally, we return the `result`.

Now, let's look at the recursive version:

```python
def compute_factorial_recursive(n):
    # Base case: factorial of 1 is 1
    if n == 1:
        return 1

    # Recursive case: n factorial is equal to n times (n-1) factorial
    else:
        return n * compute_factorial_recursive(n - 1)

# Call the function with test input and print the result
print(compute_factorial_recursive(8))
```

Let me re-summarize the recursive code here. In the recursive function, `compute_factorial_recursive`, we have a base case where if `n` is 1, we return 1. For the recursive case, we return `n` times the factorial of `n-1`.

Let's run the code with the test input 8. You can see that both functions print out 40320, which is the factorial of 8.

Now, let's write a unit test to verify our solution. To save time, let me just copy the code directly.

```python
def test_compute_factorial():
    assert compute_factorial_non_recursive(5) == 120
    assert compute_factorial_non_recursive(6) == 720
    assert compute_factorial_non_recursive(7) == 5040
    assert compute_factorial_non_recursive(8) == 40320

    assert compute_factorial_recursive(5) == 120
    assert compute_factorial_recursive(6) == 720
    assert compute_factorial_recursive(7) == 5040
    assert compute_factorial_recursive(8) == 40320


# Run the unit test
test_compute_factorial()
```

In this unit test, we're checking that our `compute_factorial_non_recursive` and `compute_factorial_recursive` functions return the correct factorial for the numbers 5, 6, 7, and 8. If the functions are working correctly, the test will pass without any errors. Let's run the test to verify, you see all test cases passed.

So in this exercise, we've explored Python's `for` loops and learned how to compute the factorial of a number both non-recursively and recursively. These are fundamental concepts that you'll use over and over in Python programming.

That's it for today's exercise. I hope you found it useful. Keep practicing and stay tuned for more Python exercises that will sharpen your coding skills. Happy coding, and see you in the next one!
