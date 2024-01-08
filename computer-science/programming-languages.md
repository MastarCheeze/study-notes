# Programming Language

## Low-level

> Closer to machine language

- Machine code
- Assembly
    - Uses mnemonics
    - Assembler to translate into machine code

## High-level

> English-like statements

- Python
- Java
- VB.NET

<br>

|                         | Advantages                                                                                                                        | Disadvantages                                                                                                                       |
| ----------------------- | --------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- |
| <nobr>Low-level</nobr>  | <ul><li>Does not need translating <br> (Assembly translates fast)</li><li>Can directly manipulate memory</li></ul>                | <ul><li>Hard to read/write</li><li>Hard to debug</li><li>Not portable, machine dependent</li><li>More instructions needed</li></ul> |
| <nobr>High-level</nobr> | <ul><li>Easy to read/write</li><li>Easy to debug</li><li>Portable, machine independent</li><li>Less instructions needed</li></ul> | <ul><li>Needs translating</li><li>Cannot directly manipulate memory</li></ul>                                                       |

<br>

# Translators

> High-level → machine code

## Compiler

> Translates whole code at once before executing \
> Produces executable file

## Interpreter

> Translates/executes code line by line

## Assembler

> Assembly → machine code

<br>

| Compiler                                              | Interpreter                                   |
| ----------------------------------------------------- | --------------------------------------------- |
| Useful for **distributing** finished program          | Useful when **writing** program               |
| Produces executable file                              | Does not produce executable file              |
| No other software required to run                     | Interpreter software required to run          |
| Source code not required to run                       | Source code required to run                   |
| Code does not need re-translating each time it is run | Code needs re-translating each time it is run |
| Creates **error report** with **all** errors          | Stops when error is found                     |

<br>

# IDE[^IDE]

> Software \
> Provides useful tools for writing a program

- Code editors
- Run-time environment
- Translators
- Error diagnostics
- Auto-completion
- Auto-correction
- Prettyprint

<br>

[^IDE]: Integrated Development Environment
