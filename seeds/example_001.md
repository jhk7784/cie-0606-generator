# Example Question: Logarithms + Differentiation

## Skills Used
- LOG-003: Solving exponential equations with logs
- CALC-008: Tangent and normal

## Paper Type
Paper 1

## Question

The curve $C$ has equation $y = e^{2x} - 4e^x + 3$.

**(a)** Find the coordinates of the points where $C$ crosses the x-axis. [4]

**(b)** Find $\frac{dy}{dx}$. [2]

**(c)** Find the equation of the tangent to $C$ at the point where $x = \ln 2$. [4]

**[10 marks]**

---

## Mark Scheme

**(a)**
At x-axis, $y = 0$
$e^{2x} - 4e^x + 3 = 0$ **M1**

Let $u = e^x$:
$u^2 - 4u + 3 = 0$ **M1**
$(u - 1)(u - 3) = 0$
$u = 1$ or $u = 3$ **A1**

$e^x = 1 \Rightarrow x = 0$
$e^x = 3 \Rightarrow x = \ln 3$ **A1**

Points: $(0, 0)$ and $(\ln 3, 0)$

**(b)**
$\frac{dy}{dx} = 2e^{2x} - 4e^x$ **M1 A1**

**(c)**
When $x = \ln 2$:
$y = e^{2\ln 2} - 4e^{\ln 2} + 3 = 4 - 8 + 3 = -1$ **A1**

$\frac{dy}{dx} = 2e^{2\ln 2} - 4e^{\ln 2} = 8 - 8 = 0$ **A1**

Gradient = 0, so tangent is horizontal **M1**
Equation: $y = -1$ **A1**

---

## Difficulty Rating
**4/7** — Standard application combining log/exponential work with calculus

## Skill Integration
The question requires recognizing $e^{2x} = (e^x)^2$ to form a quadratic (LOG-003), then using differentiation of exponentials to find the tangent (CALC-008). Neither skill is decorative - both are essential.
