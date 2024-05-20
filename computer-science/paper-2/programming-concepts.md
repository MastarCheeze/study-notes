# Variables & Constants

| Variable                  | Constant                     |
| ------------------------- | ---------------------------- |
| Stores data               | Stores data                  |
| Accessed with identifier  | Accessed with identifier     |
| Can change during runtime | Cannot change during runtime |

# Selection

## IF

-   Result is either true or false

## CASE

-   Has a list of values to compare a single value against

# Iteration

## Count-controlled

> `FOR`

-   Set number of iterations

## Pre-condition

> `WHILE`

-   Checks condition at start of loop
-   May not iterate at all

## Post-condition

> `REPEAT-UNTIL`, `DO-WHILE`

-   Checks condition at end of loop
-   Iterates at least once

# Procedures & Functions

> **Parameter** - value passed into a procedure/function

| Procedure                        | Function                         |
| -------------------------------- | -------------------------------- |
| Define once, call multiple times | Define once, call multiple times |
| Called using identifier          | Called using identifier          |
| Can be passed parameters         | Can be passed parameters         |
| Does not return a value          | Returns a value                  |

## Benefits

-   Modularisation, code can be reused
-   Faster development
-   Shorter code, more maintainable

## Scope

| Global                            | Local                                               |
| --------------------------------- | --------------------------------------------------- |
| Declared outside of any functions | Declared inside a function                          |
| Accessed anywhere                 | Accessed only within the function it is declared in |

# Library routines <small><sup><sub>(built-in functions)</sub></sup></small>

|            |                                                                |
| ---------- | -------------------------------------------------------------- |
| **DIV**    | Does integer division and returns only the whole number        |
| **MOD**    | Does integer division and returns only the remainder           |
| **ROUND**  | Rounds a number <br> To the number of decimal points specified |
| **RANDOM** | Picks a pseudorandom number <br> Between the numbers specified |
