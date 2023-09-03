[[12 - Differentiation]]
## Integrating Standard Functions
\
 $$ \int x^n dx = \frac{x^n + 1}{n + 1} + c$$
\
$$ \int e^x dx = e^x + c$$
\
$$ \int \frac{1}{x} = ln|x| + c$$
\
$$\int cos(x) dx = sin(x) +c$$
\
$$\int sin(x)dx=-cos(x)+c$$
\
$$\int sec^2(x)dx=tan(x)+c$$
\
$$\int cosec(x)cot(x)dx=-cosec(x)+c$$
\
$$\int cosec^2(x)dx = -cot(x)+c$$
\
$$\int sec(x)tan(x)dx = sec(x)+c$$
## Reverse Chain Rule
\
$$\int sin(ax+b)dx = \frac{-cos(ax+b)}{a} +c$$
\
$$\int e^{ax+b}dx = \frac{1}{a}e^{ax+b}+c$$
\
In general:
$$\int f'(ax+b)dx = \frac{1}{a}f(ax+b)+c$$

## Integration by Substitution

\
$$I = \int x \sqrt{ax+b}*dx$$
Let:$$u = ax+b$$
So: $$\frac{du}{dx} = a$$
Substituting into the original equation: $$I = \int \frac{u-b}{a}u^{\frac{1}{2}}*\frac{du}{a}$$
Simplifying gives: $$I = \frac{1}{a^2}\int u^{\frac{3}{2}}-u^{\frac{1}{2}}b*du$$
Integrating then gives: $$I = \frac{1}{a^2}(\frac{2u^{\frac{5}{2}}}{5} - \frac{2u^{\frac{3}{2}}b}{3}+c)$$
Then substitute $x$ back into the equation using $u=ax+b$: $$I = \frac{2(ax+b)^{\frac{5}{2}}}{5a^2}-\frac{2(ax+b)^{\frac{3}{2}}}{3a^2}$$
## Integration by parts
\
$$\frac{d}{dx}(uv) = u\frac{dv}{dx}+v\frac{du}{dx}$$
$$u\frac{dv}{dx}=\frac{d}{dx}(uv)-v\frac{du}{dx}$$
$$\int u\frac{dv}{dx}dx=\int\frac{d}{dx}(uv)dx-\int v\frac{du}{dx}dx$$
$$\int u\frac{dv}{dx}dx=uv-\int v\frac{du}{dx}dx$$
#### Example:
$$I = \int xcos(x)dx$$
Let: $$u=x$$ so: $$\frac{du}{dx} = 1$$
Let: $$\frac{dv}{dx} = cos(x)$$ so: $$v = sin(x)$$
\
Using the formula for integration by parts: $$\int xcos(x)dx = xsin(x) - \int 1sin(x)dx$$
Integrating the right side gives: $$\int xcos(x)dx = xsin(x)+cos(x)+c$$
#### Remember LATE when choosing what part should be $u$:
- ##### L - logarithms
- ##### A - algebra
- ##### T - trigonometry
- ##### E - exponentials

## Partial Fractions

#### Example:
$$I = \int \frac{x-5}{(x+1)(x-2)}dx$$
\
$$\frac{x-5}{(x+1)(x-2)} = \frac{A}{x+1}+\frac{B}{x-2}$$
\
$$x-5 = A(x-2) + B(x+1)$$
Solving for $A$ and $B$ gives $A = 2$ and $B = -1$
So: $$I = \int\frac{x-5}{(x+1)(x-2)}dx$$
\
$$I=\int(\frac{2}{x+1}-\frac{1}{x-2})dx$$
\
$$I = 2ln|x+1|-ln|x-2|+c$$
\
$$I = ln|\frac{(x+1)^2}{x-2}|+c$$
## Trapezium Rule
\
If you cannot integrate a function algebraically, you can use a numerical method to approximate the area beneath the curve.

Consider the curve $y=f(x)$: 
![[Pasted image 20230903152603.png]]
To approximate the area given by $\int_{a}^bydx$ you can divide the area up into n equal strips. Each strip will be of width $h$ where $$h = \frac{b-a}{n}$$
$b$ and $a$ are the limits of the integral and $n$ is the number of trapeziums used to estimate the area.

Next you calculate the value of $y$ for each value of $x$ that forms a boundary of one of the strips. So you find $y$ for $x=a$, $x = a +h$, $x = a + 2h$, $x = a + 3h$ and so on until $x=b$. These values of y can be labelled $y_0, y_1, y_2, y_3,..., y_n$.

The trapezium rule is given by the equation: $$\int_{a}^bydx \approx \frac{1}{2}h(y_0+2(y_1+y_2...+y_{n-1})+y_n)$$
where: $$h =\frac{b-a}{n}$$
and $$y_i=f(a+ih)$$

#### Example:
The diagram shows a sketch of the curve $y=sec(x)$. The finite region $R$ is bounded by the curve, the $x$-axis, and the $y$-axis and the line $x=\frac{π}{3}$

![[Pasted image 20230903164725.png]]

| $x$ | 0 | $\frac{π}{12}$ | $\frac{π}{6}$ | $\frac{π}{4}$ | $\frac{π}{3}$ |
| - | - | :-: | - | -  | - | 
| $y$ | 1 | 1.035 | | | 2|

- a) Complete the table with the values of $y$ corresponding to $x = \frac{π}{6}$ and $x = \frac{π}{4}$, giving your answers to 3 decimal places.
	- $sec(\frac{π}{6}) = \frac{1}{cos(\frac{π}{6})} = 1.155$
	- $sec(\frac{π}{4}) = \frac{1}{cos(\frac{π}{4})} = 1.414$

| $x$ | 0 | $\frac{π}{12}$ | $\frac{π}{6}$ | $\frac{π}{4}$ | $\frac{π}{3}$ |
| - | - | :-: | :-: | :-:  | - | 
| $y$ | 1 | 1.035 |1.155 | 1.414 | 2|

- b) Use the trapezium rule, with all the values of $y$ in the completed table, to obtain an estimate for the area of $R$, giving your answer to 2 decimal places.
	$$I = \int_a^bydx \approx \frac{1}{2}h(y_0+2(y_1+y_2...+y_{n-1})+y_n)$$
	$$I \approx \frac{1}{2}(\frac{π}{12})(1+2(1.035+1.155+1.414)+2)$$
	$$I \approx \frac{π}{24} \times 10.208$$
	$$I \approx 1.34$$
- c) Explain the reason whether your estimate in part **b** will be an underestimate or an overestimate.
	- It would be an overestimate as the graph is convex so the lines connecting the endpoints of each trapezium would be above the curve, giving a greater answer than the real answer