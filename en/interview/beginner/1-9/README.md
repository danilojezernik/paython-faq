## 1. What is Python and what are its key features?

Python is a high-level, interpreted programming language known for its readability and simplicity. It was created by
Guido van Rossum and first released in 1991. Python supports multiple programming paradigms, including procedural,
object-oriented, and functional programming. Its syntax allows developers to express concepts in fewer lines of code
compared to languages like C++ or Java.

### Key Features of Python:

1. **Easy to Read, Learn, and Write**: Python's syntax is clear and intuitive, making it an excellent choice for
   beginners.
2. **Interpreted Language**: Python code is executed line by line, which makes debugging easier and code testing more
   efficient.
3. **Dynamically Typed**: You don't need to declare the type of a variable; the type is determined at runtime.
4. **Extensive Standard Library**: Python has a rich standard library that supports many common programming tasks like
   file I/O, system calls, and data manipulation.
5. **Portability**: Python code can run on various operating systems like Windows, macOS, and Linux without requiring
   changes.
6. **Extensibility**: Python can be extended with modules written in C or C++, enabling performance-critical tasks.
7. **Support for Multiple Programming Paradigms**: Python supports procedural, object-oriented, and functional
   programming paradigms.
8. **Community Support**: Python has a large and active community, which contributes to a wealth of resources,
   libraries, and frameworks.
9. **Third-Party Packages**: The Python Package Index (PyPI) hosts thousands of third-party packages that extend
   Python's capabilities.
10. **Strong Integration Capabilities**: Python can easily integrate with other languages and technologies, such as
    Java, C, and C++.

These features make Python a versatile language suitable for a wide range of applications, including web development,
data analysis, artificial intelligence, scientific computing, and automation.

## 2. How do you write and execute a simple Python script?

### Writing a Simple Python Script

1. **Open a Text Editor**: You can use any text editor (e.g., VSCode, Sublime Text, Notepad++) or an Integrated
   Development Environment (IDE) like PyCharm.

2. **Write Your Python Code**: Write a simple Python script. For example, create a file named `hello.py` and add the
   following code:
    ```python
    print("Hello, World!")
    ```

### Executing a Simple Python Script

1. **Open a Terminal or Command Prompt**:
    - On Windows, you can open Command Prompt by pressing `Win + R`, typing `cmd`, and pressing Enter.
    - On macOS or Linux, you can open Terminal from the Applications folder or by pressing `Ctrl + Alt + T`.

2. **Navigate to the Directory Containing Your Script**: Use the `cd` command to change the directory. For example:
    ```sh
    cd path/to/your/script
    ```

3. **Run the Python Script**: Execute the script by typing `python` (or `python3` depending on your installation)
   followed by the script name. For example:
    ```sh
    python hello.py
    ```
   or
    ```sh
    python3 hello.py
    ```

### Example:

1. **Write the Script**:
    ```python
    # hello.py
    print("Hello, World!")
    ```

2. **Navigate to the Directory**:
    ```sh
    cd path/to/your/script
    ```

3. **Execute the Script**:
    ```sh
    python hello.py
    ```

### Output:

```sh
Hello, World!
```

This will print Hello, World! to the terminal, confirming that your script executed successfully.

## 3. What are variables in Python and how do you declare them?

### Variables in Python

Variables are used to store data that can be referenced and manipulated in a program. They act as placeholders for
values and can be used to perform operations on the stored data.

### Declaring Variables in Python

In Python, declaring a variable is simple and straightforward. You do not need to specify the type of the variable
explicitly. The type is inferred from the value assigned to the variable. Here are the steps and examples to declare
variables in Python:

1. **Assign a Value to a Variable**: Use the `=` operator to assign a value to a variable.
    ```python
    variable_name = value
    ```

### Examples

1. **Declaring an Integer Variable**:
    ```python
    age = 25
    ```

2. **Declaring a Floating-Point Variable**:
    ```python
    temperature = 36.6
    ```

3. **Declaring a String Variable**:
    ```python
    name = "Alice"
    ```

4. **Declaring a Boolean Variable**:
    ```python
    is_student = True
    ```

### Rules for Naming Variables

