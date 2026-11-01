#math 
## Motivation
### A zero pivot
$A = \begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix}$ encounters a zero pivot at the first row, stopping Gaussian elimination instantly.
### A small pivot
Let $\mu = 10^{-20}$ and 
$$
A = \begin{pmatrix} \mu & 1 \\ 1 & 1\end{pmatrix},\; 
b = \begin{pmatrix} 1 \\ 2 \end{pmatrix},\; x = \frac{1}{1-\mu}\begin{pmatrix}1 \\ 1-2\mu \end{pmatrix} \approx \begin{pmatrix}1 \\ 1\end{pmatrix}

$$
Note that the system is rather well conditioned; $\kappa_1(A) = 2 \times \frac{2}{1-\mu} \approx 4$.
However, gaussian elimination gives 
$$
\ell_{21} = \frac{A_{2,1}}{A_{1,1}} = 10^{20}, \qquad U_{2,2} = A_{2,2} - \ell_{21} A_{1,2} = 1 - 10^{-20},
\qquad fl(1-10^{-20}) = -10^{-20}
$$
and ends up factorizing $A$ into 
$$
\begin{pmatrix}1 & 0 \\ 10^{20} & 1\end{pmatrix} \begin{pmatrix}\mu & 1 \\ 0 & -10^{-20}\end{pmatrix}
= \begin{pmatrix}\mu & 1 \\ 1 & 0\end{pmatrix} \ne A
$$
## The solution
We would like to rearrange the rows to avoid a zero pivot or a small pivot. Hence at each step we can look for a pivot with the largest absolute value that is available.
This is accomplished by exchanging rows, hence a left multiplication by a permutation matrix. Since we are only permuting rows this is called **partial pivoting**, whereas also exchanging the columns gives **complete pivoting**.


