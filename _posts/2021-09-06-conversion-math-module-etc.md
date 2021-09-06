---
layout: post
title: "[7] Data Type Conversions, More Built-in Functions, Math +, and Another Project"
---

- Project: Diners' Calculator

- Data Types Revisited

- Type Conversion

- `f-strings` Redux

- Math Methods & Functions

  - Built-ins

  - Intro to Custom (i.e., __Your Own__) Functions

  - Math Module & Imports

---

## Diner's Calculator Project

---

<div style="position: relative; padding-bottom: 56.25%; height: 0;"><iframe src="https://www.loom.com/embed/3054c971777345a0a0181e3fd1ce6a51" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"></iframe></div>

---

## Data Types Revisited

Let's go a bit further with some of the things mentioned in an earlier post - _see_ [Variable Types in Python](http://localhost:4000/code/2021/08/31/variables-string-methods-functions.html).

As mentioned, we may or may not be able to use a Python built-in function with the data.  For example, you can't use

- the `len()` function on a number, but only a sequence like a `string`

- the `[ ]` subscripting operators on a number, but, once again, only a sequence like a `string`

Sometimes, however you are able to convert from one type to another.

---

## Type Conversion

Converting from one type to another is often used when the input data is a `string` but needs to be processed as an `integer` or `float`.

E.g.,

```python
age = input("Enter your age in years")

# convert to an integer
int_age = int(age)
# or you could just do
age = int(age) # changing the existing variable

weight = input("Enter your weight in kilos ")

# convert to a float
float_weight = float(weight)
```

But it occurs elsewhere.  For example, you may want convert a `float` to an `integer`:

```python
>>> ratio_value = 38 / 6
>>> ratio_value
6.333333333333333
>>> ratio_value_estimate = int(ratio_value)
>>> ratio_value_estimate
6
>>>
```

---

## `f-strings` Redux

Refer back to [the first mention of f-strings](https://multum-non-multa.github.io/code/2021/08/18/printing-strings.html).

Also, you'll remember that sometimes you wanted to convert an `integer` to a `string` in order to accomplish concatenation:

```python
print("The estimated ratio value is " + str(ratio_value_estimate))
```



---




## How Functions Work

--> input --> [... process ...] -> output

e.g. shake maker

recipe in => ... => shake out

many times a function depends on a certain type of input

e.g., len() takes a sequence type, e.g., string, but NOT a number

and functions often return a certain type

input() returns a string

how to determine --- the type() function
returns the type

print(type(input("What is your name?" )))
print(type(len(input("What is your name?" ))))

type conversion (aka 'casting') required if
type == string but need integer or float

int()
float()

if len() => integer
str(len())
then can concatenate


exercise / challenge

given a random 2-digit number
from input()
print the sum of the two digits as a type of float
e.g.
```bash
Type a two-digit number: 43
7.0
```
involves
type checking
string subscripting
conversion
arithmetic operations

---

More math

+ = * /

** exponent

%

--
<!-- order of operations
essentially same as algebra
'PEMDAS'
from L => R
left to right
===
() parentheses <==
===
** exponents
===
* multiplication & / division
===
+ addition & - substraction -->

homework
using ** and +
produce the value 9
1 1 1 3

--

now introduce math module

> compare ** with math.pow()

** returns integer
pow returns float

>>> import math
>>> math.pow(4,5)
1024.0
>>> 4**5
1024
>>>


> other modules in math

...

> also see random module

---

cover operations for bmi calc (without mentioning bmi challenge)

bmi calculator
height = input("Enter the height in inches ")
weight = input("Enter the weight in pounts ")

bmi = weight / height**2


note:

>>> int(34.967)
34
>>> math.ceil(34.967)
35
>>> math.floor(34.967)
34
>>>


math rounding
e.g.
print(8 / 3)
2.66666666666666
int()
not great
rather use built-in round()

round((8/3))
options in round()
round((8/3), 3)

or use floor division

8 // 3
same as math.floor(8/3)




Beware the inexactitude of floating point numbers.
Note what happens here:
>>> 100 * 1.12
112.00000000000001
>>>
https://docs.python.org/3/tutorial/floatingpoint.html

So it's a good idea to choose a rounding so as not to factor in that inexactitude.
Not an issue now, but we'll return to it when we do comparison operators and conditional statements.


---
shorthand arithmetic operations

increment

score = 0
could do
score = score + 1
or use shorthand
score += 1

halving
>>> volume = 85.0
>>> volume /= 2
>>> volume
42.5
>>> volume /= 2
>>> volume
21.25
>>>

exponential growth
>>> gain = 2
>>> gain **= 2
>>> gain
4
>>> gain **= 2
>>> gain
16


revisit f-strings



can do a lot but not sure can use shorthand:

>>> h = 12.33
>>> m = False
>>> msg = f"When you reach {h} then go to {h + 100} and return {m}"
>>> msg
'When you reach 12.33 then go to 112.33 and return False'
>>> msg = f"When you reach {h} then go to {h += 233} and return {m}"
  File "<input>", line 1
    (h +)
        ^

alternative: lambda functions
 msg = f"When you reach {h} then go to {(lambda x: x + 1)(h)} and return {m}"
>>> msg
'When you reach 12.33 then go to 13.33 and return False'
>>>


challenge / homework
Your Life in Weeks
Instructions

Create a program using maths and f-Strings that tells us how many days, weeks, months we have left if we live until 90 years old.

It will take your current age as the input and output a message with our time left in this format:

You have x days, y weeks, and z months left.

Where x, y and z are replaced with the actual calculated numbers.

Warning your output should match the Example Output format exactly, even the positions of the commas and full stops.

Example Input
56
Example Output
You have 12410 days, 1768 weeks, and 408 months left.
e.g. When you hit run, this is what should happen:

https://cdn.fs.teachablecdn.com/RjqBViZQpyVTv7XY6cfA

Hint
There are 365 days in a year, 52 weeks in a year and 12 months in a year.
Try copying the example output into your code and replace the relevant parts so that the sentence is formated the same way.
Test Your Code
Before checking the solution, try copy-pasting your code into this repl:

https://repl.it/@appbrewery/day-2-3-test-your-code

This repl includes my testing code that will check if your code meets this assignment's objectives.

Solution
https://repl.it/@appbrewery/day-2-3-solution















