# fundamentals-of-python-programming

### Comment in Python
A comment provide a quick instruction on what does the line of code do <br>
A docstring provide a summary of what does the function do.
```
# This is a python comment
'''This is a docstring / multiline string / comment'''
```

### Variables and Data Types

```
x = 1                 # ---> integer: numbers (without decimal) - int() -- convert to an integer value
y = 2.5               # ---> float: numbers (with decimal) - float() -- convert to a float value
name = 'John'         # ---> string: any characters - str() -- convert to string value
is_cool = True        # ---> boolean: is either True or False - bool() -- convert to boolean value

# Types of Data Structures:
some_list = [1,2,3]     # ---> list(): a collection which is order and changeable
some_tuples = (1,2,3)   # ---> tuple(): a collection which is ordered but unchangeable
some_set = {1,2,3}      # ---> set(): a collection which is undordered, unindexed, no duplicate members (but changeable)
some_dictionary = {
    'first_name' : 'John',
    'last_name' : 'Doe',
    'age' : 20
}                       # ---> dic() (key-value pair): a collection which is undordered, indexed, no duplicate members (but changeable)

# Assignment Magic
x, y, z = 1, 2, 3
print(x, y, z)

```

### What is a Data Structures
A data structure is a collection of data elements (such as numbers or characters, or even other data structures) that is structured in some way, such as by numbering the elements. 
- List
- Tuples
- Set
- Dictionary

### Common Operators
Common operators include indexing, slicing, adding, multiplying, and checking for membership. 
```
greeting = 'Hello'
greeting[0] <-- Indexing

tag = '<a href="http://www.python.org">Python web site</a>'
tag[9:30] <-- Slicing

```

### Strings
```
print(name + x + y) <-- Concatenate strings
print(name, x, y) <-- Concatenate strings
print(name.capitalize()) <-- Using capitalize() method
"{name} is approximately {value}.".format(value=pi, name="π") <-- Formatted Strings (1): Argument by Position
f"Euler's constant is roughly {e}." <-- Formatted Strings (2): Using F-Strings
```

### Functions
Function is a block of code which only runs when it's called in python.
Lambda Function - a small anonymous function, can take any number of arguments, but can only have one expression.
```
# regular composition of a function in python
def sayhello(name):
  print('Hi!')
  given_name = name <-- given_name is a variable where the scope is within the function only.
  return given_name

# lambda function
getsum = lambda num1, num2: num1 + num2
print(getsum(10,3))
```

### Conditional 
```
if x > y: # if condition
  print(x)
elif x != y: # elif condition
  print(z)
else: # else condition
  print(y)
```
### Comparisson Operators
```
== (equal to), != (not equal to), > (greater than), < (less than), >= (greater/equal), <= (less/equal)
```
### Logical Operators
```
and, or, not
```
### Membership Operators
```
# This test to see if something is in or not in a the data structure
is, is not, in, not in

if 'apple' not in fruits:
  print('not existing')
```
### Loops
Python only have for and while loops.
Use break (stop), pass (skip entire block, then, go to next iteration), continue (skip but keep going to next block code)
- Break: To end (break out of) a loop, you use break. Let’s say you wanted to find the largest square (the result of an integer multiplied by itself) below 100. Then you start at 100 and iterate downward to 0. When you’ve found a square, there’s no need to continue, so you simply break out of the loop.

- Continue: The continue statement is used less often than break. It causes the current iteration to end and to “jump” to the beginning of the next. It basically means “skip the rest of the loop body, but don’t end the loop.” This can be useful if you have a large and complicated loop body and several possible reasons for skipping it. 

```
# FOR LOOPS:

for person in people:
  print(person)
  
for i in range(len(people)):
  print(people(i))

for i in range(0,11):
  print(i)

# WHILE LOOPS:

count = 0
while count <= 10:
  print(count)
  count =+1 # Augmented Assignments: same as count = count + 1
  
name = ''
while not name:
 name = input('Please enter your name: ')
print('Hello, {}!'.format(name))

```

#### Importing
```
# when you import something from a module, you either use:

import module
from module import function
from module import function1, function2, function3
from module import *

# You can add an as clause to the end and supply the name you want to use, either for the entire module:

import math as m
m.sqrt(4)

For the open functions from different modules, you might use the following:
from module1 import open as open1
from module2 import open as open2
```



<hr></hr>

### Terminologies

- Algorithms: An algorithm is a recipe telling you exactly how to perform a task. When you program a computer, you are essentially describing an algorithm in a language the computer can understand, such as Python. Such a machinefriendly description is called a program, and it mainly consists of expressions and statements.

- Expressions: An expression is a part of a computer program that represents a value. For example, 2 + 2 is an expression, representing the value 4. Simple expressions are built from literal values (such as 2 or "Hello") by using operators (such as + or %) and functions (such as pow). More complicated expressions can be created by combining simpler expressions (e.g., (2 + 2) * (3 - 1)). Expressions may also contain variables.

- Variables: A variable is a name that represents a value. New values may be assigned to variables through assignments such as x = 2. An assignment is a kind of statement.

- Statements: A statement is an instruction that tells the computer to do something. That may involve changing variables (through assignments), printing things to the screen (such as print("Hello, world!")), importing modules, or doing a host of other stuff.

- Functions: Functions in Python work just like functions in mathematics: they may take some arguments, and they return a result. (They may actually do lots of interesting stuff before returning.

- Modules: Modules are extensions that can be imported into Python to extend its capabilities. For example, several useful mathematical functions are available in the math module.

- Strings: Strings are really simple—they are just pieces of text, with characters represented as Unicode code points. And yet there is a lot to know about them. In this chapter, you’ve seen many ways to write them, and in Chapter 3 you learn many ways of using them.

- Sequences: A sequence is a data structure in which the elements are numbered (starting with zero). Examples of sequence types are lists, strings, and tuples. Of these, lists are mutable (you can change them), whereas tuples and strings are immutable (once they’re created, they’re fixed). Parts of a sequence can be accessed through slicing, supplying two indices that indicate the starting and ending positions of the slice. To change a list, you assign new values to its positions or use assignment to overwrite entire slices.

- Membership: Whether a value can be found in a sequence (or other container) is checked with the operator in. Using in with strings is a special case—it will let you look for substrings.

- Methods: Some of the built-in types (such as lists and strings but not tuples) have many useful methods attached to them. These are a bit like functions, except that they are tied closely to a specific value. 

- Mappings: A mapping enables you to label its elements with any immutable object, the most usual types being strings and tuples. The only built-in mapping type in Python is the dictionary.

- String formatting with dictionaries: You can apply the string formatting operation to dictionaries by using format_map, rather than using named arguments with format.

- Dictionary methods: Dictionaries have quite a few methods, which are called in the same way as list and string methods.
