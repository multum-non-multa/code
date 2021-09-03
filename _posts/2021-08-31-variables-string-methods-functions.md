---
layout: post
title: "More On Variables and Strings"
---


---

## Overview

1. Variables

    [Variables ...](https://realpython.com/python-variables/)

    Variable Declarations

    Variable Assignment

    Variable Use

    Variable Types in Python

    Object References

    Object Identity

    Variable Names & Key Words in Python

2. Data Types

    [data](https://realpython.com/python-data-types/)

3. More Regarding Strings

    [string methods](https://realpython.com/python-strings/)

    a. Strings are 'data structures'

    b. Common Methods and Operations on Strings

        i. Slicing

        ii.  Manipulations

---

## Variables

[Variables ...](https://realpython.com/python-variables/)

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

But one of the reasons you create a variable is ease of use. Not only do you keep track of a value (even if the value itself changes state, e.g., a number increases from 1 to 2), you can use the variable name anywhere you might you the literal.  In order words, take:

```python
food = input("Enter the restaurant's major food item")
```

If that message (`"Enter the restaurant's ..."`) will be used more than once, stick that in a variable name:

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

For now ignore the `<class` and `>` parts.  More importantly for now: you'll the type of each variable entered.  To what they refer is obvious: `str` => string, `int` => integer, etc.



### Object References

### Object Identity

### Variable Names & Key Words in Python

## Data Types

[data](https://realpython.com/python-data-types/)

## More Regarding Strings

[string methods](https://realpython.com/python-strings/)

### Strings are 'data structures'

### Common Methods and Operations on Strings

#### Slicing

#### Manipulations






