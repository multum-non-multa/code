---
layout: post
title: "[8] Introduction to Functions"
---

<h2 style="color:firebrick">

    Under Construction

</h2>

## Before Anything, An Example

Let's say your program, on several occasions, must take two values from repeated user input and produce a ratio to be used in the rest of the program.

If we assume two `string` inputs, `savings_account_balance` and `debt_owed`, you need, at the very least, convert them into `floats`, calculate the ratio, and return a properly rounded value.

A function would be the very thing you'd want.  You just dump the two values in a function, have the function perform the actions mentioned in the paragraph above, and return the value desired:

```python

def calc_asset_debt_ratio(savings, debt):
    savings = float(savings)
    debt = float(debt)
    return round(savings/debt, 2)

# then every time you need to use it, you `call` it:
savings_account_balance = input("Enter savings balance ")
debt_owed = input("Enter overall debt ")

ratio = calc_asset_debt_ratio(savings_account_balance, debt_owed)
# do something with ratio ...
# ...

```

## Anatomy of a Function





## Do You Need Them?

Yes.  All the time.


##  Think of Them As Mini-Programs

in => data ---- arguments
process
out => data ---- return value