- Variable names must start with a letter (a-z, A-Z) or an underscore (_).
- The rest of the variable name can include letters, numbers (0-9), and underscores.
- Variable names are case-sensitive (e.g., `age` and `Age` are different variables).
- Avoid using Python reserved keywords (e.g., `class`, `for`, `if`, etc.) as variable names.

### Examples of Valid and Invalid Variable Names

1. **Valid Variable Names**:
    ```python
    my_var = 10
    _my_var = 20
    myVar123 = 30
    ```

2. **Invalid Variable Names**:
    ```python
    1st_var = 10  # Invalid: cannot start with a number
    my-var = 20   # Invalid: cannot contain hyphens
    class = 30    # Invalid: cannot use reserved keywords
    ```

### Example Usage:

```python
# Declaring variables
age = 25
temperature = 36.6
name = "Alice"
is_student = True

# Using variables
print("Name:", name)
print("Age:", age)
print("Temperature:", temperature)
print("Is Student:", is_student)
```

### Output:

```vbnet
Name: Alice
Age: 25
Temperature: 36.6
Is Student: True
```

## 4. What are the different data types in Python?

Python supports various data types, which are used to define the type of a variable. These data types can be broadly
categorized into the following:

### 1. Numeric Types

- **Integer (`int`)**: Represents whole numbers, both positive and negative.
  ```python
  age = 25
  ```
- **Floating-Point (`float`)**: Represents real numbers with a fractional part.
   ```python
   temperature = 36.6
   ```
- **Complex (`complex`)**: Represents complex numbers with real and imaginary parts.
   ```python
   temperature = 36.6
   ```

### 2. Sequence Types

- **String (`str`)**: Represents a sequence of characters.
  ```python
  name = "Alice"
  ```
- **List (`list`)**: Represents an ordered collection of items, which can be of different types.
   ```python
   fruits = ["apple", "banana", "cherry"]
   ```
- Tuple (tuple): Represents an ordered collection of items, which are immutable.
   ```python
   coordinates = (10, 20)
   ```

### 3. Mapping Type

- **Dictionary (`dict`)**: Represents a collection of key-value pairs.
  ```python
  student = {"name": "Alice", "age": 25}
  ```

### 4. Set Types

- **Set (`set`)**: Represents an unordered collection of unique items.
  ```python
  unique_numbers = {1, 2, 3, 4}
  ```
- **Frozen Set (`frozenset`)**: Represents an immutable set.
  ```python
  frozen_numbers = frozenset([1, 2, 3, 4])
  ```

### 5. Boolean Type

- **Boolean (bool)**: Represents two values: `True` and `False`.
  ```python
  student = {"name": "Alice", "age": 25}
  ```

### 6. None Type

- **NoneType (`None`)**: Represents the absence of a value.
  ```python
  data = None
  ```

### Example Code:

```python
# Numeric Types
age = 25  # int
temperature = 36.6  # float
complex_number = 3 + 4j  # complex

# Sequence Types
name = "Alice"  # str
fruits = ["apple", "banana", "cherry"]  # list
coordinates = (10, 20)  # tuple

# Mapping Type
student = {"name": "Alice", "age": 25}  # dict

# Set Types
unique_numbers = {1, 2, 3, 4}  # set
frozen_numbers = frozenset([1, 2, 3, 4])  # frozenset

# Boolean Type
is_student = True  # bool

# None Type
data = None  # NoneType
```

### Example Usage:

```python
print("Age:", age)  # Age: 25
print("Temperature:", temperature)  # Temperature: 36.6
print("Complex Number:", complex_number)  # Complex Number: (3+4j)
print("Name:", name)  # Name: Alice
print("Fruits:", fruits)  # Fruits: ['apple', 'banana', 'cherry']
print("Coordinates:", coordinates)  # Coordinates: (10, 20)
print("Student:", student)  # Student: {'name': 'Alice', 'age': 25}
print("Unique Numbers:", unique_numbers)  # Unique Numbers: {1, 2, 3, 4}
print("Frozen Numbers:", frozen_numbers)  # Frozen Numbers: frozenset({1, 2, 3, 4})
print("Is Student:", is_student)  # Is Student: True
print("Data:", data)  # Data: None
```

