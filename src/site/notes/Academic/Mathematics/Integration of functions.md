---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Integration of functions/"}
---

# Multi-variable integration

## Double Integrals

### Definition:
A double integral allows you to integrate a function of two variables over a region in the plane. Given a function $f(x, y)$ and a region $R$ in the $xy$-plane, the double integral is written as:
$$
\iint_R f(x, y) \, dA
$$
Where $dA$ represents an infinitesimal area element in the plane.

### Geometric Interpretation:
The double integral represents the volume under the surface $z = f(x, y)$ over the region $R$. When $f(x, y) \geq 0$, the result is the volume trapped between the surface and the plane.

### Iterated Integrals:
A double integral can often be computed as two iterated integrals:
$$
\iint_R f(x, y) \, dA = \int_{a}^{b} \left( \int_{c(x)}^{d(x)} f(x, y) \, dy \right) dx
$$
Where $a$, $b$, $c(x)$, and $d(x)$ define the limits of the region $R$.

### Example:
Evaluate the double integral of $f(x, y) = x + y$ over the rectangle $R = [0, 2] \times [0, 3]$:
$$
\iint_R (x + y) \, dA = \int_0^2 \left( \int_0^3 (x + y) \, dy \right) dx
$$

First, integrate with respect to $y$:
$$
\int_0^3 (x + y) \, dy = [xy + \frac{y^2}{2}]_0^3 = 3x + \frac{9}{2}
$$

Then integrate with respect to $x$:
$$
\int_0^2 \left( 3x + \frac{9}{2} \right) dx = \left[ \frac{3x^2}{2} + \frac{9}{2}x \right]_0^2 = \left( \frac{12}{2} + 9 \right) = 15
$$

So, the value of the double integral is $15$.

---

## Polar Coordinates and Double Integrals

### Definition:
Polar coordinates provide an alternative to Cartesian coordinates for describing locations in the plane. A point in polar coordinates is represented as $(r, \theta)$, where:
- $r$ is the distance from the origin to the point.
- $\theta$ is the angle between the positive $x$-axis and the line segment connecting the origin to the point.

The conversion between Cartesian coordinates $(x, y)$ and polar coordinates $(r, \theta)$ is:
$$
x = r \cos \theta, \quad y = r \sin \theta
$$

### Double Integrals in Polar Coordinates:
To compute a double integral in polar coordinates, use the following formula:
$$
\iint_R f(x, y) \, dA = \iint_R f(r \cos \theta, r \sin \theta) \, r \, dr \, d\theta
$$
The extra factor of $r$ comes from the Jacobian determinant when changing variables.

### Example:
Find the area of the region inside the circle of radius 2 centered at the origin:
$$
\iint_R 1 \, dA = \int_0^{2\pi} \int_0^2 r \, dr \, d\theta
$$

First, integrate with respect to $r$:
$$
\int_0^2 r \, dr = \left[ \frac{r^2}{2} \right]_0^2 = 2
$$

Now, integrate with respect to $\theta$:
$$
\int_0^{2\pi} 2 \, d\theta = 2 \times 2\pi = 4\pi
$$

So, the area of the circle is $4\pi$.

---

## Triple Integrals

### Definition:
A triple integral allows you to integrate a function of three variables over a region in three-dimensional space. Given a function $f(x, y, z)$ and a region $D$ in space, the triple integral is written as:
$$
\iiint_D f(x, y, z) \, dV
$$
Where $dV$ represents an infinitesimal volume element.

### Example:
Evaluate the triple integral of $f(x, y, z) = x + y + z$ over the cube $[0, 1] \times [0, 1] \times [0, 1]$:
$$
\iiint_D (x + y + z) \, dV = \int_0^1 \int_0^1 \int_0^1 (x + y + z) \, dz \, dy \, dx
$$

First, integrate with respect to $z$:
$$
\int_0^1 (x + y + z) \, dz = [xz + yz + \frac{z^2}{2}]_0^1 = x + y + \frac{1}{2}
$$

Then, integrate with respect to $y$:
$$
\int_0^1 \left( x + y + \frac{1}{2} \right) \, dy = \left[ xy + \frac{y^2}{2} + \frac{y}{2} \right]_0^1 = x + \frac{1}{2} + \frac{1}{2} = x + 1
$$

Finally, integrate with respect to $x$:
$$
\int_0^1 (x + 1) \, dx = \left[ \frac{x^2}{2} + x \right]_0^1 = \frac{1}{2} + 1 = \frac{3}{2}
$$

So, the value of the triple integral is $\frac{3}{2}$.

---

## Sequences and Series

### Sequences:
A sequence is an ordered list of numbers, typically written as $\{a_n\}$, where $n$ represents the position in the sequence. 

- **Convergence of a Sequence**: A sequence $\{a_n\}$ converges to a limit $L$ if, as $n$ approaches infinity, the terms of the sequence approach $L$. Formally:
$$
\lim_{n \to \infty} a_n = L
$$

- **Divergence**: If a sequence does not converge to any finite limit, it is said to diverge.

### Series:
A series is the sum of the terms of a sequence. The most common type of series is the **infinite series**, denoted by:
$$
\sum_{n=1}^{\infty} a_n
$$

- **Geometric Series**: A geometric series has the form:
$$
\sum_{n=0}^{\infty} ar^n
$$
It converges if $|r| < 1$, and its sum is:
$$
S = \frac{a}{1 - r}
$$

### Integral Test:
If $f(x)$ is a continuous, positive, decreasing function, and $a_n = f(n)$, then the series $\sum_{n=1}^{\infty} a_n$ and the improper integral $\int_1^{\infty} f(x) \, dx$ either both converge or both diverge.

---
