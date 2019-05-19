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

The CDF is in the form of a log-logistic function

$$
F\left(x;\alpha,\beta\right)=\frac{1}{1+\left(x/\alpha\right)^{-\beta}}
$$

where $\alpha>0$ is a scale parameter and the median of the distribution and $\beta>0$ is a shape parameter and the distribution is unimodal when $\beta > 1$. 

#### Normal distribution

Often used in the natural and social sciences to represent real-valued random variables whose distributions are not known. Its importance derives mainly from central limit theorem. 

$$
f\left(x|\mu,\sigma^{2}\right)=\frac{1}{\sqrt{2\pi\sigma^{2}}}e^{-\frac{\left(x-\mu\right)^{2}}{2\sigma^{2}}}
$$

- $\mu$ is the mean

- $\sigma$ the standard deviation

- $\sigma^2$ the variance.

A random vector is said to be $k$-variate normally distributed if every linear combination of its $k$ components has a univariate normal distribution. A real random vector is called a standard normal random vector if all of its components are independent and each is a zero-mean unit-variance normally distributed random variable, i.e. if $X_n ~ \mathcal{N}\left(0,1\right)$ for all $n$.

$$
\mathrm{X}\sim\mathcal{N}\left(\mu,\Sigma\right)\iff\text{there exist }\mu\in\mathbb{R}^{k},\mathrm{A}\in\mathbb{R}^{k\times l}s.t.\ \mathrm{X=AZ}+\mu\ \text{for\ }Z_{n}\sim\mathcal{N}\left(0,1\right),\text{i.i.d}
$$

The covariance matrix $\Sigma = \mathcal{A}\mathcal{A}^T$.

The degenerate case is when the covariance matrix is singular, giving no density.

PDF

Non-degenerate case: the symmetric covariance matrix $\Sigma$ is positive definite.
$$
f_{\mathrm{X}}\left(x_{1},\dots,x_{k}\right)=\frac{\exp\left(-\frac{1}{2}\left(\mathrm{x-\mu}\right)^{T}\Sigma^{-1}\left(\mathrm{x-\mu}\right)\right)}{\sqrt{\left(2\pi\right)^{k}\left|\Sigma\right|}}
$$

The likelihood function is given by 

$$
\ln L=-\frac{1}{2}\left[\ln\left(\left|\Sigma\right|\right)+\left(\mathrm{x-\mu}\right)^{T}\Sigma^{-1}\left(\mathrm{x-\mu}\right)+k\ln\left(2\pi\right)\right]
$$

If a random vector has a multivariate normal distribution then any two or more of its components that are uncorrelated are independent.

#### Exponential distribution

Describes the time between events in a Poisson point process and is the continuous analog of the geometric distribution.

$$
f\left(x;\lambda\right)=\lambda e^{-\lambda x}H\left(x\right)
$$

where $H(x)$ is the Heaviside step function, $\lambda$ called the _rate parameter_.

The exponential distribution has an important property: memorylessness

$$
\Pr\left(T>s+t|T>s\right)=\Pr\left(T>t\right)\quad \forall s,t\geq 0
$$

For example, if an event has not occurred after 30 seconds, the conditional probability that occurrence will take at least 10 more seconds is equal to the unconditional probability of observing the event more than 10 seconds after the initial time.
