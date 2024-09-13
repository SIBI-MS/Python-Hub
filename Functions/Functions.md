# Basic Python Functions
<div align="center">

  <!-- LinkedIn Badge -->
  <a href="https://www.linkedin.com/in/sibi-m-s/" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-Sibi_M_S-0077B5?style=flat&logo=linkedin" alt="LinkedIn Badge">
  </a>

  <!-- Twitter Badge -->
  <a href="https://twitter.com/SIBI_M_S" target="_blank">
    <img src="https://img.shields.io/twitter/follow/SIBI_M_S?style=flat&logo=twitter" alt="Twitter Follow">
  </a>

  <br>
  <sub>Author: <a href="https://www.linkedin.com/in/sibi-m-s/" target="_blank">Sibi M. S.</a></sub>

</div>


</div>
<p align="center">
  <img src="https://github.com/SIBI-MS/Python-Hub/blob/main/Assets/python.jpg" alt="Sublime's custom image"/>
</p>

To add an image as the front page at the top of your Markdown files, you can use the Markdown syntax for embedding images. Here’s how you can do it:

1. **Upload the Image**: First, make sure your image is uploaded to your GitHub repository or hosted somewhere online. If you’re uploading to GitHub, you can do so by adding the image to your repository (e.g., in an `assets` or `images` folder).

2. **Use Markdown to Embed the Image**: Add the image to the top of your `.md` file using the Markdown image syntax.

Here’s how you can modify your `basic_functions.md` and `advanced_functions.md` files to include an image at the top:

### **File 1: `basic_functions.md`**


# Basic Python Functions

