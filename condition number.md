#definition #math 
The **condition number** of an invertible matrix $A \in M_{n\times n}(\mathbb{K})$ with respect to an induced norm is
$$
\kappa(A) := \|A\|\|A^{-1}\|
$$
written $\kappa_1$ for the 1-norm; for a [[singular matrix]] we set $\kappa(A) = \infty$. 
## Motivation
> [!proposition]
> Let $A \in Mat_{n\times n}(\mathbb{K})$ be invertible, $b \ne 0$ and $x = A^{-1}b$.
> (i) If $(A+\delta A)(x+\delta x) = b$ then 
> $$
> \frac{\| \delta x\|}{\|x+\delta x\|} \le \|A^{-1}\|\|\delta A\| = \|A\|\|A^{-1}\| \frac{\|\delta A\|}{\|A\|}
>$$
>(ii) If $A(x + \delta x) = b+\delta b$ then 
>$$
>\frac{\|\delta x\|}{\|x\|} \le \|A\| \|A^{-1}\| \frac{\|\delta b \|}{\|b\|}
>$$

> [!proof]
> (i).
> Subtracting $Ax = b$ gives $A \delta x + \delta A(x+\delta x)= 0$, rearranging gives $\delta x = -A^{-1}\delta A (x+\delta x)$, whose norm is bounded by $\|A^{-1}\| \|\delta A\| \|x+\delta x\|$.
> (ii).
> #TODO 






## Properties
- Scale: $\kappa(A) \ge 1$ as $1 = \|I\| = \|AA^{-1}\| \le \|A\|\|A^{-1}\|$, and $\kappa(\alpha A) = \kappa(A)$ for any $\alpha \ne 0$.


Examples:
[[A nearly singular matrix condition number]]
[[Vandermonde matrices condition number]]

