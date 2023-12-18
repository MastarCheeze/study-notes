# Integration

## Finding integrals

### Rules

- Constant rule
  $$\integral{a} = ax + c$$
- Constant multiple rule
  $$\integral{ax} = a\integral{x}$$
- Sum & difference rule
  $$\integral{f(x)+g(x)} = \integral{f(x)}+\integral{g(x)}$$
- Power rule
  $$
  \begin{aligned}
    \int x^n &= \frac{x^{n+1}}{n+1}+c \\
    \int (ax+b)^n &= \frac{(ax+b)^{n+1}}{a(n+1)}+c \\
  \end{aligned}
  $$

### Properties

- Exponential functions
  $$
  \begin{aligned}
    \integral{e^x} &= e^x + c \\
    \integral{e^{ax}} &= \frac{e^{ax}}{a} + c
  \end{aligned}
  $$
- Logarithmic functions
  $$
  \begin{aligned}
    \integral{\frac{1}{x}} &= \ln(x) + c \\
    \frac{1}{ax} &= \frac{\ln(ax)}{a} + c
  \end{aligned}
  $$
- Trigonometric functions
  $$
  \begin{aligned}
    \integral{\sin x} &= -\cos x + c \\
    \integral{\cos x} &= \sin x + c \\
    \integral{\sin ax} &= \frac{\sin ax}{a} + c \\
    \integral{\sec^2x} &= \tan x + c
  \end{aligned}
  $$
