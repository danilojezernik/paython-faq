## 10. How do you create a dictionary in Python?

Dictionaries in Python are collections of key-value pairs. They are mutable, which means you can change, add, or remove
items. Here are various methods to create and work with dictionaries:

### Creating a Dictionary

#### 1. Using Curly Braces

You can create a dictionary by enclosing key-value pairs within curly braces {}.

```python
# Creating a dictionary with initial key-value pairs
my_dict = {
    "name": "Alice",
    "age": 25,
    "city": "New York"
}

print(my_dict)  # Output: {'name': 'Alice', 'age': 25, 'city': 'New York'}
```

#### 2. Using the dict() Constructor

The dict() constructor can create dictionaries from keyword arguments or a list of tuples.

```python
# Using keyword arguments
my_dict = dict(name="Alice", age=25, city="New York")

print(my_dict)  # Output: {'name': 'Alice', 'age': 25, 'city': 'New York'}

# Using a list of tuples
my_dict = dict([("name", "Alice"), ("age", 25), ("city", "New York")])

print(my_dict)  # Output: {'name': 'Alice', 'age': 25, 'city': 'New York'}
```

#### 3. Creating an Empty Dictionary

You can create an empty dictionary and add key-value pairs later.

```python
# Creating an empty dictionary
my_dict = {}

# Adding key-value pairs
my_dict["name"] = "Alice"
my_dict["age"] = 25
my_dict["city"] = "New York"

print(my_dict)  # Output: {'name': 'Alice', 'age': 25, 'city': 'New York'}
```

#### 4. Dictionary Comprehension

Dictionary comprehension is a concise way to create dictionaries.

```python
# Creating a dictionary with comprehension
squares = {x: x * x for x in range(1, 6)}

print(squares)  # Output: {1: 1, 2: 4, 3: 9, 4: 16, 5: 25}
```

#### Using fromkeys()

The fromkeys() method creates a new dictionary with specified keys and a common value.

```python
# Create a dictionary with the same value for all keys
keys = ["name", "age", "city"]
my_dict = dict.fromkeys(keys, "unknown")

print(my_dict)  # Output: {'name': 'unknown', 'age': 'unknown', 'city': 'unknown'}
```

### Accessing and Modifying Dictionary Elements

#### Accessing Values

You can access dictionary values using keys inside square brackets [] or the get() method.

```python
my_dict = {"name": "Alice", "age": 25, "city": "New York"}

# Using square brackets
print(my_dict["name"])  # Output: Alice

# Using get() method
print(my_dict.get("age"))  # Output: 25
```

#### Modifying Values

To modify a value, assign a new value to an existing key.

```python
my_dict["age"] = 26
print(my_dict)  # Output: {'name': 'Alice', 'age': 26, 'city': 'New York'}
```

#### Adding and Removing Elements

You can add new key-value pairs or remove existing ones.

```python
# Adding a new key-value pair
my_dict["country"] = "USA"
print(my_dict)  # Output: {'name': 'Alice', 'age': 26, 'city': 'New York', 'country': 'USA'}

# Removing a key-value pair using del
del my_dict["city"]
print(my_dict)  # Output: {'name': 'Alice', 'age': 26, 'country': 'USA'}

# Removing a key-value pair using pop()
age = my_dict.pop("age")
print(age)  # Output: 26
print(my_dict)  # Output: {'name': 'Alice', 'country': 'USA'}
```

### Summary

Summary
Dictionaries in Python are versatile and efficient for storing and retrieving values based on keys. You can create
dictionaries using curly braces, the `dict()` constructor, or dictionary comprehension. Dictionaries can be accessed and
modified using keys, and elements can be added or removed as needed. This flexibility makes dictionaries a powerful tool
in Python programming.

## 11. How do you access values from a dictionary?

In Python, you can access values from a dictionary using keys. Here are the various methods to access values from a
dictionary:

### 1. Using Square Brackets

You can access the value of a specific key by placing the key inside square brackets [].

```python
my_dict = dict(name="Alice", age=25, city="New York")

# Accessing values using square brackets
name = my_dict["name"]
age = my_dict["age"]
city = my_dict["city"]

print(name)  # Output: Alice
print(age)  # Output: 25
print(city)  # Output: New York
```

### 2. Using the get() Method

The `get()` method returns the value for the specified key if the key is in the dictionary. If the key is not found, it
returns `None` or a specified default value.

```python
my_dict = dict(name="Alice", age=25, city="New York")

# Accessing values using the get() method
name = my_dict.get("name")
age = my_dict.get("age")
city = my_dict.get("city")

print(name)  # Output: Alice
print(age)  # Output: 25
print(city)  # Output: New York

# Using get() with a default value
country = my_dict.get("country", "Unknown")
print(country)  # Output: Unknown
```

### 3. Accessing Values in a Loop

