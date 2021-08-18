---
layout: post
title: "Print and Strings"
---

# Project Goal: Generate a Title with Two Separate String Inputs

The idea is simply to take two inputs from the console and, after combining them, print out the result:

```python
> Enter the name of your hometown:
Chicago
> Enter the name of a pasta:
Mostaccioli
 > You generated the title Mostaccioli Chicago

```

### Review Printing to the Console in Python

- `print()` function

- think of functions as mini-programs

- a great deal of the code you write will consist of functions so a great deal more to come on them

- here two of Python's _built-in_ functions are  introduced, `print()` and `input()`


### String Manipulation and Code Intelligence

- `string` is a data type in Python

- the contents can be between either double or single quotes, just don't mix them.

- common error with strings - leave off a quotation mark

```python
File "main.py", line 1
    print('Hello, World)
                       ^
SyntaxError: EOL while scanning string literal
```

But how to interpret the error message?

Well, you do know:

- occurred in `File "main.py"`
- on line 1 of that file
- that it was a `SyntaxError` involving `EOL`

What is a `SyntaxError`?  What does the `^` tell you?  `EOL`?

Errors

- Get used to them
- Learn to decipher them
- Don't be afraid of them

If you cannot for the life of you figure out what the message means, copy the error and dump it into a search engine.  Typically you find yourself at _StackOverflow_.

### A closer look at the `string` data type and comments

```python

# this is a comment
# the hashtag tells the Python interpreter to ignore the whole line or ...

print('a string to print')  # ... the right it

# You will use comments a lot ... more on that later

# Note these strings

"Hello"

# vs

'Hello'

# but not

"Hello'

#  also

"Goodbye 'Cruel' World"

# vs

"Goodbye "Cruel" World"

# special characters for strings and printing
# escape
"Goodbye \"Cruel\" World"

# prints: Goodbye "Cruel" World
# or
"Goodbye 'Cruel' World" # combine single and double







```





### Exercise - Debugging Practice


### The Python `input()` Function

### Exercise - `input()` Function

### Variables

### Exercise - Variables

### Variable Naming

### Quiz 2: Variable Naming Quiz

### Project: Title Generator