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
In the above example the variable `name` holds the value `"John Doe"`.

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
my_variable_name = "freeCodeCamp"
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