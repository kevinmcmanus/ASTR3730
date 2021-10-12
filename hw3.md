# Homework \#3
Kevin McManus

ASTR 3730

## Problem 1

### Problem 1a:  Find enclosed mass $m(r)$ and total mass M of the star in terms of $\rho_0$ and $R_0$ 
First find the derivative of volume with respect to radius:

$$
\begin{align}
V &= \frac{4}{3} \pi * r^3 \\ 
\frac{dV}{dr} &= 4 \pi * r^2
\end{align}
$$
Equation 2 is just the equation for surface area.

The mass at radius $r$ of an infinitely thin shell of the sphere of thickness $dr$ is the density at that radius $\rho(r)$ times the volume of that shell:
$$
\begin{equation}
dm = \rho(r)*dV
\end{equation}
$$
Substitute in Equation 2 to get:

$$
\begin{equation}
dm = \rho(r)*4 \pi * r^2\ dr
\end{equation}
$$
and insert the expression for $\rho(r)$:

$$
\begin{equation}
dm = \rho_0(1-r/R_0)*4 \pi * r^2\ dr
\end{equation}
$$
To get $m(r)$, the enclosed mass at radius $r$, integrate Equation 5 from $r'=0$ to $r'=r$:

$$
\begin{align}
m(r) &= \int_0^r \rho_0(1-r'/R_0)*4 \pi * r'^2\ dr' \\ 
&= 4\pi\rho_0 \int_0^r (1-r'/R_0) * r'^2\ dr' \\
&= 4\pi\rho_0(\frac{1}{3}r'^3 - \frac{1}{4R_0}r'^4 +C)\Big|_0^r \\
&= 4\pi\rho_0(\frac{1}{3}r^3 - \frac{1}{4R_0}r^4)
\end{align}
$$
since $m(r=0)=0$. So the equation for mass as a function of $r$, $\rho_0$ and $R_0$ is:
$$
\begin{align}
m(r) = 4\pi\rho_0(\frac{1}{3}r^3 - \frac{1}{4R_0}r^4)
\end{align}
$$

To get the total mass of the star, evaluate Equation 10 at $r=R_0$:
$$
\begin{align}
m(R_0) &= 4\pi\rho_0(\frac{1}{3}R_0^3 - \frac{1}{4R_0}R_0^4) \\
&=4\pi\rho_0(4R_0^4 - 3R_0^4/12R_0) \\
&=\frac{1}{3}\pi\rho_0R_0^3
\end{align}
$$

The total mass of the star is therefore $M = \frac{1}{3}\pi\rho_0R_0^3$ where $R_0$ is its radius.