You can iterate over the keys or items of the dictionary to access all values.

#### Iterating over keys

```python
my_dict = dict(name="Alice", age=25, city="New York")

# Iterating over keys to access values
for key in my_dict:
    print(f"{key}: {my_dict[key]}")

# Output: 
# name: Alice 
# age: 25
# city: New York
```

#### Iterating over keys-value pairs

```python
my_dict = dict(name="Alice", age=25, city="New York")

# Iterating over key-value pairs
for key, value in my_dict.items():
    print(f"{key}: {value}")

# Output: 
# name: Alice 
# age: 25
# city: New York
```

### 4. Using Dictionary Views

Python provides dictionary view objects that allow you to access keys, values, and key-value pairs.

#### Accessing All Values

```python
my_dict = dict(name="Alice", age=25, city="New York")

# Accessing all values useing values() method
values = my_dict.values()
print(values)  # Output: dict_values(['Alice', 25, 'New York'])

# Iterating over all values
for value in values:
    print(value)

# Output:
# Alice
# 25
# New York
```

### Summary

- **Square Brackets `[]`**: Direct access using a key. Raises `KeyError` if the key is not found.
- **get() Method**: Safe access using a key. Returns `None` or a specified default value if the key is not found.
- **Loops**: Iterating over keys or key-value pairs to access values.
- **Dictionary Views**: Using `values()` method to access all values at once.

## 12. What are the conditional statements in Python?

In Python, conditional statements allow you to execute certain blocks of code based on whether a condition is true or
false. The primary conditional statements are `if`, `elif`, and `else`. Here’s a detailed explanation of each:

### `if` Statement

The `if` statement checks a condition and executes the block of code inside it if the condition is true.

```python
x = 10
if x > 5:
    print("x is greater than 5")
```

### `elif` Statement

The `elif` (short for "else if") statement allows you to check multiple conditions, executing the block of code inside
it
if its condition is true and all preceding conditions are false.

```python
x = 10
if x > 15:
    print("x is greater than 15")
elif x > 5:
    print("x is greater than 5 but less than or equal to 15")
```

### `else` Statement

The `else` statement is used to execute a block of code if all preceding conditions are false.

```python
x = 3
if x > 15:
    print("x is greater than 15")
elif x > 5:
    print("x is greater than 5 but less than or equal to 15")
else:
    print("x is 5 or less")
```

### Nested Conditional Statements

You can nest conditional statements inside other conditional statements.

```python
x = 10
if x > 5:
    print("x is greater than 5")
    if x > 8:
        print("x is also greater than 8")
    else:
        print("x is 6, 7, or 8")
```

### Conditional Expressions (Ternary Operator)

Python also supports conditional expressions, which are a shorthand way of writing an `if-else` statement.

```python
x = 10
result = "x is greater than 5" if x > 5 else "x is 5 or less"
print(result)  # Output: x is greater than 5
```

### Logical Operators in Conditional Statements

You can use logical operators to combine multiple conditions:

- **and**: True if both conditions are true.
- **or**: True if at least one condition is true.
- **not**: Inverts the truth value.

```python
x = 10
y = 20

if x > 5 and y > 15:
    print("x is greater than 5 and y is greater than 15")

if x > 15 or y > 15:
    print("Either x is greater than 15 or y is greater than 15")

if not x < 5:
    print("x is not less than 5")
```

### Summary

- `if`: Executes a block of code if a condition is true.
- `elif`: Checks another condition if all previous conditions are false.
- `else`: Executes a block of code if all previous conditions are false.
- **Nested Conditional Statements**: Conditional statements within other conditional statements.
- **Conditional Expressions**: Shorthand way of writing `if-else` statements.
- **Logical Operators**: Combine multiple conditions using `and`, `or`, and `not`.

These conditional statements and techniques allow you to control the flow of your program based on various conditions.

## 13. How do you write a for loop in Python?

In Python, `for` loops are used to iterate over a sequence (such as a list, tuple, string, or range). Here’s a detailed
explanation of how to write and use `for` loops:

### Basic `for` Loop

A basic for loop iterates over each item in a sequence and executes a block of code for each item.

```python
# Iterating over a list
fruits = ["apple", "banana", "cherry"]

for fruit in fruits:
    print(fruit)

# Output:
# apple
# banana
# cherry
```

### Using `range()`

The` range()` function generates a sequence of numbers, which is often used to control the number of times a loop runs.

```python
# Iterate over a range of values
for i in range(5):
    print(i)

# Output:
# 0
# 1
# 2
# 3
# 4
```

#### Specifying Start, Stop, and Step in range()

The `range()` function can take up to three arguments: start, stop, and step.

```python
# Specifying start, stop, and step in range()
for i in range(2, 10, 2):
    print(i)

# Output:
# 2
# 4
# 6
# 8
```

### Iterating Over a String

