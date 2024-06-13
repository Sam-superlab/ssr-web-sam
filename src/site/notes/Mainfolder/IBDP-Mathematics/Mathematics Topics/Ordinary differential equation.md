---
{"dg-publish":true,"permalink":"/Mainfolder/IBDP-Mathematics/Mathematics Topics/Ordinary differential equation/"}
---

## Ordinary Differential Equation
- 1st Equation
	- 1st Linear diff 


### 1st diff Eq
- linear
$$y'+p(x)y=q(x)$$

Common Solution:
$$y=e^{-\int p(x)dx}[q(x)\cdot e^{\int p(x)dx}dx+C]$$

Integrating factor:
$$e^{\int p(x)dx}$$

- If Eq 
$$\int g(y)dy=\int f(x)dx$$
- w
## Homogeneous Differential Equation
$$\frac{dy}{dx}=f(\frac{y}{x})$$
Solution:
Let $\frac{y}{x}=u\to y=x\cdot u$  
$$\frac{dy}{dx}=\frac{udx}{dx}+\frac{xdu}{dx}$$
Then 
$$u+x\cdot \frac{du}{dx}$$
- Bonuli
In the form 
$$y'+p(x)y=q(x)y^n$$
1. Divded by $y^n$ or times $y^{-n}$ 
2. Let $y^{1-n}=u$ 

$$(1-n)y^{-n}y'=u'=\frac{du}{dx}$$
$$\frac{1}{1-n} \frac{du}{dx} +u\cdot p(x)=q(x)$$
- 全微分
In the form
$$P(x,y)dx+Q(x,y)dy=0$$
$$df=Pdx+Qdy$$
Solution:
$$f(x,y)=C$$
[[Mainfolder/IA/Math IA\|Math IA]] 