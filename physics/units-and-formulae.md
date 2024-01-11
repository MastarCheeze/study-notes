# Units

## Base units

| Quantity                                               | Sym.     | Unit                                 |
| ------------------------------------------------------ | -------- | ------------------------------------ |
| [Mass](./mass-and-weight.md)                           | $m$      | kilogram $(\mathrm{kg})$             |
| Length                                                 |          | metre $(\mathrm{m})$                 |
| Time                                                   | $t$      | second $(\mathrm{s})$                |
| [Current](./current-voltage-and-resistance.md#current) | $I$      | ampere $(\mathrm{A})$                |
| Temperature                                            | $\theta$ | [kelvin $(\mathrm{K})$](./kelvin.md) |
| [Amount of substance](../chemistry/moles.md)           |          | mole $(\mathrm{mol})$                |
| Luminous intensity                                     |          | candela $(\mathrm{cd})$              |

## Derived units

| Quantity                                                         | Sym.      | Unit                   |                             |                  |
| ---------------------------------------------------------------- | --------- | ---------------------- | --------------------------- | ---------------- |
| Volume                                                           | $V$       |                        | $\mathrm{m^3}$              |                  |
| Density                                                          | $𝜌$       |                        | $\mathrm{kg/m^3}$           |                  |
| Speed/Velocity                                                   | $v$       |                        | $\mathrm{m/s}$              |                  |
| Acceleration                                                     | $a$       |                        | $\mathrm{m/s^2}$            |                  |
| [Force](./newtons-laws-of-motion.md#second-law)                  | $F$       | newton $(\mathrm{N})$  | $\mathrm{kg~m/s^2}$         |                  |
| [Gravitational field strength](./mass-and-weight.md)             | $g$       |                        | $\mathrm{m/s^2}$            | $\mathrm{N/kg}$  |
| [Momentum](./momentum.md)                                        | $p$       |                        | $\mathrm{kg~m/s}$           | $\mathrm{N~s}$   |
| [Moment of force (torque)](./moment-of-force.md)                 | $M$       |                        | $\mathrm{N~m}$              |                  |
| [Spring constant](./hookes-law.md)                               | $k$       |                        | $\mathrm{N/m}$              |                  |
| [Pressure](./pressure.md)                                        | $p$       | pascal $(\mathrm{Pa})$ | $\mathrm{N/m^2}$            |                  |
| [Energy](./energy.md)                                            | $E$       | joule $(\mathrm{J})$   | $\mathrm{N~m}$              |                  |
| [Power](./power.md)                                              | $P$       | watt $(\mathrm{W})$    | $\mathrm{J/s}$              | $\mathrm{N~m/s}$ |
| [Specific heat capacity](./specific-heat-capacity.md)            | $c$       |                        | $\mathrm{J/(kg~\degree C)}$ |                  |
| [Thermal capacity](./specific-heat-capacity.md#thermal-capacity) | $C$       |                        | $\mathrm{J/\degree C}$      |                  |
| [Specific latent heat](./latent-heat.md)                         | $L$       |                        | $\mathrm{J/kg}$             |                  |
| [Frequency](./waves.md#properties-of-waves)                      | $\lambda$ | hertz $(\mathrm{Hz})$  | $\mathrm{1/s}$              |                  |
| [Charge](./charge.md)                                            | $Q$       | coulomb $(\mathrm{C})$ | $\mathrm{A~s}$              |                  |
| [Voltage](./current-voltage-and-resistance.md#voltage)           | $V$       | volt $(\mathrm{V})$    | $\mathrm{J/C}$              |                  |
| [Resistance](./current-voltage-and-resistance.md#resistance)     | $R$       | ohm $(\Omega)$         | $\mathrm{V/A}$              |                  |

<br>

# Formulae

## Kinematics

$$
\begin{aligned}
  v &= \frac{\Delta d}{\Delta t} \\
  a &= \frac{\Delta v}{\Delta t} = \frac{v-u}{t} \\
\end{aligned}
$$

## Dynamics

$$
\begin{aligned}
  \tag*{\scriptsize (Newton's 2nd law)} F &= ma \\
  p &= mv \\
  \Delta p &= F\Delta t \\
  F &= \frac{\Delta p}{\Delta t} = \frac{m(v-u)}{\Delta t} \\
  F &= mg \\
  M &= Fd \\
\end{aligned}
$$

## Energy

$$
\begin{aligned}
  W &= Fd \\
  \text{GPE} &= \mathrm{mgh} \\
  \text{KE} &= \frac{1}{2}mv^2 \\
  P &= \frac{E}{t}
\end{aligned}
$$

## Solid mechanics

$$
\begin{aligned}
  F &= kx \\
\end{aligned}
$$

## Thermodynamics

$$
\begin{aligned}
  p &= \frac{F}{A} \\
  p &= \rho gh \\
  p_1V_1 &= p_2V_2 \\
  E &= mc\Delta\theta \\
  E &= C\Delta\theta \\
  E &= mL \\
\end{aligned}
$$

## Electricity

$$
\begin{aligned}
  Q &= It \\
  V &= \frac{E}{Q} \\
  V &= IR \\
  P &= VI \\
  E &= VIt
\end{aligned}
$$

#### Series

$$
\begin{aligned}
  A&=A_1=A_2=\dots=A_n \\
  V&=V_1+V_2+\dots+V_n \\
  R&=R_1+R_2+\dots+R_n
\end{aligned}
$$

#### Parallel
$$
\begin{aligned}
  A&=A_1+A_2+\dots+A_n \\
  V&=V_1=V_2=\dots=V_n \\
  \frac{1}{R}&=\frac{1}{R_1}+\frac{1}{R_2}+\dots+\frac{1}{R_n} \\
  R&=\frac{R_1\cdot R_2}{R_1+R_2}
\end{aligned}
$$

#### Potential divider

$$\frac{V_{\text{in}}}{R_\text{total}} = \frac{V_{\text{out}}}{R_\text{out}}$$

#### Transformer

$$
\begin{aligned}
  \frac{V_p}{N_p} &= \frac{V_s}{N_s} \\
  V_pI_p &= V_sI_s \\
\end{aligned}
$$

## Light

$$
\begin{aligned}
  n &= \frac{c}{v} = \frac{\sin i}{\sin r} \\
  n &= \frac{\sin 90\degree}{\sin c} = \frac{1}{\sin c} \\
\end{aligned}
$$

## Waves

$$
\begin{aligned}
  v &= f\lambda \\
  f &= \frac{1}{T} \\
\end{aligned}
$$

## Space

$$
\begin{aligned}
  H_0 &= \frac{v}{d} \\
  t &= \frac{1}{H_0} \\
\end{aligned}
$$

<br>

# Constants

$$
\begin{aligned}
  c &= 3\cdot10^8 \text{ m/s} \\
  \text{sound \scriptsize(air)} &= 340 \text{ m/s} \\
  \text{sound \scriptsize(water)} &= 1500 \text{ m/s} \\
  H_0 &= 2.3 \cdot 10^{-18} \\
  \text{light year} &= 9.5 \cdot 10^{15} \text{~m}
\end{aligned}
$$
