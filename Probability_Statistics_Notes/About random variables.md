#### Random variables
The formal definition and related properties as well as proofs are not presented here, refer to [The definition of random variables](https://en.wikipedia.org/wiki/Random_variable#Definition)

---

  Several important facts must be kept in mind:

1. A random variable $X:\Omega\mapsto E$ is a measurable function from a set of possible __outcomes__ to a __measurable space__. It is a function dependent on samples.

2. A random variables's possible values conceptually represent either the results of an __"objectively" random process__ (such as rolling a die), or the "subjective" randomness that results from __incomplete knowledge__of a quantity. The meaning of the probabilities assigned to the potential values of a random variable is not part of probability theory itself but instead related to philosophical arguments over the [interpretation of probability](https://plato.stanford.edu/entries/probability-interpret/). The mathematics works the same regardless of the particular interpretation in use.

3. The discrete counterpart of probability density function of a random variable is the _probability mass function_. It is often the primary means of defining a discrete probability distribution and can be seen as a special case of the distribution and the probability density function w.r.t. the [counting measure](https://en.wikipedia.org/wiki/Counting_measure). See [here](https://en.wikipedia.org/wiki/Probability_mass_function#Measure_theoretic_formulation) for more details.

4. The generalization of _random variable_, with a more broad measurable space image $E$ is a [_random element_](https://en.wikipedia.org/wiki/Random_element), frequently assumed a topological vector space. The narrow concept _random variable_ is more used as with values in $R$. Do note that random process a one of the case of _random element_.

5. The distribution of a random variable is defined on the sample space $\Omega$. The notation $P(X=2)$ is actually just a shorthand of $P\{\omega\colon X(\omega)=2\}$, although in practice the underlying probability space $\Omega$ is completely disposed, only as a technical device to guarantee the existence of random variables. In fact, one can just works with probability distribution
s instead of random variables, see [quantile function](https://en.wikipedia.org/wiki/Quantile_function).

6. The most formal, axiomatic definition of a random variable involves measure theory.

7. The probability distribution of a random variable is often [characterised](https://en.wikipedia.org/wiki/Moment_problem) by a small number of parameters, which also have a practical interpretation, such as the first moment (expected value) or the variance and standard deviation. For non-real-valued random variables, moments can be taken of real-valued functions of those variables.

8. The determination of functions of random variables normally requires invertibility of the function. In the measure-theoretic, axiomatic approach to probability, if a random variable $X$ on $\Omega$  and a Borel measurable function $g\colon \mathbb {R} \rightarrow \mathbb {R}$ , then $Y=g(X)$ is also a random variable on  $\Omega$ , since the composition of measurable functions is also measurable. The same procedure that allowed one to go from a probability space $(\Omega ,P)$ to  $(\mathbb {R} ,dF_{X})$ can be used to obtain the distribution of $Y$.

9. The equivalence of random variables can be defined w.r.t. _equality in distribution_, _almost sure equality_ ($P(X\neq Y)=0$) or _equality in sample spaces_.

#### About probability distributions

The terminology of "distribution" is not uniform and can be confusing sometimes. Refer to [distribution terminology](https://en.wikipedia.org/wiki/Probability_distribution#Terminology). Do remember _mode_, _support_, _head_, _tail_ and _skewness_.

A discrete probability distribution is often represented as a generalized probability density function involving Dirac delta functions, which substantially unifies the treatment of continuous and discrete distributions.

[0-1 indicator function](https://en.wikipedia.org/wiki/Indicator_function)

##### Cumulative distribution function (CDF)

Do lay emphasis on continuity of CDF

##### [Quantile](https://en.wikipedia.org/wiki/Quantile) function (inverse cumulative distribution function)

W.r.t a continuous and strictly monotonic distribution function. Suppose a CDF $F_{X}\colon R\mapsto\left[0,1\right]$, the corresponding quantile function is $Q\left(p\right)=\inf\left\{ x\in\mathbb{R}\colon p\leq F\left(x\right)\right\}$

##### Probability density function (PDF)

The terms "probability distribution function" and "probability function" have sometimes been used to denote the probability density function. Not every probability distribution has a density function: the distributions of discrete random variables do not; nor does the Cantor distribution, even though it has no discrete component, i.e., does not assign positive probability to any individual point.

The probability density function of the sum of two independent random variables U and V, each of which has a probability density function, is the convolution of their separate density functions.

##### joint probability distribution

The joint probabilit distribution for $`X,Y,\dots`$ is a probability distribution that gives the probability that each $`X,Y,\dots`$ falls in any particular range or discrete set of values specified for that variable.

For $`N`$ random variables $`X_1, \dots, X_n`$, the joint CDF is given by

```math
F_{X_{1},\dots,X_{N}}\left(x_{1},\dots,x_{n}\right)=P\left(X_{1}\leq x_{1},\dots,X_{n}\leq x_{n}\right)
```

The joint probability density function ${\displaystyle f_{X,Y}(x,y)} f_{{X,Y}}(x,y)$ for two continuous random variables is defined as the derivative of the joint cumulative distribution function.

