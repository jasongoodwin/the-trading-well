# tradewell

Repository containing dark arts.

# Pinescript Basics

## Boilerplate
files have the version annotation at the top:

`//@version=4`

then have a call to strategy or study.

Studies have to call a function to output (`plot` etc)
Strategies have to call a `strategy.*` function 

## Study vs Strategy

Studies:
- can plot
- contain calculations
- can't be used in back-testing
- do not contain `strategy.*` calls.
- can create and use `alertcondition`

Strategies:
- same as studies
- can be used for backtesting
- need to contain calls for buy/sell orders
- You can create an `alertcondition` but can't use it.

## Spacing + Indenting

Multi-line statements are made by having the subsequent lines having any number of spaces that are not a multiple of 4.

```python
a = 1
  + 1
```

Functions require indentation of 4 spaces similar to python

```python
my_function() => 
    a = 1 + 1
    a

```

## Comments 
Pine supports single-line comments only.
Comments are denoted by `//`. They can be placed most anywhere apart from on multi-line statements.

# Identifiers
Identifiers the name referencing a function or variable. Identifiers can't be re-defined.

```python
a = 1
b = 2
c = b
```

Can contain uppercase or lowercase, numbers and underscore. Cannot start with number. 

# Variable Types
Pine has the following types:

- Integer: `a = 1`
- Float: `a = 3.2`
- Strings: `a = "hello"` or `a = 'hello'`
- Bool `a = true`
- Colors `a = #ff0000` or `a = color.red`
- Lines and Labels
- Plots and hline (horizontal line)
- `na` which is null/none


