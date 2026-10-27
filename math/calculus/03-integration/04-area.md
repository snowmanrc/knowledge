# Area

Integrals can be used to find the area under given curve. The area found is bounded between the curve and the x-axis.

> [!tip] GRAPH!
> Always graph the functions before calculating area for clarity.

## Area under a curve

1. Find integral of the curve.
2. Compute definite integral with the bounds given.

> [!info] Things to consider
> Some things to keep note of when finding the area under the graph:
> + Area cannot be negative. If a negative value is obtained at the end, take its absolute.
> + Area can also cancel out. In some cases, when both the graph and the interval is symmetric, the areas can actually cancel eachother out and give zero which is not correct.
>	1. For this, first find the points where $f(x) = 0$.
>	2. if any of those points lie in $[a, b]$, the graph *might* make a flip so just divide the intervals.
>	3. Take the absolute for negative areas and then add.
> + Flipping the upper and lower limits negates the area.
> + Area can also overlap both in the positive and negative quadrants. For this, just flip the axis.

## Area between curves

Given two functions $f$ and $g$ such that $f \ge g$ for an interval $[a, b]$, then the area between them is the definite integral of $h = f - g$.

> [!tip] Bounds $a$ and $b$
> These might not always be provided. Most of the time, they are the common points of the the two graphs.

> [!tip] Greater function
> $f$ might not always be greater than $g$ at all points. Check where one is greater by drawing graphs and also finding their common points.

## Average value of a function

Average value of a function over an interval be found. Just divide the definite integral by $1/(b-a)$