You can iterate over the characters of a string.

```python
# Iterating over a string
for char in "hello":
    print(char)

# Output:
# h
# e
# l
# l
# o
```

### Iterating Over a Dictionary

You can iterate over the characters of a string.

#### Iterating Over Keys

```python
my_dict = {"name": "Alice", "age": 25, "city": "New York"}
for key in my_dict:
    print(key)

# Output:
# name
# age
# city
```

#### Iterating Over Values

```python
for value in my_dict.values():
    print(value)

# Output:
# Alice
# 25
# New York
```

#### Iterating Over Key-Value Pairs

```python
for key, value in my_dict.items():
    print(f"{key}: {value}")

# Output:
# name: Alice
# age: 25
# city: New York
```

#### Nested for Loops

You can nest for loops to iterate over multi-dimensional sequences.

```python
matrix = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
]

for row in matrix:
    for num in row:
        print(num)

# Output:
# 1
# 2
# 3
# 4
# 5
# 6
# 7
# 8
# 9
```

### Using else with for Loops

An `else` block can be used with a `for` loop. The `else` block executes after the loop completes normally, but not if
the loop is terminated by a `break` statement.

```python
for i in range(5):
    print(i)
else:
    print("Loop completed")

# Output:
# 0
# 1
# 2
# 3
# 4
# Loop completed
```

### Breaking Out of a Loop

You can use the `break` statement to exit a loop prematurely.

```python
for i in range(10):
    if i == 5:
        break
    print(i)

# Output:
# 0
# 1
# 2
# 3
# 4
```

### Continuing to the Next Iteration

You can use the `continue` statement to skip the rest of the code inside the loop for the current iteration and move to
the next iteration.

```python
for i in range(10):
    if i % 2 == 0:
        continue
    print(i)

# Output:
# 1
# 3
# 5
# 7
# 9
```

### Summary

- **Basic `for` Loop**: Iterates over each item in a sequence.
- **Using `range()`**: Generates a sequence of numbers.
- **Specifying Start, Stop, and Step in `range()`**: Controls the range of numbers iterated over.
- **Iterating Over a String**: Iterates over characters in a string.
- **Iterating Over a Dictionary**: Iterates over keys, values, or key-value pairs.
- **Nested `for` Loops**: Iterates over multi-dimensional sequences.
- **Using `else` with `for` Loops**: Executes after the loop completes normally.
- **Breaking Out of a Loop**: Exits a loop prematurely with `break`.
- **Continuing to the Next Iteration**: Skips the rest of the code for the current iteration with `continue`.

These features make `for` loops in Python powerful and flexible for various iteration tasks.

## 14. How do you write a while loop in Python?

In Python, a `while` loop repeatedly executes a block of code as long as a specified condition is true. Here’s a
detailed
explanation of how to write and use `while` loops:

### Basic `while` Loop

A basic `while` loop continues to run as long as the condition is true.

```python
x = 0
while x < 5:
    print(x)
    x += 1

# Output:
# 0
# 1
# 2
# 3
# 4
```

### Using `break` to Exit the Loop

The `break` statement can be used to exit the loop prematurely when a certain condition is met.

```python
x = 0
while x < 10:
    if x == 5:
        break
    print(x)
    x += 1

# Output:
# 0
# 1
# 2
# 3
# 4
```

### Using `continue` to Skip an Iteration

The `continue` statement skips the rest of the code inside the loop for the current iteration and moves to the next
iteration.

```python
x = 0
while x < 10:
    x += 1
    if x % 2 == 0:
        continue
    print(x)

# Output:
# 1
# 3
# 5
# 7
# 9
```

### Using `else` with `while` Loop

An `else` block can be used with a `while` loop. The `else` block is executed when the condition becomes false, but not
if the loop is terminated by a `break` statement.

```python
x = 0
while x < 5:
    print(x)
    x += 1
else:
    print("Loop completed")

# Output:
# 0
# 1
# 2
# 3
# 4
# Loop completed
```

### Infinite Loop

A `while` loop can run indefinitely if the condition always remains true. Make sure to include a mechanism to break out
of such loops to avoid infinite execution.

```python
x = 0
while True:
    print(x)
    x += 1
    if x == 10:
        break

# Output:
# 1
# 2
# 3
# 4
# 5
# 6
# 7
# 8
# 9
```

### Nested `while` Loop

You can nest `while` loops to handle more complex conditions.

```python
x = 0
while x < 3:
    y = 0
    while y < 3:
        print(f"x: {x}, y: {y}")
        y += 1
    x += 1

# output:
# x: 0, y: 0
# x: 0, y: 1
# x: 0, y: 2
# x: 1, y: 0
# x: 1, y: 1
# x: 1, y: 2
# x: 2, y: 0
# x: 2, y: 1
# x: 2, y: 2
```

### Summary

