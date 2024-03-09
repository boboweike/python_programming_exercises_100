Hello everyone, welcome back to our Python programming exercise series. Today we're going to tackle a slightly more complex problem. Don't worry, I'll guide you through it step by step. Let's dive right in!

Our task today is to write a program that calculates and prints the value according to a given formula: Q equals the square root of [(2 * C * D) / H]. Here, C is 50 and H is 30. D is a variable whose values we'll input to our program in a comma-separated sequence.

Let's start by writing the Python code for this problem.

```python
import math

c = 50
h = 30

d_values = input("Please enter the values of D, separated by commas: ").split(',')
result = []

for d in d_values:
    q = math.sqrt((2 * c * int(d)) / h)
    result.append(str(round(q)))

print(", ".join(result))
```

In this code, we first import the `math` module to use the `sqrt` function. We then define the constants C and H. We ask the user to input the values of D, separated by commas, and we split this input into a list. We then loop over each value of D, calculate Q using the given formula, and print the rounded value of Q.

Let's test our code with the example given in the problem: D values are 100, 150, and 180. The output should be 18, 22, 24.

```python
# Test
# Input: 100,150,180
# Expected Output: 18,22,24
```

This problem mainly involves the use of Python's math module, string split method, for loop, and the round function. It's a great exercise to practice these Python concepts.

That's it for today's lesson. I hope you found it helpful. Remember, practice is key in programming. Keep coding, and I'll see you in the next lesson!
