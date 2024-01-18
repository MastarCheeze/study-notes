# Pseudocode

## Data types

|                        |                      |
| ---------------------- | -------------------- |
| `INTEGER`              | `5`, `-3`            |
| `REAL`                 | `4.7`, `-8.0`, `0.0` |
| `CHAR`                 | `'x'`, `'@'`         |
| `STRING`               | `"foo"`, `"bar"`     |
| `BOOLEAN`              | `TRUE`, `FALSE`      |
| `ARRAY OF <data type>` |                      |

## Arithmetic

|               |                             |
| ------------- | --------------------------- |
| `+`           | addition                    |
| `-`           | subtraction                 |
| `*`           | multiplication              |
| `/`           | division                    |
| `^`           | power                       |
| `DIV(a, b)`   | floor division              |
| `MOD(a, b)`   | modulus                     |
| `ROUND(a, b)` | round to `b` decimal places |

## Comparison

|      |                          |
| ---- | ------------------------ |
| `=`  | equal to                 |
| `<`  | less than                |
| `<=` | less than or equal to    |
| `>`  | greater than             |
| `>=` | greater than or equal to |
| `<>` | not equal to             |

# Boolean

`NOT` &ensp; `AND` &ensp; `OR`

## Naming convention

- PascalCase
- Only contain `a-z`, `A-Z`, `0-9`
- Start with letter
- No special characters (including `_`)
- Case sensitive

## Declarations & assignments

```
// Variables
DECLARE Variable : INTEGER
Variable <- 42

// Constants
CONSTANT Pi <- 3.142
```

## Arrays

```
// 1D array (1-indexed)
DECLARE Array : ARRAY[1:10] OF STRING
Array[1] <- "spam"

// 2D array
DECLARE Array2D : ARRAY[1:10, 1:10] OF INTEGER
Array2D[4, 2] <- 18
```

## IO

```
// Output
OUTPUT "Hello World"
OUTPUT Name
OUTPUT "Score: ", Score

// Input
INPUT Answer
```

## String operations

```
LENGTH("Spam Ham and Eggs")  // 17

LCASE("Spam Ham and Eggs")  // "spam ham and eggs"
UCASE("Spam Ham and Eggs")  // "SPAM HAM AND EGGS"

// (1-indexed)
SUBSTRING("Spam Ham and Eggs", 1, 4)  // "Spam"
```

## Random

```
RANDOM()  // random real between 0-1 (inclusive)
```

## Control

### If

```
IF <condition> THEN
    <statements>
ENDIF

IF <condition> THEN
    <statements>
ELSE
    <statements>
ENDIF
```

### Case

```
CASE OF variable
    value1 : <statement>
    value2 : <statement>
    ...
    OTHERWISE <statement>
ENDCASE
```

### For
```
FOR i <- start TO end
    <statements>
NEXT i

FOR i <- start TO end STEP increment
    <statements>
NEXT i
```

### While
```
WHILE <condition> DO
    <statements>
ENDWHILE
```

### Repeat until
```
REPEAT
    <statements>
UNTIL <condition>
```

## Procedures

```
PROCEDURE Procedure
    <statements>
ENDPROCEDURE

PROCEDURE Procedure(param1:<dtype2>, param2:<dtype2>, ...)
    <statements>
ENDPROCEDURE

// Calling
CALL Procedure
CALL Procedure(arg1, arg2, ...)
```

## Functions

```
FUNCTION Function RETURNS <dtype>
    <statements>
    RETURN <value>
ENDFUNCTION

FUNCTION Function(param1:<dtype2>, param2:<dtype2>, ...) RETURNS <dtype>
    <statements>
    RETURN <value>
ENDFUNCTION

// Calling
Function()
Function(arg1, arg2, ...)
```

## File IO

```
OPENFILE "file.txt" FOR READ
OPENFILE "file.txt" FOR WRITE
READFILE "file.txt", ReadText
WRITEFILE "file.txt", WriteText
CLOSEFILE "file.txt"
```
