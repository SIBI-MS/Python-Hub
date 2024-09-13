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
Defining and Calling Functions
You can define a function using the def keyword, followed by the function name and parentheses. To execute a function, you "call" it by its name.

Example
python
Copy code
def add(a, b):
    return a + b

result = add(3, 5)
print(result)  # Output: 8
Function Parameters
Functions can accept inputs (parameters). You can pass values to these parameters when calling the function.

Example
python
Copy code
def greet_person(name):
    print(f"Hello, {name}!")

greet_person("Alice")
Return Statement
Functions can return values using the return statement.

Example
python
Copy code
def square(number):
    return number * number

result = square(4)
print(result)  # Output: 16
Default Parameters
You can set default values for function parameters. If the argument is not provided, the default value is used.

Example
python
Copy code
def greet(name="Guest"):
    print(f"Hello, {name}!")

greet()           # Output: Hello, Guest!
greet("Sibi")     # Output: Hello, Sibi!
Scope of Variables
Variables defined inside a function are local to that function and cannot be accessed outside of it.

Example
python
Copy code
def demo_scope():
    x = 10  # Local variable
    print(x)

demo_scope()
# print(x)  # Error: 'x' is not defined outside the function
Practice Questions
Write a function that takes two numbers as arguments and returns their product.
Define a function that prints whether a number is odd or even.
Write a function that takes a string as input and returns the length of the string.
Create a function that checks if a number is prime or not.
Hint: Use a loop to check if the number is divisible by any number other than 1 and itself.
Write a function that converts Celsius to Fahrenheit.
Hint: Use the formula F = (C * 9/5) + 32.
Define a function that returns the factorial of a number.
Hint: Factorial of n is n * (n-1) * ... * 1. Use a loop or recursion.
Create a function that counts the vowels in a given string.
Write a function that reverses a string and returns it.
Write a function that takes a list of numbers and returns the sum of all the elements.
Define a function that finds the largest number in a list.
Hint: Iterate through the list and keep track of the maximum value.
