# freecodecamp-python-certification
## Understanding Variables and Data Types
### How Do you Declare Variables and What Are Naming Conventions to Name Variables?
- Variables are for storing and referencing different data types
- To declare variables, you assign a value to an identifier with the assignment `(=)`operator
- You write the name of the variable on the left, followed by the assignment operator, and the value you want to assign the variable on the right

e.g Declaring `name` and `age` variables

```python
name = 'John Doe'
age = 25

```
In the above example the variable `name` holds the value `'John Doe'`.

- This value is a **String** - A series of characters used to represent text
- Strings are written with single or double quotes, for example `'Hello'` or `"Hello"`

**Important rules to consider when naming variables in Python**
- Variable names can only start with a letter or an underscore, not a number.
- Variable names can only contain alphanumeric characters (`a-z`, `A-Z`,`0-9`) and underscores(`_`).
- Variable names are case-sensitive -`age`, `Age`, and `AGE` are all considered unique.
- Variable names cannot be one of Python's reserved keywords such as `if`, `class`, or `def`.

If you break any of those rules, your Python program will throw a `SyntaxError`

**Common naming conventions for variables in Python**
1. Variable names should be in lowercase, with separate words separated by an underscore. This is called **snake case**:

```python
my_variable_name = 'freeCodeCamp'
```
2. Use descriptive names for variables. For example, if you want to save a user's age as a variable, `user_age` is better than `age` or an abbreviation like `ua`:

```python
user_age = 30
```
This way you can easily communicate the purpose of a variable to other team members (or to your future self) in a large codebase.

3. Avoid using single-letter variable names. Variable names with a single letter communicate no purpose or meaning:

```python
x = 56 # What do you mean by x?
```

**What are comments and how do they work in Python**
- Comments are used to explain your code, leave reminders for yourself, or clarify why a line exists. However they should'nt be used to explain what your variable name mean, as the variables should be descriptive and communicate what they are for
- Comments start with a pound symbol (`#`), and the language ignores everything after the `#` symbol on that line

```python
# This is a single-line comment
```
- Multi-line comments can be created by using consecutive single-line comments:
```python
# This is a 
# multi-line
# comment
```

### How Does the Print Function Work?
Every programming language has some way to output data to the terminal with a built-in method, function, property, or keyword.
- In Python, you can use the `print` function to print data to the terminal.
- Put the string `Hello world!` in between the opening and closing parentheses and call the `print` function:

```python
print('Hello world!') # Hello world!
```
- In the example above, the string `Hello world!` is an *argument* passed to the `print` function.
- You can also use the `print` function to show multiple values, or arguments, at once by separating them with commas. For example

```python
print('My favorite colors are', 'blue', 'green', 'red')

# Output: My favorite colors are blue green red
```
Python automatically adds a space between each item when you separate them with commas. This is helpful if you want to print several pieces of information together

### Understanding Variables and Data Types
Before working with variables, it's important to understand data types.
- Data types `describe the kind of value a variable holds`. For example, a `number`, a `piece of text (string)`, or a `list of items`.
- Programming languages use data types so they know how to store and work with different kinds of information.
- Python is a `dynamically-typed language` like JavaScript, you don't need to explicitly declare variable types. The interpreter determines the data type based on the value you assign.  

```python
name = 'John Doe'#Python interpreter knows this is a string
age = 25 # The interpreter knows this is an integer

```
This is in contrast to some `statically-typed languages` like #C, Java, and C++, where you have to declare types with variables

```java
string name = 'John Doe'
int age = 25
```
The dynamic-typing nature of Python makes coding really fast and more flexible, but it can lead to unexpected bugs because type errors are detected only when a program runs, not when the program compiles

- Since Python determines data types while your program is running, type-related mistakes are only discovered at that moment.
- When a program runs, Python executes your code line by line.
- If it reaches a line where a certain object is expected to behave in a way it's not able to, Python will stop and show an error.

In contrast, some languages compile your program before it runs.
- Compiling means the computer checks your code in advance and prepares it to run.
- During this step, those languages can catch type errors before the program even starts

- `In Python type errors can reveal themselves during execution, when the program is actually running and using your code`.

- `Compiled languages catch type errors during the compile step, before the program is allowed to run`.

**Common data types in Python**
- **Integer**: A whole number without decimals, for example, `10` or `-5`.
```python
my_integer_var = 10
print('Integer:', my_integer_var) # Integer: 10
```
- **Float**: A number with a decimal point, like `4.41` or `-0.4`.
```python
my_float_var = 4.50
print('Float:', my_float_var) # Float: 4.50
```
- **String**: A series of characters used to represent text / A sequence of characters enclosed in single or double quotations marks like `'Hello World!'`
```python
my_string_var = 'hello'
print('String:', my_string_var) # String: hello
```
- **Boolean**: A true or false type, writtten as `True` or `False`
```python
my_boolean_var = True
print('Boolean:', my_boolean_var) # Boolean: True
```
- **Set**: An `unordered collection of unique elements` enclosed in curly braces, like `{0.5, 4, 'apple'}`
```python
my_set_var = {6, 'code', 2.4}
print('Set:', my_set_var) # Set: {6, 'code', 2.4}
```
- **Dictonary**: A collecton of `key-value pairs` enclosed in curly braces, like `{'name': 'John Doe', 'age': 28}`
```python
my_dictionary_var = {'name': 'Alice', 'age': 25}
print('Dictionary:', my_dictionary_var) # Dictionary: {'name': 'Alice', 'age': 25}
```
- **Tuple**: An `immutable ordered collection`, enclosed in parentheses, like `(apple', 4.5, 7)`
```python
my_tuple_var = (6, 'code', 2.4)
print('Tuple:', my_tuple_var) # Tuple: (6, 'code', 2.4)
```
- **Range**: A sequence of numbers, often used n loops, for example, `range(5)`
```python
my_range_var = range(5)
print('Range:', my_range_var) # Range : range(0.5)
```
- **List**: An `ordered collection` of elements that `supports different data types`
```python
my_list = [22, 'Hello world', 3.14, True]
print(my_list) # [22, 'Hello world', 3.14, True]
```
- **None**: A special value that represents the absence of a value
```python
my_none_var = None
print('None:', my_none_var)
