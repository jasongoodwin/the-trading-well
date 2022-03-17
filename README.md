# tradewell
dark arts go here

# Pinescript Quickstart

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

## Format
Multi-line statements are made by having the subsequent lines having any number of spaces that are not a multiple of 4.

```python
a = 1
  + 1
```

