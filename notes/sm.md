## Gaussian Sampling
Sampling $$x$$ from $$N(\mu,\sigma^{2})$$ is calculated as:

$$
\begin{align*}
x\sim N(\mu,\sigma^{2}) \\
x = \mu + \sigma. \epsilon \\
\epsilon \sim N(0,1)
\end{align*}
$$

This is because:

Mean of $Y$ is:

$$
E(Y)=E(aX) = a.E(X)
$$

Whereas, Variance of $Y$ is:

$$
Var(Y) = a^{2}.Var(X)
$$

Why?

The variance of a random variable $X$ is:

$$ 
Var(X) = E(X-E(X))^{2} 
$$


Suppose we define a new variable by scaling $X$:

$$
Y = aX
$$

Then the variance of $Y$ is:

$$
\begin{align*}
Var(Y) &= Var(aX) \\        
&= E(aX-E(aX))^{2} \\        
&= E(a^{2}.E(X-E(X))^{2} \\         
&= a^{2}.E(X-E(X))^{2} \\         
&= a^{2}.Var(X)
\end{align*}
$$


