#math #Computational_mathematics 
The main questions tackled in this chapter are:
1. How do we compute an approximate solution?
2. What do the rounding errors of the computer do to the result?
3. Can we prove that a mathematically exact solution exists?

The methods we used all use a sequence meant to converge to $\check{x}$. We uses the [[order and rate of a sequence]] to measure how quickly the sequence converges. This matters because errors propagate along steps, so the more steps we take the more error we make.

We introduce the following algorithms to find roots: ^18ad89
- [[Bisection]]
- [[Fixed point iteration]]
- [[Newton's method]]
- [[Secant method]]

In order to understand where errors come from, we need to look at how computers stores real numbers: It stores an [[rounding|approximation]] of the number in [[double precision number]]. Since there is approximation we can study [[propagation of errors|how much error is made]]. 

We can provide instead a bound on the calculations we make, and then ensure that the answer we want lies in such a region. For this we introduce [[interval arithmetic]].

Finally we use [[interval arithmetic]] to show how good the solutions provided by [[^18ad89| the algorithms introduced above]] is.

We introduce [[radii polynomial theorem]].

Applying the [[radii polynomial theorem|theorem]] boils down to the following steps:
1. Compute an approximation $\bar{x}$.
2. Formulate the zero finding problem $f$ and obtain $f'$.
3. Construct  the approximate inverse $A \approx 1/f'(x)$.
4. Choose $r_*$ and estimate the bounds $Y, Z_1, Z_2$ in interval arithmetic.
5. Check if the hypotheses holds.

Examples: 
[[Square root of 2 (first order form)]]
[[Cube root of 2 (second order form)]]




