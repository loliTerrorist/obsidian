#math #Computational_mathematics 
This chapter will extend on the root-finding and error analysis concepts from [[Chapter 1 Solving nonlinear equations]] into multidimensional system in $\mathbb{R}^n$ or $\mathbb{C}^n$.

We first review some concepts in linear algebra: 
- Coordinates
- Norms
- Operator norms
- Invertibility

We move on to solving linear systems, primarily through [[LU factorization]], and show that solving $Ax = b$ with LU factorization costs less steps compared to explicit matrix inverse, hence reducing error. We use the [[condition number]] to study how data perturbations affect solutions of $Ax = b$; This allow us to analyze how much precision is loss by [[rounding]]. We also show that small or zero pivots cause catastrophic loss of precision or algorithm failure, hence introducing [[partial pivoting]]. 

The eigenvalues of a matrix $A$ decide the behavior of the iteration $x \mapsto Ax$  and, in the
chapter on differential equations, the stability of equilibria. We present three tools: the
[[power method]], which finds the eigenvalue of largest modulus, [[inverse iteration]], which
finds the eigenvalue closest to a given number, and [[Gershgorin’s discs]], which locate all
the eigenvalues at once [7, 10]. Even for a real matrix the eigenvalues may be complex,
so we take $\mathbb{K} = \mathbb{C}$ throughout: $A ∈ Mat_{n×n}(\mathbb{C})$, real matrices being included.

Finally we move on to nonlinear systems and computer-assisted proofs in $\mathbb{R}^n$. We introduce [[Newton's method]] and [[radii polynomial theorem]] in $\mathbb{R}^n$.

We conclude the chapter with some examples:
[[Intersection of two curves]]

 