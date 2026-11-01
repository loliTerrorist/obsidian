#algorithm #math #Computational_mathematics 
Bisection depends on the [[Intermediate Value Theorem]].
> [!theorem] Let $f:[a,b] \to \mathbb{R}$ be continuous with $f(a)f(b) \le 0$. Set $a_0 = a$, $b_0 = b$, and for $n \ge 0$ let $m_n = (a_n+b_n)/2$ and $[a_{n+1}, b_{n+1}] = [a_n, m_n]$ if $f(a_n)f(m_n) \le 0$ and $= [m_n, b_n]$ otherwise. Then $f(a_n)f(b_n) \le 0$ for all $n$, the sequence $(a_n), (b_n)$ converges to a common limit $\check{x} \in [a,b]$, $f(\check{x}) = 0$ and 
> $$
> |m_n-\check{x}| \le \frac{b-a}{2^{n+1}}
> $$

Translation: On each iteration split the interval in half and keep the interval that contains the root. A bound on how far the midpoint to the root is provided.

> [!proof]
> First we show that $f(a_n)f(b_n) \le 0$ for all $n$. 
> If $f(a_n)f(m_n) \le 0$ then $f(a_{n+1}), f(b_{n+1})$ are of different sign. The other case also holds, and by induction we completed the proof.
> #TODO

- Order and rate: The definition doesn't apply as the limit doesn't exist. Since 
  $|b-a|/2^{n+1}$ is halved at every step, we say that it converges linearly with a rate of $\frac{1}{2}$. 
- Digits: 
- Cost: 1 evaluation of $f$ per step.
- A priori bound: 
- Several roots in $[a,b]$: Finds one of them.