## 5. How do you perform basic arithmetic operations in Python?

Python supports a variety of arithmetic operations that can be performed using standard operators. Here are the basic
arithmetic operations you can perform in Python:

### Basic Arithmetic Operators

1. **Addition (`+`)**: Adds two numbers.
    ```python
    result = 5 + 3  # result is 8
    ```

2. **Subtraction (`-`)**: Subtracts the second number from the first number.
    ```python
    result = 5 - 3  # result is 2
    ```

3. **Multiplication (`*`)**: Multiplies two numbers.
    ```python
    result = 5 * 3  # result is 15
    ```

4. **Division (`/`)**: Divides the first number by the second number and returns a float.
    ```python
    result = 5 / 3  # result is 1.6666666666666667
    ```

5. **Floor Division (`//`)**: Divides the first number by the second number and returns the integer part of the
   quotient.
    ```python
    result = 5 // 3  # result is 1
    ```

6. **Modulus (`%`)**: Returns the remainder when the first number is divided by the second number.
    ```python
    result = 5 % 3  # result is 2
    ```

7. **Exponentiation (`**`)**: Raises the first number to the power of the second number.
    ```python
    result = 5 ** 3  # result is 125
    ```

### Example Code:

```python
# Addition
addition = 5 + 3
print("5 + 3 =", addition)  # 5 + 3 = 8

# Subtraction
subtraction = 5 - 3
print("5 - 3 =", subtraction)  # 5 - 3 = 2

# Multiplication
multiplication = 5 * 3
print("5 * 3 =", multiplication)  # 5 * 3 = 15

# Division
division = 5 / 3
print("5 / 3 =", division)  # 5 / 3 = 1.6666666666666667

# Floor Division
floor_division = 5 // 3
print("5 // 3 =", floor_division)  # 5 // 3 = 1

# Modulus
modulus = 5 % 3
print("5 % 3 =", modulus)  # 5 % 3 = 2

# Exponentiation
exponentiation = 5 ** 3
print("5 ** 3 =", exponentiation)  # 5 ** 3 = 125
```

## 6. What is the difference between `print()` and `input()` functions? What is `flush` and `file` in `print()` function?

The `print()` and `input()` functions in Python are used for different purposes: `print()` is used to display output to
the
user, while `input()` is used to get input from the user.

### `print()` Function

**Purpose**: The `print()` function is used to display information to the console or terminal.

**Syntax**: `print(*objects, sep=' ', end='\n', file=sys.stdout, flush=False)`

**Parameters**:

- `*objects`: The values to be printed. Multiple values can be separated by a comma.
- `sep`: A string inserted between values. Default is a space.
- `end`: A string appended after the last value. Default is a newline (\n).
- `file`: An object with a write(string) method. Default is sys.stdout.
- `flush`: Whether to forcibly flush the stream. Default is False.

### `input()` Function

**Purpose**: The `input()` function is used to get input from the user via the console or terminal.

**Syntax**: `input(prompt=None)`

**Parameters**:

- prompt: A string, representing a message to display to the user before input. Default is `None`.

**Returns**: A string representing the user's input.

### Differences Between `print()` and `input()`

**Functionality**:

- `print()`: Displays information to the console.
- `input()`: Reads information from the user.

**Return Value**:

- `print()`: Returns None.
- `input()`: Returns the user's input as a string.

**Use Case**:

- `print()`: Used when you want to show output to the user.
- `input()`: Used when you need to get input from the user.

### Example Usage

#### print():

- `print("Hello, World!")` will display "Hello, World!" on the console.
- `print("Age:", 25)` will display "Age: 25" on the console.

#### input():

- `name = input("Enter your name: ")` will prompt the user to enter their name.
- `age = input("Enter your age: ")` will prompt the user to enter their age.

### `flush` and `file` Parameter

### `flush` Parameter

- **Purpose**: Controls whether the output buffer is forcibly flushed (written to the terminal or file immediately).
- **Syntax**: `print(*objects, sep=' ', end='\n', file=sys.stdout, flush=False)`
- **Default Value**: `False`

