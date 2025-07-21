---
{"dg-publish":true,"permalink":"/Academic/Mathematics/Partial Derivatives/"}
---



- [[Academic/Mathematics/Partial Derivatives#Definition:\|Definition:]]
	- [[Academic/Mathematics/Partial Derivatives#Definition:\|Example:]]
- [[Academic/Mathematics/Partial Derivatives#Geometric Interpretation:\|Geometric Interpretation:]]
	- [[Academic/Mathematics/Partial Derivatives#Geometric Interpretation:\|Visualizing Partial Derivatives:]]
- [[Academic/Mathematics/Partial Derivatives#Higher-Order Partial Derivatives:\|Higher-Order Partial Derivatives:]]
	- [[Academic/Mathematics/Partial Derivatives#Higher-Order Partial Derivatives:\|Clairaut’s Theorem on Mixed Partial Derivatives:]]
	- [[Academic/Mathematics/Partial Derivatives#Higher-Order Partial Derivatives:\|Example of Higher-Order Partial Derivatives:]]
- [[Academic/Mathematics/Partial Derivatives#Chain Rule for Partial Derivatives:\|Chain Rule for Partial Derivatives:]]
	- [[Academic/Mathematics/Partial Derivatives#Chain Rule for Partial Derivatives:\|Example:]]
- [[Academic/Mathematics/Partial Derivatives#Gradient:\|Gradient:]]
	- [[Academic/Mathematics/Partial Derivatives#Gradient:\|Geometric Interpretation of the Gradient:]]
	- [[Academic/Mathematics/Partial Derivatives#Gradient:\|Example:]]
- [[Academic/Mathematics/Partial Derivatives#Applications of Partial Derivatives:\|Applications of Partial Derivatives:]]
	- [[Academic/Mathematics/Partial Derivatives#Applications of Partial Derivatives:\|Optimization:]]
	- [[Academic/Mathematics/Partial Derivatives#Applications of Partial Derivatives:\|Example:]]
	- [[Academic/Mathematics/Partial Derivatives#Applications of Partial Derivatives:\|Tangent Planes:]]
	- [[Academic/Mathematics/Partial Derivatives#Applications of Partial Derivatives:\|Example:]]



# Partial Derivatives

## Definition:
Partial derivatives measure how a multivariable function changes as one of its variables is varied, while keeping the other variables constant. Given a function $f(x_1, x_2, \dots, x_n)$, the partial derivative of $f$ with respect to $x_i$ is denoted by:
$$
\frac{\partial f}{\partial x_i} \quad \text{or} \quad f_{x_i}
$$

This notation indicates that we treat all other variables $(x_1, x_2, \dots, x_{i-1}, x_{i+1}, \dots, x_n)$ as constants and differentiate with respect to $x_i$.

### Example:
Consider a function $f(x, y) = 3x^2y + 2y^2$. The partial derivative of $f$ with respect to $x$ is:
$$
\frac{\partial f}{\partial x} = 6xy
$$
Here, $y$ is treated as a constant. Similarly, the partial derivative of $f$ with respect to $y$ is:
$$
\frac{\partial f}{\partial y} = 3x^2 + 4y
$$

## Geometric Interpretation:
Partial derivatives give us the slope of the function along a specific axis. For a function $f(x, y)$, the partial derivative $\frac{\partial f}{\partial x}$ represents the rate of change of $f$ with respect to $x$, while holding $y$ constant. This is equivalent to slicing the surface $z = f(x, y)$ parallel to the $yz$-plane and examining the slope of the curve along the $x$-direction.

Similarly, $\frac{\partial f}{\partial y}$ represents the rate of change of $f$ in the $y$-direction, with $x$ held constant.

### Visualizing Partial Derivatives:
Consider a surface $z = f(x, y)$. The partial derivative $\frac{\partial f}{\partial x}$ corresponds to the slope of the tangent line in the direction of the $x$-axis at any point $(x, y)$. Geometrically, this is the slope of the curve you would see if you "cut" the surface along a plane parallel to the $yz$-plane. Similarly, $\frac{\partial f}{\partial y}$ is the slope of the tangent line in the direction of the $y$-axis.

## Higher-Order Partial Derivatives:
Just like with single-variable functions, we can take higher-order derivatives in multivariable functions. A second-order partial derivative is obtained by differentiating a first-order partial derivative. There are several types of second-order partial derivatives:
- $\frac{\partial^2 f}{\partial x^2}$: The second derivative of $f$ with respect to $x$ twice (also called the second-order derivative in $x$).
- $\frac{\partial^2 f}{\partial y^2}$: The second derivative of $f$ with respect to $y$ twice.
- $\frac{\partial^2 f}{\partial x \partial y}$ or $\frac{\partial^2 f}{\partial y \partial x}$: Mixed partial derivatives.

### Clairaut’s Theorem on Mixed Partial Derivatives:
If the mixed partial derivatives are continuous, then the order of differentiation does not matter. That is:
$$
\frac{\partial^2 f}{\partial x \partial y} = \frac{\partial^2 f}{\partial y \partial x}
$$

### Example of Higher-Order Partial Derivatives:
For the function $f(x, y) = x^3y^2 + 4xy$, the second-order partial derivatives are:
- $\frac{\partial^2 f}{\partial x^2} = 6xy^2 + 4y$
- $\frac{\partial^2 f}{\partial y^2} = 2x^3$
- Mixed partial derivatives: $\frac{\partial^2 f}{\partial x \partial y} = \frac{\partial^2}{\partial x}(3x^2y^2 + 4y) = 6x^2y + 4$

## Chain Rule for Partial Derivatives:
The chain rule in the context of partial derivatives allows us to differentiate composite functions. Suppose $z = f(x, y)$ and both $x$ and $y$ are functions of another variable $t$. The chain rule expresses the derivative of $z$ with respect to $t$ as:
$$
\frac{dz}{dt} = \frac{\partial f}{\partial x} \frac{dx}{dt} + \frac{\partial f}{\partial y} \frac{dy}{dt}
$$

This can be generalized for functions of more variables and multiple intermediate dependencies.

### Example:
Let $z = x^2 + xy$, where $x = t^2$ and $y = e^t$. Using the chain rule:
$$
\frac{dz}{dt} = \frac{\partial z}{\partial x} \frac{dx}{dt} + \frac{\partial z}{\partial y} \frac{dy}{dt}
$$
We calculate:
$$
\frac{\partial z}{\partial x} = 2x + y, \quad \frac{\partial z}{\partial y} = x
$$
Substituting $x = t^2$ and $y = e^t$:
$$
\frac{dz}{dt} = (2t^2 + e^t)(2t) + (t^2)(e^t)
$$


## Applications of Partial Derivatives:

### Optimization:
Partial derivatives are essential in finding the local maxima and minima of functions of multiple variables. To find critical points (where the function might have a local max or min), you set the gradient equal to zero:
$$
\nabla f = \mathbf{0}
$$

Solving this system of equations provides the critical points. From there, the second derivative test (involving second-order partial derivatives) can help determine whether the critical point is a local maximum, local minimum, or a saddle point.

### Example:
Consider the function $f(x, y) = x^2 + y^2 + 2x - 4y$. The partial derivatives are:
$$
\frac{\partial f}{\partial x} = 2x + 2, \quad \frac{\partial f}{\partial y} = 2y - 4
$$
Setting both derivatives to zero:
$$
2x + 2 = 0 \quad \text{and} \quad 2y - 4 = 0
$$
Solving these equations gives the critical point $(x, y) = (-1, 2)$.

### Tangent Planes:
The equation of a tangent plane to a surface $z = f(x, y)$ at the point $(x_0, y_0, z_0)$ can be written as:
$$
z - z_0 = f_x(x_0, y_0)(x - x_0) + f_y(x_0, y_0)(y - y_0)
$$
This gives a linear approximation of the surface near the point $(x_0, y_0, z_0)$.

### Example:
For the function $f(x, y) = x^2 + y^2$, find the equation of the tangent plane at the point $(1, 1, 2)$:
The partial derivatives are:
$$
f_x(x, y) = 2x, \quad f_y(x, y) = 2y
$$
At the point $(1, 1)$:
$$
f_x(1, 1) = 2, \quad f_y(1, 1) = 2
$$
Thus, the equation of the tangent plane is:
$$
z - 2 = 2(x - 1) + 2(y - 1)
$$
Simplifying:
$$
z = 2x + 2y - 2
$$
