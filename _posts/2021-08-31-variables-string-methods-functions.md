---
layout: post
title: "Variables, Data Types, and More on Strings"
---


---

## Overview

1. Variables

    Variable Declarations

    Variable Assignment

    Variable Use

    Variable Types in Python

    Variable Names & Key Words in Python

2. More Regarding Strings

    a. Strings are 'data structures'

    b. Common Methods and Operations on Strings

      i. Slicing

      ii.  Manipulations

---

### Note

> A very good idea:  when you see some code snippets below, dump it in a repl and play around with it.  It builds a certain type of coding memory.

---

## Variables

### Variable Declarations

Order is important in a program.  A program reads from top of the page to the bottom.  The Python interpreter cannot anticipate what falls below the line it is reading.  Thus, only __after__ you declare a variable can you use it.  For example:

```python
# this works
num = 9
print(num)

# this throws a NameError
print(number)
number = 12
```

### Variable Assignment

The `=` sign between a variable name on the left and a value on the right is an `operator`.  It acts to __bind__ or ___assign___ the variable name to the value.  Thus:

```python
college = "Whatsamatta U"
```

### Variable Use

But one of the reasons you create a variable is ease of use. Not only do you keep track of a value (even if the value itself changes state, e.g., a number increases from 1 to 2), you can use the variable name anywhere you might use the literal.  In other words, take:

```python
food = input("Enter the restaurant's major food item")
```

If that message (`"Enter the restaurant's ..."`) will be used more than once, use a variable name instead:

```python
# declare a variable
get_rest_food = "Enter the restaurant's major food item"
# do other stuff here . . .
# sometime later
food = input(get_rest_food)
```
### Variable Types in Python

As mentioned in a prior post, Python's primitive or basic data types are:

- `strings`
- `integers`
- `floats`
- `booleans`
- `None`

Leaving `None` aside for now, plug the others into a repl and see:

```python
park_name = "Grant Park"
print(type(park_name))

age_of_park = 120
print(type(age_of_park))

acreage_of_park = 34.54
print(type(acreage_of_park))

is_urban_park = True
print(type(is_urban_park))

```

If you run that you'll get:

```bash
<class 'str'>
<class 'int'>
<class 'float'>
<class 'bool'>
```

For now ignore the `<class` and `>` parts.

More importantly for now: you'll the type of each variable entered.  To what they refer is obvious: `str` => string, `int` => integer, etc.

That your data has a type is important.

Simply put: with different data types you do different things, you store different values and you perform different operations.  You'll find some built-in functions won't accept certain types of data.  As as example of, look at this repl:

```python
>>> length_of_name = len("Fred")
>>> length_of_name
4
# value of 4 returned
# if Fred's age is now entered:
>>> fred_age = 89
>>> len(fred_age)
Traceback (most recent call last):
  File "<input>", line 1, in <module>
    len(fred_age)
TypeError: object of type 'int' has no len()
>>>
```

That error is trying to tell you that the built-in `len()` function does not take an `integer`.  Simply put, numbers don't have length.  The data type matters.

Another example:  if you are taking a user's age an input (that may be at the console, but more typically it is through a web browser or retrieving it from a database), that age is often a `string`.  Thus:

```python
age_of_statue_in_park = "12"
```

__Conversion__

But you want to perform some math operation on that age value, e.g., you want to use it to calculate how many years after Grant Park had been established that the statue was erected.  Well, you can't just use the data from above --- `age_of_park` and substract `"12"` from it.

Why?

That `"12"` is a `string` but `age_of_park` is an `integer`.  So what to do?

Convert the `string` into an `integer` using another one of Python's built-in functions.

Here we use the built-in `int()`:

```python
age_of_statue_in_park = int(age_of_statue_in_park) # convert string to an integer
# now you can use it to subtract from age of park
age_built = age_of_park - age_of_statue_in_park
```

`int()` ___takes in___ a `string` that wraps an `integer`, e.g., `int(age_of_statue_in_park)` or `"12"`, and `returns` the `integer`.

### Variable Names & Key Words in Python

One last thing about variable names (at least, for now):  certain words may not be used. These are Pythons keywords or reserved words.  For example, `print` is the name of a built-in function in Python.  You should ___not___ use that for a variable name.  Below you see Python run directly from the command line.  `print` is assigned a value of `4`.  Once that's done, it can now no longer be used as a function --- at least not as long as the program is running.

```python
>>> print = 4
>>> print
4
>>> print('some string here')
Traceback (most recent call last):
  File "<input>", line 1, in <module>
    print('some string here')
TypeError: 'int' object is not callable
>>>

```

### Keywords to Avoid Using for Your Variables' Names

Do ___not___ use the following when naming a value:

```
and
as
assert
async
await
break
class
continue
def
del
elif
else
except
False
finally
for
from
global
if
import
in
is
lambda
None
nonlocal
not
or
pass
raise
return
True
try
while
with
yield
```

Got that?  No worries; you'll be using these keywords soon enough for their proper purposes.

---

## More Regarding Strings

### Strings are 'data structures'

When you create a `string`, the computer stores it as just that, a ___string___ of characters.  Thus:

```python
movie_title = "Rocky"
```

In memory, that is stored in a contiguous series of characters:

`[R][o][c][k][y]`

which are indexed:

![Superscripting](/code/assets/images/variables-08-31/rocky-index.jpg)

What does that mean?  First, a `string` is a `data structure` --- it holds data.

Second, you can retrieve these characters by index value using the `[ ]` (square bracket) operator:

```python

third_letter = movie_title[2]
print(third_letter)
# c
```







### Common Methods and Operations on Strings

#### Slicing

#### Manipulations


