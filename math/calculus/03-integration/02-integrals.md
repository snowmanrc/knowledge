# Integrals

## Deriving from Summation

As it is know, the estimated area under the graph, using the summation notation, can be expressed as:
$$A = \Delta x \cdot \sum_{k=1}^{n} f(c_k) $$
As these intervals can be of different widths, the above formula can be more accurately written as:
$$A = \sum_{k=1}^{n} \Delta x_k \cdot f(c_k) $$
Now, assume that we can change the number of intervals. As we know, more intervals -> more closer to actual area. Applying limit,
$$A = \lim_{n \to \infty} \sum_{k=1}^{n} \Delta x_k \cdot f(c_k)$$
The above formula basically tells us what the area approaches as the number of intervals of the estimated sum reach infinity.
*As the intervals get smaller and smaller, the rectangles more precisely fit the shape of the graph and their overall sum appraoches to the actual area of the graph.*

This is basically the definite integral.

![Estimation turns into reality](https://www.youtube.com/watch?v=WUvTyaaNkzM)

## Definite Integral

The general form of the definite integral is:
$$\int_{a}^{b} f(x) dx$$
This calculates the area of the graph from $a$ to $b$. To calculate the definite integral, however, one must find the function whose dervative gives $f(x)$, or basically find the indefinite integral of $f(x)$.

## As Anti-Derivative

Integration, in essence, is the reverse operation of differentiation. 
+ If $f$ is obtained by integrating $g$, then $g$ is obtained by differentiating $f$. 
+ $g$ is the derivative of $f$ while $f$ is the anti-derivative of $g$.

## Finding Integrals

1. Anti-derivative Formulas
    1. Power
    2. Logarithmic and Exponents
    3. Trignometric
2. U-Substitution
    1. Simple U substitution
    2. Subsitution formula (change of integral limits)
3. Integration by Parts
4. Trignometric Function Substitution
5. Partial fraction decomposition

Remember using the model: `FUPTPF` -> Formulas, U, Parts, Trig, Partial Fractions