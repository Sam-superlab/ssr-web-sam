---
{"dg-publish":true,"permalink":"/Mainfolder/IBDP-Mathematics/Derivatives/"}
---



## 1. Definition:
Partial derivatives represent the rate of change of a multivariable function with respect to one variable while keeping the others constant.

Given a function $f(x_1, x_2, \dots, x_n)$, the partial derivative of $f$ with respect to $x_i$ is:
$$
\frac{\partial f}{\partial x_i} \quad \text{or} \quad f_{x_i}
$$

## 2. Geometric Interpretation:
The partial derivative gives the slope of the surface along a specific axis:
- $\frac{\partial f}{\partial x}$: Slope along the $x$-axis, holding $y$ constant.
- $\frac{\partial f}{\partial y}$: Slope along the $y$-axis, holding $x$ constant.

## 3. Notation:
- $\frac{\partial f}{\partial x}$: Partial derivative with respect to $x$.
- $f_x(x, y)$: Another notation for the same.
- **Higher-order partial derivatives**: Derivatives of derivatives:
$$
\frac{\partial^2 f}{\partial x^2} \quad \text{or} \quad f_{xx}
$$

## 4. Chain Rule in Partial Derivatives:
If $z = f(x, y)$, and both $x$ and $y$ are functions of another variable $t$, then:
$$
\frac{dz}{dt} = \frac{\partial f}{\partial x} \cdot \frac{dx}{dt} + \frac{\partial f}{\partial y} \cdot \frac{dy}{dt}
$$

## 5. Mixed Partial Derivatives:
For functions with more variables, we can take partial derivatives with respect to different variables:
- $\frac{\partial^2 f}{\partial x \partial y}$
- $\frac{\partial^2 f}{\partial y \partial x}$

**Clairaut's Theorem**: If $f$ has continuous second-order partial derivatives, then:
$$
\frac{\partial^2 f}{\partial x \partial y} = \frac{\partial^2 f}{\partial y \partial x}
$$

## 6. Applications:
- **Optimization**: Finding critical points by solving $\nabla f = 0$ (the gradient is zero).
- **Tangent Planes**: The equation of the tangent plane to $z = f(x, y)$ at $(x_0, y_0, z_0)$ is:
$$
z - z_0 = f_x(x_0, y_0)(x - x_0) + f_y(x_0, y_0)(y - y_0)
$$
- **Differential Equations**: Many physical models are based on partial differential equations (PDEs).

## 7. Gradient:
The gradient of a function $f(x_1, x_2, \dots, x_n)$ is the vector of its partial derivatives:
$$
\nabla f = \left( \frac{\partial f}{\partial x_1}, \frac{\partial f}{\partial x_2}, \dots, \frac{\partial f}{\partial x_n} \right)
$$
The gradient points in the direction of the steepest ascent.

## 8. Example:

Given the function $f(x, y) = x^2y + 3xy^2$, the partial derivatives are:
- $\frac{\partial f}{\partial x} = 2xy + 3y^2$
- $\frac{\partial f}{\partial y} = x^2 + 6xy$

These derivatives represent the rates of change of $f$ with respect to $x$ and $y$.
