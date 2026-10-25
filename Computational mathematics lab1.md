#math #Computational_mathematics #homework
## Problem 1.
### (a)![[Pasted image 20261021214802.png]]
### (b) 
1756
### (c)
35
### (d)


## Problem 2. 
### (a)
![[Pasted image 20261021215043.png]]
It certifies 5 digits.
When written as `@exact F(x) = x^2-0.7`, the 0.7 is stored as a floating point approximation of 0.7, and thus we are enclosing that instead. In order to enclose $\sqrt{0.7}$  we may use `@exact F(x) = x^2 - interval(0.7)` instead.
### (b)
#### (i)
![[Pasted image 20261021222741.png]]
#### (ii)
The corollary states that $Z_2$ must satisfy $|A(f'(x)-f'(\bar{x}))| \le Z_2 |x-\bar{x}|$ , applying mean value theorem gives

$$
|A(f''(c)(x-\bar{x}))| \le Z_2|x-\bar{x}|
$$
for some $c \in \bar{B}(\bar{x}, r_*)$. Dividing both sides by $|x-\bar{x}|$ we see that 
$$
|A||f''(c)| \le Z_2
$$
and thus we choose $Z_2$ to be the supremum of $|A||f''(c)|$. Since $f''(x) = (x+2)e^x$ is strictly increasing, we may choose $|A||\bar{x}+r_{*}+2|e^{\bar{x}+r_*}$ as an upperbound.  
![[Pasted image 20261021222715.png]]
#### (iii)
## Problem 3.
### (a)

### (b)
### (c)
### (d)
