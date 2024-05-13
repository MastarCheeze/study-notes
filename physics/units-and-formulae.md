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

| Quantity                                                           | Sym.      | Unit                   |                             |                    |
| ------------------------------------------------------------------ | --------- | ---------------------- | --------------------------- | ------------------ |
| Volume                                                             | $V$       |                        | $\mathrm{m^3}$              |                    |
| Density                                                            | $𝜌$       |                        | $\mathrm{kg/m^3}$           |                    |
| Speed/Velocity                                                     | $v$       |                        | $\mathrm{m/s}$              |                    |
| Acceleration                                                       | $a$       |                        | $\mathrm{m/s^2}$            |                    |
| [Force](./newtons-laws-of-motion.md#second-law)                    | $F$       | newton $(\mathrm{N})$  | $\mathrm{kg~m/s^2}$         |                    |
| [Gravitational field strength](./mass-and-weight.md)               | $g$       |                        | $\mathrm{m/s^2}$            | $\mathrm{N/kg}$    |
| [Momentum](./momentum.md)                                          | $p$       |                        | $\mathrm{kg~m/s}$           | $\mathrm{N~s}$     |
| [Moment of force (torque)](./moment-of-force.md)                   | $M$       |                        | $\mathrm{N~m}$              |                    |
| [Spring constant](./hookes-law.md)                                 | $k$       |                        | $\mathrm{N/m}$              |                    |
| [Pressure](./pressure.md)                                          | $P$       | pascal $(\mathrm{Pa})$ | $\mathrm{N/m^2}$            |                    |
| [Energy](./energy.md)                                              | $E$       | joule $(\mathrm{J})$   | $\mathrm{N~m}$              | $\mathrm{kWh}$[^1] |
| [Power](./power.md)                                                | $P$       | watt $(\mathrm{W})$    | $\mathrm{J/s}$              | $\mathrm{N~m/s}$   |
| [Specific heat capacity](./specific-heat-capacity.md)              | $c$       |                        | $\mathrm{J/(kg~\degree C)}$ |                    |
| [Thermal capacity\*](./specific-heat-capacity.md#thermal-capacity) | $C$       |                        | $\mathrm{J/\degree C}$      |                    |
| [Specific latent heat\*](./latent-heat.md)                         | $L$       |                        | $\mathrm{J/kg}$             |                    |
| [Frequency](./waves.md#properties-of-waves)                        | $\lambda$ | hertz $(\mathrm{Hz})$  | $\mathrm{1/s}$              |                    |
| [Charge](./charge.md)                                              | $Q$       | coulomb $(\mathrm{C})$ | $\mathrm{A~s}$              |                    |
| [Voltage](./current-voltage-and-resistance.md#voltage)             | $V$       | volt $(\mathrm{V})$    | $\mathrm{J/C}$              |                    |
| [Resistance](./current-voltage-and-resistance.md#resistance)       | $R$       | ohm $(\Omega)$         | $\mathrm{V/A}$              |                    |

[^1]: $\mathrm{1~kWh = 3.6\cdot10^6~J}$

<br>

# Formulae

$$
\begin{align*}
    \tag*{\scriptsize (density)} \rho = \frac{m}{V} \\
\end{align*}
$$

## Kinematics

$$
\begin{align*}
  v &= \frac{\Delta d}{\Delta t} \\
  a &= \frac{\Delta v}{\Delta t} = \frac{v-u}{t} \\
  s &= \frac{1}{2}vt = \frac{1}{2}at^2
\end{align*}
$$

## Dynamics

$$
\begin{align*}
  \tag*{\scriptsize (Newton's 2nd law)} F &= ma \\
  p &= mv \\
  \Delta p &= Ft \\
  F &= \frac{\Delta p}{t} = \frac{m(v-u)}{t} \\
  \tag*{\scriptsize ~~~~~~~~~~~~~~~~~~~(weight)} F &= mg \\
  \tag*{\scriptsize ~~~(moment of force)} M &= Fd \\
\end{align*}
$$

## Energy

$$
\begin{align*}
  W &= Fd \\
  \text{GPE} &= \mathrm{mgh} \\
  \text{KE} &= \frac{1}{2}mv^2 \\
  P &= \frac{E}{t}
\end{align*}
$$

## Solid mechanics

$$
\begin{align*}
  \tag*{\scriptsize (Hooke's law)} F &= kx \\
  \frac{F_1}{x_1} &= \frac{F_2}{x_2} \\
\end{align*}
$$

## Thermodynamics

$$
\begin{align*}
  P &= \frac{F}{A} \\
  P &= \rho gh \\
  \tag*{\scriptsize (Boyle's law)} P_1V_1 &= P_2V_2 \\
  E &= mc\Delta\theta \\
  E &= C\Delta\theta \text{ *} \\
  E &= mL \text{ *} \\
\end{align*}
$$

## Electricity

$$
\begin{align*}
  Q &= It \\
  V &= \frac{E}{Q} \\
  V &= IR \\
  R &= \rho \cdot \frac{l}{A} \\
  P &= VI \\
  E &= VIt \\
  \text{efficiency} &= \frac{\text{useful output}}{\text{total input}} \cdot 100\%
\end{align*}
$$

#### Series

$$
\begin{align*}
  I&=I_1=I_2=\dots=I_n \\
  V&=V_1+V_2+\dots+V_n \\
  R&=R_1+R_2+\dots+R_n
\end{align*}
$$

#### Parallel

$$
\begin{align*}
  I&=I_1+I_2+\dots+I_n \\
  V&=V_1=V_2=\dots=V_n \\
  \frac{1}{R}&=\frac{1}{R_1}+\frac{1}{R_2}+\dots+\frac{1}{R_n} \\
  R&=\frac{R_1\cdot R_2}{R_1+R_2}
\end{align*}
$$

#### Potential divider

$$
\begin{align*}
  \frac{V_{\text{in}}}{R_\text{total}} &= \frac{V_{\text{out}}}{R_\text{out}}
\end{align*}
$$

#### Transformer

$$
\begin{align*}
  \frac{V_p}{N_p} &= \frac{V_s}{N_s} \\
  V_pI_p &= V_sI_s \\
\end{align*}
$$

## Light

$$
\begin{align*}
  \tag*{\scriptsize (Snell's law)} n &= \frac{c}{v} = \frac{\sin i}{\sin r} \\
  n &= \frac{\sin 90\degree}{\sin c} = \frac{1}{\sin c} \\
\end{align*}
$$

## Waves

$$
\begin{align*}
  v &= f\lambda \\
  f &= \frac{1}{T} \\
\end{align*}
$$

## Nuclear

$$
\begin{align*}
  N &= \frac{N_0}{2^{\frac{t}{h}}} \\
\end{align*}
$$

## Space

$$
\begin{align*}
  \tag*{\scriptsize ~~~(Hubble's law)} H_0 &= \frac{v}{d} \\
  \tag*{\scriptsize (age of universe)} t &= \frac{1}{H_0} \\
\end{align*}
$$

<br>

# Constants

$$
\begin{align*}
  \text{absolute zero} &= -273\degree \mathrm{C} \\
  c &= 3.0\cdot10^8 \text{ m/s} \\
  \text{sound \scriptsize(air)} &= 340 \text{ m/s} \\
  \text{sound \scriptsize(water)} &= 1500 \text{ m/s} \\
  \tag*{\scriptsize (Hubble constant)} H_0 &= 2.2 \cdot 10^{-18} \text{ s}^{-1} \\
  \text{light year} &= 9.5 \cdot 10^{15} \text{ m}
\end{align*}
$$
