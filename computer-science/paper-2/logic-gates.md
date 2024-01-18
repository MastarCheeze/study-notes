# Logic Gates

- [NOT](#not)
- [AND](#and)
- [OR](#or)
- [NAND](#nand)
- [NOR](#nor)
- [XOR](#xor)

<br>

> <p></p>
> Purpose of logic gates
>
> - Perform logic operations
> - Control flow of electricity
> - Input → apply logic → output

## NOT
![NOT gate](../images/logic-gate-not.png)

> $$
\begin{align*}
  \text{X} &= \text{NOT A} \\
  \mathrm{X} &= \mathrm{\overline{A}}
\end{align*}
> $$

| A   | X     |
| --- | ----- |
| 0   | **1** |
| 1   | **0** |

## AND
![AND gate](../images/logic-gate-and.png)

> $$
\begin{align*}
  \text{X} &= \text{A AND B} \\
  \mathrm{X} &= \mathrm{A.B}
\end{align*}
> $$

| A   | B   | X     |
| --- | --- | ----- |
| 0   | 0   | **0** |
| 1   | 0   | **0** |
| 0   | 1   | **0** |
| 1   | 1   | **1** |

## OR
![OR gate](../images/logic-gate-or.png)

> $$
\begin{align*}
  \text{X} &= \text{A OR B} \\
  \mathrm{X} &= \mathrm{A+B}
\end{align*}
> $$

| A   | B   | X     |
| --- | --- | ----- |
| 0   | 0   | **0** |
| 1   | 0   | **1** |
| 0   | 1   | **1** |
| 1   | 1   | **1** |

## NAND
![NAND gate](../images/logic-gate-nand.png)

> $$
\begin{align*}
  \text{X} &= \text{A AND B} \\
  \mathrm{X} &= \mathrm{\overline{A.B}}
\end{align*}
> $$

| A   | B   | X     |
| --- | --- | ----- |
| 0   | 0   | **1** |
| 1   | 0   | **1** |
| 0   | 1   | **1** |
| 1   | 1   | **0** |

## NOR
![NOR gate](../images/logic-gate-nor.png)

> $$
\begin{align*}
  \text{X} &= \text{A OR B} \\
  \mathrm{X} &= \mathrm{\overline{A+B}}
\end{align*}
> $$

| A   | B   | X     |
| --- | --- | ----- |
| 0   | 0   | **1** |
| 1   | 0   | **0** |
| 0   | 1   | **0** |
| 1   | 1   | **0** |

## XOR
![XOR gate](../images/logic-gate-xor.png)

> $$
\begin{align*}
  \text{X} &= \text{A XOR B} \\
  \mathrm{X} &= \mathrm{A\oplus B}
\end{align*}
> $$

| A   | B   | X     |
| --- | --- | ----- |
| 0   | 0   | **0** |
| 1   | 0   | **1** |
| 0   | 1   | **1** |
| 1   | 1   | **0** |
