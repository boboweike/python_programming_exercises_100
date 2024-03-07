# Exercise 3(Level 1) ~ Generate Dictionary

Hello everyone, welcome back to our Python programming exercises series. Today we're going to tackle a Level 1 problem, which is perfect for beginners.

Our task today is to write a Python program that takes an integer input, let's call it 'n', and generates a dictionary. This dictionary should contain pairs of numbers, where the key is a number 'i' between 1 and 'n', and the value is the square of 'i'.

Let's dive into the code:

```python
def generate_dict(n):
    # Initialize an empty dictionary
    result = {} # a pair of curly braces indicates an empty dictionary

    # Loop over the range from 1 to n (inclusive)
    for i in range(1, n + 1):
        # Add the pair (i, i*i) to the dictionary
        result[i] = i * i

    # Return the resulting dictionary
    return result

# Test the function with an example input
print(generate_dict(8))
```

In this code, we first initialize an empty dictionary. Then, we loop over the range from 1 to 'n', and for each number 'i' in this range, we add a pair to the dictionary where the key is 'i' and the value is 'i' squared. Finally, we return the resulting dictionary.

When we test this function with the input 8, it correctly outputs the dictionary {1: 1, 2: 4, 3: 9, 4: 16, 5: 25, 6: 36, 7: 49, 8: 64}.

This exercise is a great way to practice using Python's built-in data structures, specifically dictionaries, and also to get comfortable with loops and arithmetic operations.

That's it for today's lesson. I hope you found it helpful and interesting. Stay tuned for more Python exercises!