- **Basic `while` Loop**: Repeats a block of code as long as the condition is true.
- **Using `break`**: Exits the loop prematurely when a specific condition is met.
- **Using `continue`**: Skips the rest of the code for the current iteration and moves to the next iteration.
- **Using `else` with `while` Loop**: Executes after the loop condition becomes false, unless exited by `break`.
- **Infinite Loop**: Runs indefinitely unless interrupted by a break statement or external intervention.
- **Nested `while` Loop**: Handles more complex conditions by nesting loops.

## 15. What is the purpose of the `break` statement in loops?

The `break` statement in Python is used to exit a loop prematurely. When a `break` statement is encountered inside a
loop, the loop is immediately terminated, and the program control is transferred to the statement following the loop.
This is useful for stopping the loop when a certain condition is met, regardless of whether the loop would normally
terminate.

### Example of break in a for loop

```python
for i in range(10):
    if i == 5:
        break
    print(i)

# Output:
# 0
# 1
# 2
# 3
# 4
```

### Example of break in a while loop

```python
x = 0
while x < 10:
    if x == 5:
        break
    print(x)
    x += 1

# Output:
# 0
# 1
# 2
# 3
# 4
```

## 16. What is the purpose of the `continue` statement in loops?

The continue statement in Python is used to skip the rest of the code inside the current iteration of a loop and proceed
to the next iteration. When a continue statement is encountered, the remaining code inside the loop for that particular
iteration is ignored, and the loop moves to the next iteration. This is useful for skipping specific conditions or
iterations within the loop.

### Example of continue in a for loop

```python
for i in range(10):
    if i % 2 == 0:  # Skip even numbers
        continue
    print(i)

# Output:
# 1
# 3
# 5
# 7
# 9
```

### Example of continue in a while loop

```python
x = 0
while x < 10:
    x += 1
    if x % 2 == 0:  # Skip even numbers
        continue
    print(x)

# Output:
# 1
# 3
# 5
# 7
# 9
```

## 17. How do you define a function in Python?

In Python, you define a function using the `def` keyword, followed by the function name, parentheses `()`, and a
colon `:`. The function body contains the code that executes when the function is called, and it is indented to indicate
that it is part of the function. Here’s a detailed explanation of how to define and use functions in Python:

### Basic Function Definition

A basic function definition includes the def keyword, the function name, and the function body.

```python
def greet():
    print("Hello World!")
```

### Calling a Function

To execute the code inside a function, you call the function by its name followed by parentheses.

```python
greet()  # Output: Hello, world!
```

### Function with Parameters

You can define a function that takes parameters, which allows you to pass values to the function.

```python
def greet(name):
    print(f"Hello, {name}!")


greet("Alice")  # Output: Hello, Alice!
```

### Function with Default Parameters

You can define default values for parameters. If the function is called without arguments, the default values are used.

```python
def greet(name="world"):
    print(f"Hello, {name}!")


greet()  # Output: Hello, world!
greet("Alice")  # Output: Hello, Alice!
```

### Function with Variable-Length Arguments

You can define functions that accept an arbitrary number of arguments using `*args` for positional arguments and **
kwargs
for keyword arguments.

#### Positional Arguments

```python
def greet(*names):
    for name in names:
        print(f"Hello, {name}!")


greet("Alice", "Bob", "Charlie")

# Output:
# Hello, Alice!
# Hello, Bob!
# Hello, Charlie!
```

#### Keyword Arguments

```python
def describe_person(**info):
    for key, value in info.items():
        print(f"{key}: {value}")


describe_person(name="Alice", age=30, city="New York")

# Output:
# name: Alice
# age: 30
# city: New York
```

### Nested Functions

You can define functions inside other functions.

```python
def outer_function(text):
    def inner_function():
        print(text)

    inner_function()


outer_function("Hello from outer function!")  # Output: Hello from outer function!
```

### Lambda Functions

Python also supports anonymous functions, known as lambda functions, which are defined using the lambda keyword.

```python
add = lambda a, b: a + b
print(add(3, 5))  # Output: 8
```

### Summary

- **Basic Function**: Defined using `def`, followed by the function name and body.
- **Parameters**: Functions can take parameters to accept input values.
- **Return Value**: Functions can return values using the return statement.
- **Default Parameters**: Functions can have default values for parameters.
- **Variable-Length Arguments**: Use `*args` for positional and **kwargs for keyword arguments to accept arbitrary
  numbers of arguments.
- **Nested Functions**: Functions can be defined within other functions.
- **Lambda Functions**: Anonymous functions defined using the lambda keyword.

## 18. What are default arguments in Python functions?

In Python, default arguments are values that are provided in a function definition, which are used if no corresponding
argument is passed during the function call. This allows functions to have flexible interfaces and provide default
behavior for certain parameters.

## 19. How do you return values from a function?
