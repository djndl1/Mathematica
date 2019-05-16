## Common Distributions

### Discrete distributions

#### [Bernoulli distribution](https://en.wikipedia.org/wiki/Bernoulli_distribution)

The probability distribution of any single experiment that asks a yes-no question, a special case of the _binomial distribution_ where a single trial is conducted. Also a special case of the _two-point distribution_.

PMF: 

$$
f\left(k;p\right)=p^{k}\left(1-p\right)^{1-k} \quad\text{for } k\in \left\{0,1\right\}
$$

#### [Categorical distribution](https://en.wikipedia.org/wiki/Categorical_distribution) Generalized Bernoulli distribution, multinoulli distribution

It describes the possible results of a random variable that can take on one of $K$ possible categories, with the probability of each category separately specified.

PMF:

Let $\boldsymbol{p} = \left(p_1, \dots , p_k \right)$ and $\sum_{i=1}^k p_i = 1$

$$
f\left(x|\boldsymbol{p}\right)=\prod_{i=1}^{k}p_{i}^{\left[x=i\right]}
$$

where $\left[x=i\right]$ evaluates to $1$ if $x=i$, $0$ otherwise. See [Iverson bracket](https://en.wikipedia.org/wiki/Iverson_bracket) and [Kronecker delta](https://en.wikipedia.org/wiki/Kronecker_delta).

e.g. the roll of a die

#### [Binomial distribution](https://en.wikipedia.org/wiki/Binomial_distribution)

A sequence of $n$ independent experiments, each asking a yes-no question, or the probability of $k$ successes in $n$ draws with [replacement](https://math.stackexchange.com/questions/2685714/without-replacement-hypergeometric-with-replacement-binomial)([put back](http://www.maths.qmul.ac.uk/~rab/ProbI/notes2.pdf)).

#### [Multinomial distribution](https://en.wikipedia.org/wiki/Multinomial_distribution)

A generalization of the binomial distribution

$$
f\left(x_{1},\dots,x_{k};n,p_{1},\dots,p_{k}\right)=\frac{n!}{x_{1}!\dotsb x_{k}!}p_{1}^{x_{1}}\dotsb p_{k}^{x_{k}}
$$

where $\sum_{i=1}^k x_i = n$ for non-negative integers $x_1, \dots , x_k$.

#### [Geometric distribution](https://en.wikipedia.org/wiki/Geometric_distribution)

- The probability distribution of the number $X$ of Bernoulli trials needed to get one success

- The probability distribution of the number $Y=X-1$ of the failures before the first success

$$
\Pr\left(X=k\right)=\left(1-p\right)^{k-1}p\quad \text{for } k=1,2,3,\dots
$$

or 

$$
\Pr\left(X=k\right)=\left(1-p\right)^{k}p\quad \text{for } k=0,1,2,3,\dots
$$

#### [Hypergeometric distribution](https://en.wikipedia.org/wiki/Hypergeometric_distribution)

It describes the probability of $k$ successes in $n$ draws without replacement

$$
{\displaystyle p_{X}(k)=\Pr(X=k)={\frac {{\binom {K}{k}}{\binom {N-K}{n-k}}}{\binom {N}{n}}},}
$$

#### [Poisson distribution](https://en.wikipedia.org/wiki/Poisson_distribution)

The probability of a given number of events occurring in a fixed interval of time or space if these events occur with a known constant rate and independently of the time since the last event.

$$
f\left(k;\lambda\right)=\Pr\left(X=k\right)=\frac{\lambda^{k}e^{-\lambda}}{k!}
$$

Remark: $\lambda$ is the average number of occurrences in a given interval.

### Continuous distribution

#### Uniform distribution $U\left(a,b\right)$

$U\left(0,1 \right)$ is called __standard uniform distribution__.

#### Log-Logistic distribution


