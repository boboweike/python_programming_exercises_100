Hello everyone, welcome back to our Python programming exercises series. Today we're going to tackle a new challenge. This one is about classes in Python, a fundamental concept in object-oriented programming.

Our task is to define a class with at least two methods. The first method, `get_string`, will get a string from console input. The second method, `print_string`, will print the string in upper case.

Let's dive into the code!

```python
class MyClass:
    def __init__(self): # has two underscores on each side
        self.my_string = ""

    def get_string(self):
        self.my_string = input("Please enter a string: ")

    def print_string(self):
        print(self.my_string.upper())
```

In this code, we first define our class `MyClass`. Inside, we have an `__init__` method, which is a special method in Python classes known as a constructor. This method is called when an object is created from the class and it allows the class to initialize the attributes of the class.

We then define our two methods. `get_string` uses the `input` function to get console input and assigns it to `my_string`. `print_string` prints `my_string` in upper case using the `upper` method.

Let's test our class:

```python
test = MyClass()
test.get_string()
test.print_string()
```

In this test, we first create an object `test` of `MyClass`. We then call the `get_string` method to get the input and `print_string` to print it in upper case.

And that's it for this exercise! We've learned about Python classes, methods, the `input` function, and the `upper` method.

That's it for today's lesson. I hope you found it helpful. Stay tuned for more Python exercises!
