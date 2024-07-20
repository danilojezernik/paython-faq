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

Python supports a variety of arithmetic operations that can be performed using standard operators. Here are the basic arithmetic operations you can perform in Python:

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

5. **Floor Division (`//`)**: Divides the first number by the second number and returns the integer part of the quotient.
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

## 6. What is the difference between `print()` and `input()` functions?

## 7. How do you create a list in Python?

## 8. How do you access elements from a list?

## 9. What are tuples and how are they different from lists?