---
layout: post
title: print() and Strings
---

- [Project: Generate a Title with Two Separate String Inputs](#project--generate-a-title-with-two-separate-string-inputs)
  * [1. Review Printing to the Console in Python](#1-review-printing-to-the-console-in-python)
  * [2. String Manipulation](#2-string-manipulation)
    + [`string` data type and comments](#-string--data-type-and-comments)
    + [`string` concatenation](#-string--concatenation)
  * [3. Spacing Python Code](#3-spacing-python-code)
  * [4. Code Intelligence](#4-code-intelligence)
  * [5. Practice Debugging Errors](#5-practice-debugging-errors)
  * [6. The Python input Function](#6-the-python-input-function)
    + [a. Data in general](#a-data-in-general)
    + [b. A Program Model](#b-a-program-model)
    + [c. input](#c-input)
  * [7. Practice Using input](#7-practice-using-input)
  * [8. Variables](#8-variables)
  * [9. Practice with Variables](#9-practice-with-variables)
  * [10. Variable Naming](#10-variable-naming)
  * [11. Variable Naming Quiz](#11-variable-naming-quiz)
  * [12. Title Generator](#12-title-generator)


## Project: Generate a Title with Two Separate String Inputs

Result:  Take two inputs from the console and, after combining them, print out the result:

```python
> Enter the name of your hometown:
Chicago
> Enter the name of a pasta:
Mostaccioli
> You generated the title Mostaccioli Chicago
```

### 1. Review Printing to the Console in Python

- `print()` function

- think of functions as mini-programs

- a great deal of the code you write will consist of functions so a great deal more to come on them

- here two of Python's _built-in_ functions are  introduced, `print()` and `input()`


### 2. String Manipulation

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

#### `string` data type and comments

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

# also new line and tab characters

"Hello\nHello"

# if printed will print out
# Hello
# Hello
# The escape n or \n instructs the interpreted to insert a line break

"Hello\tHello"

# will print
# Hello     Hello
# inserting a tab space between the two words

```

#### `string` concatenation

What is 'concatenation' of `strings`?

Well, data types typically come with a set of 'operators' that can be used on them, e.g.,

```python
# math on two number data types
1 + 2
1 - 2
```

Those `+` and `-` signs are called 'operators,' i.e., they operate on the numbers which, to carry the terminology to technical use, are 'operands,' i.e., expressions on which the 'operators' 'operate.'

`strings` have operators as well.  But first, more on terminology.

Why do they even call text `strings`?

Under the hood, `strings` are essentially another type called, in some programming languages, `chars` or characters.  More than one `char` between quotes is a `string` of such data type.

Python, however, makes no distinction between the two but treats one or more characters together as a `string`, i.e., a `string` is nothing but one or more `chars` chained together such as `H` + `e` + . . .

Knowing this the term 'concatenation' makes a bit more sense:

> concatenare, from con- ‘together’ + catenare, from catena ‘chain’

A `string` is a chaining together of characters or `chars` in some languages.  Perhaps not relevant to you now, but a `string` in Python is actually an `array` of characters stored in memory together.

As it turns out the `+` operator works on `strings` as well as numbers.  E.g.,

```python
print('Hello' + 'World')
# prints HelloWorld

print('Hello ' + 'World')
# prints Hello World
#             ^
# note the space - because the string 'Hello ' inserted a space at end
```

If you concatenate `strings`, you will often need to insert spacing, e.g.,

```python
print('Hello ' + 'World')
# or
print('Hello' + ' World')
# or
print('Hello' + ' ' + 'World')
```

### 3. Spacing Python Code

```python
# put a space or two or three before the print
1   print('some string to print')
# remove the spaces
2 print('some string to print')
```

```bash
File "main.py", line 1
    print('some string to print')
    ^
IndentationError: unexpected indent
```

Neither line 1 nor line 2 will run.  Why?

Line 1:  Python, unlike many other languages, determines how to interpret code based on, among other things, the _indentation_ of a line of code.

Line 2: Because it is a type of 'compilation' or interpreter error, the interpreter will not even get to line 2.

If you correct line 1, both lines will print.



### 4. Code Intelligence

A word on syntax helpers ...

### 5. Practice Debugging Errors

Go to the team projects and work on the error and debugging exercises.

### 6. The Python `input` Function

#### a. Data in general

#### b. A Program Model

#### c. `input()`


### 7. Practice Using `input`

### 8. Variables

### 9. Practice with Variables

### 10. Variable Naming

### 11. Variable Naming Quiz

### 12. Title Generator






<small><i><a href='http://ecotrust-canada.github.io/markdown-toc/'>Table of contents generated with markdown-toc</a></i></small>