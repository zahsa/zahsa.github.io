## Sampling
The variance of a random variable X is:

$$ 
Var(X) = E(X-E(X))^{2} 
$$


Suppose we define a new variable by scaling $X$:

$$
Y = aX
$$

Then the variance of $Y$ is:

$$
Var(Y) = Var(aX) \\        
= E(aX-E(aX))^{2} \\        
= E(a^{2}E(X-E(X))^{2} \\         
= a^{2}.E(X-E(X))^{2} \\         
= a^{2}.Var(X)
$$