#### Example

```python
import time

# Example with flush set to True. This will show immediately on the console
for i in tange(5):
    print(i, end=' ', flush=True)
    time.sleep(1)
```

### `file` Parameter

- **Purpose**: Specifies where the output should be written. Default is `sys.stdout` (the console).
- **Syntax**: `print(*objects, sep=' ', end='\n', file=sys.stdout, flush=False)`
- **Default Value**: `sys.stdout`

#### Example

```python
# Writing to a file
with open('output.txt', 'w') as file:
    print("Hello, World!", file=file)
```

### Summary

### `flush`:

- Controls immediate flushing of output.
- Useful for real-time logging and progress bars.

### `file`:

- Specifies the output destination.
- Can be redirected to files or other streams like `sys.stderr` which is a built-in file object in Python that is used
  by the interpreter to write error messages.

## 7. How do you create a list in Python?

In Python, you can create a list by enclosing a sequence of elements within square brackets `[]`, separated by commas.
Here are a few examples:

### Creating an empty list

```python
my_list = []
```

### Creating a list with elements

```python
my_list = [1, 2, 3, 4, 5]
```

### Creating a list with mixed data types

```python
my_list = [1, "hello", 3.14, True]
```

### Creating a list using a list comprehension

```python
my_list = [x for x in range(10)]
```

### Creating a nested list (list of lists)

```python
my_list = [[1, 2], [3, 4], [5, 6]]
```

Lists in Python are versatile and can hold elements of different types, including other lists. You can manipulate lists
using various list methods such as `append()`, `extend()`, `insert()`, `remove()`, `pop()`, and more.

## 8. How do you access elements from a list?

To access elements from a list in Python, you use the index of the element you want to access. The index of the first
element is 0, the second element is 1, and so on. Here are some examples:

### Accessing Single Elements

```python
fruits = ["apple", "banana", "cherry"]

# Access the first element
print(fruits[0])  # Output: apple

# Access the second element
print(fruits[1])  # Output: banana

# Access the third element
print(fruits[2])  # Output: cherry
```

### Accessing Elements from the End of the List

You can also use negative indexing to access elements from the end of the list. The index of the last element is -1, the
second-to-last element is -2, and so on:

```python
# Access the last element
print(fruits[-1])  # Output: cherry

# Access the second-to-last element
print(fruits[-2])  # Output: banana

# Access the third-to-last element
print(fruits[-3])  # Output: apple
```

### Slicing Lists

You can access a range of elements from a list using slicing. The syntax is `list[start:end]`, where `start` is the
index of
the first element you want to INCLUDE, and `end` is the index of the first element you want to EXCLUDE.

```python
# Access the first two elements
print(fruits[0:2])  # Output: ['apple', 'banana']

# Access elements from the second to the end
print(fruits[1:])  # Output: ['banana', 'cherry']

# Access all elements
print(fruits[:])  # Output: ['apple', 'banana', 'cherry']
```

### Accessing Elements in a Loop

You can also access elements in a loop:

```python
for fruit in fruits:
    print(fruit)

# This will output each element in the list:
# apple
# banana
# cherry
```

These are the basic ways to access elements in a list in Python. There are other techniques and let's divide them in *
*intermediate** and **advanced** techniques.

### Intermediate

### List comprehension

List comprehension provides a concise way to create lists and can be used to access and manipulate elements.

```python
# Create a new list with lengths of each fruit name
lengths = [len(fruit) for fruit in fruits]
print(lengths)  # Output: [5, 6, 6]
```

### Using the `enumerate` function

The `enumerate` function can be used to access both the index and the value of each element in a list.

```python
for index, fruit in enumerate(fruits):
    print(f"Index: {index}, Fruit: {fruit}")
```

### Advanced

### Using the `zip` function

The `zip` function can be used to iterate over multiple lists in parallel.

```python
fruits = ["apple", "banana", "cherry"]
colors = ["red", "yellow", "red"]

for fruit, color in zip(fruits, colors):
    print(f"The color of {fruit} is {color}")
```

### Using the `map` function

The `map` function applies a given function to all items in an input list.

