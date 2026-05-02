# Orthogonal Polynomials: A Comprehensive Guide

Orthogonal polynomials play a fundamental role in mathematics, physics, and engineering. They arise naturally in the solution of differential equations, approximation theory, numerical integration (Gaussian quadrature), and many other areas. This post provides a clear, sequential overview of five important families of orthogonal polynomials: **Legendre**, **Chebyshev (First Kind)**, **Chebyshev (Second Kind)**, **Laguerre**, and **Hermite**.

For each family, we cover:
- The **original/primary definition**
- The **three-term recurrence relation**
- The **weight function** for the inner product
- The **orthogonality (inner product) result**

All polynomials are assumed to be of degree \( n \), with leading coefficient conventions as standard in the literature.

## 1. Legendre Polynomials \( P_n(x) \)

**Definition**  
Legendre polynomials are most commonly defined via **Rodrigues' formula**:
$$
P_n(x) = \frac{1}{2^n n!} \frac{d^n}{dx^n} (x^2 - 1)^n, \quad n = 0,1,2,\dots
$$
They can also be defined as the solutions to Legendre's differential equation:
$$
(1 - x^2) y'' - 2x y' + n(n+1) y = 0
$$
on the interval \( [-1, 1] \), with \( P_n(1) = 1 \).

**Three-term Recurrence**  
$$
(n+1) P_{n+1}(x) = (2n + 1) x P_n(x) - n P_{n-1}(x)
$$
with initial conditions \( P_0(x) = 1 \), \( P_1(x) = x \).

**Weight Function**  
The weight function is \( w(x) = 1 \) on \( [-1, 1] \).

**Inner Product (Orthogonality)**  
$$
\int_{-1}^{1} P_m(x) P_n(x) \, dx = \frac{2}{2n + 1} \delta_{mn}
$$

## 2. Chebyshev Polynomials of the First Kind \( T_n(x) \)

**Definition**  
The Chebyshev polynomials of the first kind have a beautiful trigonometric definition:
$$
T_n(x) = \cos(n \theta), \quad \text{where } x = \cos \theta, \quad \theta \in [0, \pi]
$$
or equivalently,
$$
T_n(x) = \cos(n \arccos x), \quad x \in [-1, 1].
$$
They satisfy the differential equation:
$$
(1 - x^2) y'' - x y' + n^2 y = 0.
$$

**Three-term Recurrence**  
$$
T_{n+1}(x) = 2x T_n(x) - T_{n-1}(x)
$$
with \( T_0(x) = 1 \), \( T_1(x) = x \).

**Weight Function**  
The weight function is \( w(x) = \frac{1}{\sqrt{1 - x^2}} \) on \( [-1, 1] \).

**Inner Product (Orthogonality)**  
$$
\int_{-1}^{1} \frac{T_m(x) T_n(x)}{\sqrt{1 - x^2}} \, dx = 
\begin{cases} 
0 & m \neq n \\
\pi & m = n = 0 \\
\frac{\pi}{2} & m = n \geq 1 
\end{cases}
$$

## 3. Chebyshev Polynomials of the Second Kind \( U_n(x) \)

**Definition**  
The second-kind Chebyshev polynomials are defined as:
$$
U_n(x) = \frac{\sin((n+1) \theta)}{\sin \theta}, \quad x = \cos \theta
$$
or
$$
U_n(x) = \frac{\sin((n+1) \arccos x)}{\sqrt{1 - x^2}}.
$$
They satisfy the differential equation:
$$
(1 - x^2) y'' - 3x y' + n(n+2) y = 0.
$$

**Three-term Recurrence**  
$$
U_{n+1}(x) = 2x U_n(x) - U_{n-1}(x)
$$
with \( U_0(x) = 1 \), \( U_1(x) = 2x \).

**Weight Function**  
The weight function is \( w(x) = \sqrt{1 - x^2} \) on \( [-1, 1] \).

**Inner Product (Orthogonality)**  
$$
\int_{-1}^{1} U_m(x) U_n(x) \sqrt{1 - x^2} \, dx = \frac{\pi}{2} \delta_{mn}
$$

## 4. Laguerre Polynomials \( L_n(x) \)

**Definition**  
Laguerre polynomials are defined on \( [0, \infty) \) via **Rodrigues' formula**:
$$
L_n(x) = \frac{e^x}{n!} \frac{d^n}{dx^n} (x^n e^{-x}), \quad n = 0,1,2,\dots
$$
They solve Laguerre's differential equation:
$$
x y'' + (1 - x) y' + n y = 0.
$$
The standard convention has \( L_n(0) = 1 \) and leading coefficient \( (-1)^n / n! \).

**Three-term Recurrence**  
$$
(n+1) L_{n+1}(x) = (2n + 1 - x) L_n(x) - n L_{n-1}(x)
$$
with \( L_0(x) = 1 \), \( L_1(x) = 1 - x \).

**Weight Function**  
The weight function is \( w(x) = e^{-x} \) on \( [0, \infty) \).

**Inner Product (Orthogonality)**  
$$
\int_{0}^{\infty} L_m(x) L_n(x) e^{-x} \, dx = \delta_{mn}
$$

## 5. Hermite Polynomials \( H_n(x) \) (Physicist's Version)

**Definition**  
Hermite polynomials (physicist's convention) are defined via Rodrigues' formula:
$$
H_n(x) = (-1)^n e^{x^2} \frac{d^n}{dx^n} e^{-x^2}, \quad n = 0,1,2,\dots
$$
They satisfy Hermite's differential equation:
$$
y'' - 2x y' + 2n y = 0.
$$
They are orthogonal on the entire real line.

**Three-term Recurrence**  
$$
H_{n+1}(x) = 2x H_n(x) - 2n H_{n-1}(x)
$$
with \( H_0(x) = 1 \), \( H_1(x) = 2x \).

**Weight Function**  
The weight function is \( w(x) = e^{-x^2} \) on \( (-\infty, \infty) \).

**Inner Product (Orthogonality)**  
$$
\int_{-\infty}^{\infty} H_m(x) H_n(x) e^{-x^2} \, dx = \sqrt{\pi} \, 2^n n! \, \delta_{mn}
$$
