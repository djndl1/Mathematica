## Moment

In mathematics, a _moment_ is a specifific quantitative measure of the shape of a function, used in both mechanics and statistics.

The $n$-th moment of a real-valued continuous function $f(x)$ of a real variable about a value $c$ is 
$$
\mu_{n}=\int_{-\infty}^{\infty}\left(x-c\right)^{n}f\left(x\right)dx
$$

The moment about zero of a PDF $f(x)$ is called a _raw/crude moment_. The moments aobut its mean are called _central moments_; these decribe the shape of the function, independently of translation.

### [Central moments](https://en.wikipedia.org/wiki/Central_moment)

A moment of a probability distribution of a random variable about the random variable's mean.

The $n$-th central moment is translation-invariant, [homogeneous](https://en.wikipedia.org/wiki/Homogeneous_function) of degree $n$.

### Important moments

#### [Expected Value/expectation](https://en.wikipedia.org/wiki/Expected_value) the first raw moment

Read the properties.

Note that
$E\left[X\right]$ exists and is finite iff $E\left[\left|X\right|\right]$ is finite.

#### [Variance](https://en.wikipedia.org/wiki/Variance) the second central moment and its positive square root (the standard deviation)

Variance is invariant w.r.t in changes in a location parameter.

$\text{Var}\left(\sum_{i=1}^{n}X_{i}\right)=\sum_{i=1}^{n}\text{Var}\left(X_{i}\right)$ for uncorrelated random variables.

$\text{Var}(c^T X) = c^T \Sigma c$ for a column vector of $n$ random variables $X$.

See [Variance for Matrix/scalar random variables](https://en.wikipedia.org/wiki/Variance#Generalizations)


[deviation](https://en.wikipedia.org/wiki/Deviation_(statistics)): a measure of difference between the observed value of a variable and some other value, often the variable's mean. The difference between the height of each man in the sample and the unobservable population mean is a statistical error, whereas the difference between the height of each man in the sample and the observable sample mean is a residual.

#### Skewness

#### Kurtosis


### Normalized moments

The normalized $n$-th central moment or standardized moment is the $n$-th central moment divided by $simga^n$