```python
# Convert all fruit names to uppercase
uppercase_fruits = list(map(str.upper, fruits))
print(uppercase_fruits)  # Output: ["APPLE", "BANANA", "CHERRY"]
```

### Using the `filter` function

The `filter` function creates a list of elements for which a function return true.

```python
# Filter out fruits with names longer than 5 characters
long_fruits = list(filter(lambda x: len(x) > 5, fruits))
print(long_fruits)  # Output: ['banana', 'cherry']
```

### Using the `reduce` function

The `reduce` function from the `functools` module applies a rolling computation to sequential pairs of values in a list.

```python
from functools import reduce

# Concatenate all fruit names into a single string
all_fruits = reduce(lambda x, y: x + y, fruits)
print(all_fruits)  # Output: "applebananacherry"
```

### List slicing with steps

You can access elements at a specific intervals using slicing with step.

```python
# Access every second element
print(fruits[::2])  # Output: ['apple', 'cherry']

# Access the list in revers
print(fruits[::-1])  # Output: ['cherry', 'banana', 'apple']
```

### Nested list comprehension

For more complex list manipulations, nested list comprehensions can be used.

```python
# Create a 2D list (matrix) and flatten it
matrix = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
flattened = [num for row in matrix for num in row]
print(flattened)  # Output: [1, 2, 3, 4, 5, 6, 7, 8, 9]
```

### Access list in multidimensional lists

For multidimensional lists, you can use multiple indices to access elements.

```python
# Access elements in a 2D list (matrix)
matrix = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
print(matrix[1][6])  # Output: 6
```

## 9. What are tuples and how are they different from lists?

Tuples are a data structure in Python that are similar to lists but have some key differences. Here are the main
characteristics and differences between tuples and lists:

### Tuples

- **Immutable**: Once a tuple is created, its elements cannot be changed, added, or removed. This immutability makes
  tuples
  useful for representing fixed collections of items.
- **Ordered**: Tuples maintain the order of elements. The elements can be accessed by their indices.
- **Defined using parentheses**: Tuples are created by placing elements inside parentheses `()`, separated by commas.
- **Can contain mixed data types**: Like lists, tuples can contain elements of different data types (e.g., integers,
  strings, floats).

### Lists

- **Mutable**: Lists are mutable, meaning their elements can be changed, and you can add or remove elements after the
  list is created.
- **Ordered**: Lists maintain the order of the elements, and elements can be accessed by their indices.
- **Defined using square brackets**: Lists are created by placing elements inside square brackets `[]`, separated by
  commas.
- **Can obtain mixed data types**: Lists can also contain mixed data types.

### Example of Tuples and Lists

#### Lists

```python
# Creating a tuple
my_tuple = (1, 2, 3, "apple", "banana")

# Accessing elements
print(my_tuple[0])  # Output: 1
print(my_tuple[3])  # Output: apple

# Tuples are immutable so this would rase an error
# my_tuple[1] = 4 # TypeError: 'tuple' object does not support item assignemnt
```

#### Lists

```python
# Creating a list
my_list = [1, 2, 3, "apple", "banana"]

# Accessing elements
print(my_list[0])  # Output: 1
print(my_list[3])  # Output: apple

# Lists are mutable, so you can change elements
my_list[1] = 4
print(my_list)  # Output: [1, 4, 3, "apple", "banana"]

# You can also add and remove elements from a list
my_list.append("cherry")
print(my_list)  # Output: [1, 4, 3, "apple", "banana", "charry"]

my_list.remove("apple")
print(my_list)  # Output: [1, 4, 3, "banana", "charry"]
```

### When to use `tuples` and when `lists`

#### Tuples:

- Use a tuple when you need a collection of items that should not change throughout the program. For example, use tuples
  to represent fixed collection of data, such as coordinates (x, y), days of the week, or a collection of constants.
- Tuples can be used as keys in dictionaries because they are immutable.

#### Lists:

- Use lists when you need a collection of items that may change, grow, or shrink over time. For example, use lists to
  represent a collection of items that might be modified, such as a list of user inputs, a shopping cart, or a sequence
  of tasks.
- Lists are suitable for operations that involve frequent updates, such as adding or removing elements.