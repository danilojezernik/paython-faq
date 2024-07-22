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

## 15. What is the purpose of the `break` statement in loops?

## 16. What is the purpose of the `continue` statement in loops?

## 17. How do you define a function in Python?

## 18. What are default arguments in Python functions?

## 19. How do you return values from a function?