![Front Page Image](https://github.com/SIBI-MS/your-repo-path/assets/front-page-image.png)

Welcome to the Basic Python Functions guide. This document covers fundamental concepts of Python functions.

## Table of Contents
1. [What is a Function?](#what-is-a-function)
2. [Defining and Calling Functions](#defining-and-calling-functions)
3. [Function Parameters](#function-parameters)
4. [Return Statement](#return-statement)
5. [Default Parameters](#default-parameters)
6. [Scope of Variables](#scope-of-variables)
7. [Practice Questions](#practice-questions)

## What is a Function?
A function is a block of code that performs a specific task. Functions help break down code into smaller, manageable parts, making it reusable and organized.

### Example
```python
def greet():
    print("Hello, world!")

# Call the function
greet()
```

## Defining and Calling Functions
You can define a function using the `def` keyword, followed by the function name and parentheses. To execute a function, you "call" it by its name.

### Example
```python
def add(a, b):
    return a + b

result = add(3, 5)
print(result)  # Output: 8
```

## Function Parameters
Functions can accept inputs (parameters). You can pass values to these parameters when calling the function.

### Example
```python
def greet_person(name):
    print(f"Hello, {name}!")

greet_person("Alice")
```

## Return Statement
Functions can return values using the `return` statement.

### Example
```python
def square(number):
    return number * number

result = square(4)
print(result)  # Output: 16
```

## Default Parameters
You can set default values for function parameters. If the argument is not provided, the default value is used.

### Example
```python
def greet(name="Guest"):
    print(f"Hello, {name}!")

greet()           # Output: Hello, Guest!
greet("Sibi")     # Output: Hello, Sibi!
```

## Scope of Variables
Variables defined inside a function are local to that function and cannot be accessed outside of it.

### Example
```python
def demo_scope():
    x = 10  # Local variable
    print(x)

demo_scope()
# print(x)  # Error: 'x' is not defined outside the function
```

## Practice Questions

1. Write a function that takes two numbers as arguments and returns their product.
2. Define a function that prints whether a number is odd or even.
3. Write a function that takes a string as input and returns the length of the string.
4. Create a function that checks if a number is prime or not.
   - *Hint: Use a loop to check if the number is divisible by any number other than 1 and itself.*
5. Write a function that converts Celsius to Fahrenheit.
   - *Hint: Use the formula `F = (C * 9/5) + 32`.*
6. Define a function that returns the factorial of a number.
   - *Hint: Factorial of `n` is `n * (n-1) * ... * 1`. Use a loop or recursion.*
7. Create a function that counts the vowels in a given string.
8. Write a function that reverses a string and returns it.
9. Write a function that takes a list of numbers and returns the sum of all the elements.
10. Define a function that finds the largest number in a list.
   - *Hint: Iterate through the list and keep track of the maximum value.*
```

### **File 2: `advanced_functions.md`**

```
# Advanced Python Functions

![Front Page Image](https://github.com/SIBI-MS/your-repo-path/assets/front-page-image.png)

Welcome to the Advanced Python Functions guide. This document covers more complex concepts of Python functions.

## Table of Contents
1. [Lambda Functions](#lambda-functions)
2. [*args and **kwargs](#args-and-kwargs)
3. [Recursive Functions](#recursive-functions)
4. [Higher-Order Functions](#higher-order-functions)
5. [Function Annotations](#function-annotations)
6. [Closures and Nested Functions](#closures-and-nested-functions)
7. [Decorators](#decorators)
8. [Practice Questions](#practice-questions)

## Lambda Functions
Lambda functions are small anonymous functions defined using the `lambda` keyword. They can take any number of arguments but have only one expression.

### Example
```python
# Regular function
def add(a, b):
    return a + b

# Lambda function
add_lambda = lambda a, b: a + b

print(add_lambda(3, 5))  # Output: 8
```

## *args and **kwargs
The `*args` and `**kwargs` allow you to pass a variable number of arguments to a function.

### Example (*args)
```python
def sum_all(*args):
    return sum(args)

print(sum_all(1, 2, 3, 4))  # Output: 10
```

### Example (**kwargs)
```python
def greet_all(**kwargs):
    for key, value in kwargs.items():
        print(f"{key} is {value}")

greet_all(name="Alice", age=25)
```

## Recursive Functions
A recursive function is a function that calls itself to solve a problem.

### Example
```python
def factorial(n):
    if n == 1:
        return 1
    else:
        return n * factorial(n-1)

print(factorial(5))  # Output: 120
```

## Higher-Order Functions
Higher-order functions are functions that take other functions as arguments or return functions as their result.

### Example
```python
def apply_twice(func, value):
    return func(func(value))

def add_five(x):
    return x + 5

print(apply_twice(add_five, 10))  # Output: 20
```

## Function Annotations
Function annotations allow you to add metadata to function parameters and return values.

### Example
```python
def greet(name: str) -> str:
    return f"Hello, {name}!"

print(greet("Alice"))
```

## Closures and Nested Functions
A closure is a function object that remembers values in enclosing scopes, even if those scopes are no longer present.

### Example
```python
def outer_function(msg):
    def inner_function():
        print(msg)
    return inner_function

my_func = outer_function("Hello")
my_func()  # Output: Hello
```

## Decorators
Decorators are functions that modify the behavior of another function.

### Example
```python
def decorator_function(original_function):
    def wrapper_function():
        print("Wrapper executed before", original_function.__name__)
        return original_function()
    return wrapper_function

@decorator_function
def display():
    print("Display function executed")

display()
```

## Practice Questions

1. Write a lambda function that squares a number.
2. Create a function that accepts any number of arguments and returns their average.
   - *Hint: Use `*args` to accept multiple arguments.*
3. Define a recursive function to calculate the Fibonacci sequence up to the nth term.
4. Write a function that uses a decorator to log the execution time of another function.
   - *Hint: Use `time.time()` to calculate the duration.*
5. Implement a closure that captures a variable and uses it in a nested function.
6. Define a higher-order function that accepts a function and a value, then calls the function twice on that value.
7. Create a recursive function to reverse a string.
8. Write a function that uses `**kwargs` to print user details (name, age, city).
9. Implement a decorator that prevents a function from being called more than once.
10. Write a function annotation that indicates a function takes two integers and returns a string.
```

---

