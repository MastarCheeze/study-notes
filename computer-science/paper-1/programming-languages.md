# Programming Language

## Low-level

> Closer to machine language

-   Machine code
-   Assembly
    -   Uses mnemonics
    -   Assembler to translate into machine code

## High-level

> English-like statements

-   Python
-   Java
-   VB.NET

<br>

| Low-level                                                    | High-level                           |
| ------------------------------------------------------------ | ------------------------------------ |
| ✅ Does not need translating <br> (assembly translates fast) | ❌ Needs translating                 |
| ✅ Can directly manipulate memory                            | ❌ Cannot directly manipulate memory |
| ❌ Hard to read/write                                        | ✅ Easy to read/write                |
| ❌ Hard to debug                                             | ✅ Easy to debug                     |
| ❌ Machine dependent (not portable)                          | ✅ Machine independent (portable)    |
| ❌ More code needed                                          | ✅ Less code needed                  |

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

**Writing program**

| Compiler                          | Interpreter                                 |
| --------------------------------- | ------------------------------------------- |
| ❌ Code has to be complete to run | ✅ Code does not have to be complete to run |
| ❌ Harder to debug                | ✅ Easier to debug                          |
| ❌ Reports error all at once      | ✅ Reports error one at a time              |

**Distributing program**

| Compiler                                                  | Interpreter                                       |
| --------------------------------------------------------- | ------------------------------------------------- |
| ✅ Produces executable file                               | ❌ Does not produce executable file               |
| ✅ Does not need translator to run                        | ❌ Needs interpreter to run                       |
| ✅ Does not need source code to run                       | ❌ Needs source code to run                       |
| ✅ Does not need to re-translate code each time it is run | ❌ Needs to re-translate code each time it is run |

<br>

# IDE[^IDE]

> Software \
> Provides useful tools for writing a program

-   Code editors
-   Run-time environment
-   Translators
-   Error diagnostics
-   Auto-completion
-   Auto-correction
-   Prettyprint

<br>

[^IDE]: Integrated Development Environment
