---
{"dg-publish":true,"permalink":"/Mainfolder/Mathematics/Maximum and Minimum in multivariable calculus/"}
---

**Maximum and Minimum Values in Multivariable Functions**

In this section, we explore how to find maximum and minimum values for functions of multiple variables. These concepts extend single-variable calculus concepts to higher dimensions, particularly for functions of two variables.

**Local Maximum and Minimum**
A function $f(x, y)$ has a **local maximum** at a point $(a, b)$ if $f(a, b) \geq f(x, y)$ for all points $(x, y)$ in a small neighborhood around $(a, b)$. Similarly, it has a **local minimum** at $(a, b)$ if $f(a, b) \leq f(x, y)$ in the vicinity. If these conditions hold for all points in the function’s domain, they represent an **absolute maximum** or **absolute minimum**.

**Critical Points**
Critical points are potential locations for these maximum or minimum values. For a function $f(x, y)$, a critical point occurs where both partial derivatives are zero:

$$\frac{\partial f}{\partial x} = 0 \text{ and } \frac{\partial f}{\partial y} = 0.$$

  

If one or both of the partial derivatives fail to exist, this point is still considered critical if it results in an extreme value for $f(x, y)$.

  

**The Second Derivative Test**

  

To classify a critical point $(a, b)$ as a local maximum, minimum, or saddle point, we compute the second partial derivatives:

  

1. Let $D = f_{xx}(a, b)f_{yy}(a, b) - (f_{xy}(a, b))^2$:

• **If** $D > 0$ and $f_{xx}(a, b) > 0$, then $f(a, b)$ is a local minimum.

• **If** $D > 0$ and $f_{xx}(a, b) < 0$, then $f(a, b)$ is a local maximum.

• **If** $D < 0$, $(a, b)$ is a saddle point.

• **If** $D = 0**, the test is inconclusive.

  

**Examples**

  

• **Example 1**: For $f(x, y) = x^2 + y^2$, the only critical point is $(0, 0)$. Here, $f_{xx} = f_{yy} = 2$ and $f_{xy} = 0$, so $D = 4 > 0$ and $f_{xx} > 0$, indicating a local (and absolute) minimum at $(0, 0)$.

• **Example 2**: To maximize the volume of an open box under material constraints, we set up the function for volume and apply the method for boundary conditions alongside critical points to find maximum volume.

  

**Absolute Maximum and Minimum on Closed and Bounded Sets**

  

The **Extreme Value Theorem for Functions of Two Variables** states that if a function $f(x, y)$ is continuous on a closed, bounded set $D$, it must attain an absolute maximum and minimum within $D$. To find these extreme values:

  

1. Evaluate $f$ at all critical points within $D$.

2. Evaluate $f$ along the boundary of $D$.

3. Compare these values to identify the absolute extrema.

  

**Using Boundary Points for Optimization**

On closed, bounded regions, boundary points can hold extreme values. To find these:

1. Parameterize the boundary as needed (e.g., substituting $y = f(x)$ for a region).

2. Compute derivatives along the boundary.

3. Use single-variable calculus to analyze each segment of the boundary.
