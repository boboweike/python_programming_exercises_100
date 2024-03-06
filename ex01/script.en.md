# Exercise 1(level1)

Hello everyone, welcome to our Python programming exercise series. Are you ready to boost your coding skills? Let's dive into our first exercise.

Our task today is to write a Python program that finds all numbers between 2000 and 3200, inclusive, that are divisible by 7 but not a multiple of 5. We want these numbers to be printed in a comma-separated sequence on a single line. Can you think of how you might approach this problem?

Let's break it down. We need to iterate over a range of numbers from 2000 to 3200. For each number, we'll check if it is divisible by 7 and not a multiple of 5. If it meets these conditions, we'll print it.

Let'me write some Python code to illustrate the solution:

```python
def find_numbers():
    # Create an empty list to store the numbers
    result = [] # square brackets

    # Iterate over the range of numbers
    for num in range(2000, 3201):  # We go up to 3201 because range's end is exclusive
        # Check if the number is divisible by 7 and not a multiple of 5
        if num % 7 == 0 and num % 5 != 0:
            # Append the number to the result list
            result.append(str(num))

    # Print the numbers in a comma-separated sequence
    print(', '.join(result))

# Call the function
find_numbers()
```

Let me re-summarize the code here. In this function, `find_numbers`, we first create an empty list `result` to store the numbers that meet our conditions. We then iterate over the range of numbers, and for each number that is divisible by 7 and not a multiple of 5, we add it to the `result` list. Finally, we join the numbers in the `result` list with a comma and print them out.

Let's run the code. You can see that it prints out numbers like 2002, 2009, 2016, all the way up to 3199. These numbers are exactly what we expected.

So in today's exercise, we've explored Python's `range` function, `for` loops, `if` statements, and `join` method on string. We've also seen how to use the modulus operator `%` to check divisibility. These are fundamental concepts that you'll use over and over in Python programming.

That's it for today's exercise. I hope you found it useful. Keep practicing and stay tuned for more Python exercises that will sharpen your coding skills. Happy coding, and see you in the next one!
