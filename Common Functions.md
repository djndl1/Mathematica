# Common Functions

## Sigmoid function

A characteristic "S" shaped curve or sigmoid curve. A sigmoid function is a _bounded_, _differentiable_, _real_ function that is defined for all real input values and has a non-negative derivative at each point. In general it is _monotonic_ and has a first _bell-shaped_ derivative, _convex_ for values less than $0$, _concave_ for values more than $0$.

### Examples

#### Logistic function

Generally

$$
f\left(x\right)=\frac{L}{1+e^{-k\left(x-x_{0}\right)}}
$$

where $L$ is the maximum value and $k$ is the logistic growth rate or steepness of the curve.

$$
f\left(x\right)=\frac{1}{1+e^{-x}} = =\frac{1}{2}+\frac{1}{2}\tanh\left(\frac{x}{2}\right)
$$

It has a symmetry property that

$$
1-f\left(x\right)=f\left(-x\right)
$$

and an easily calculated derivative

$$
f'\left(x\right) = f\left(x\right)\left(1-f\left(x\right)\right)
$$

```python
f(x) = 1/(1+e^(-x))
show(f)
left_inf_lim = limit(f, x=-oo)
right_inf_lim = limit(f, x=oo)
logis_plot = plot(f, (x, -5, 5))
logis_plot + plot(left_inf_lim, (-5, 5), linestyle='--', color='gray') + plot(right_inf_lim, (-5,5), linestyle='--', color='gray')
```

#### [Hyperbolic](https://en.wikipedia.org/wiki/Hyperbolic_function) tangent (shifted and scaled version of the logistic function)

$$
f\left(x\right)=\tanh x=\frac{e^{x}-e^{-x}}{e^{e}+e^{-x}}
$$

```python
f(x) = (e^x - e^(-x))/(e^x + e^(-x))
left_inf_lim = limit(f, x=-oo)
right_inf_lim = limit(f, x=oo)
tanh_plot = plot(f, (x, -5, 5))
tanh_plot + plot(left_inf_lim, (-5, 5), linestyle='--', color='gray') + plot(right_inf_lim, (-5,5), linestyle='--', color='gray')
```

#### Arctangent function

$$
f\left(x\right)=\arctan x
$$

## Beta function

$$
{\displaystyle \mathrm {B} (x,y)=\int _{0}^{1}t^{x-1}(1-t)^{y-1}\,dt}
$$

for $Re\ x > 0, Re\ y > 0$.

or written in terms of gamma function

$$
\mathrm{B}\left(x,y\right)=\frac{\Gamma\left(x\right)\Gamma\left(y\right)}{\Gamma\left(x+y\right)}
$$
## Gamma function

In mathematics, the gamma function (represented by Γ, the capital Greek alphabet letter gamma) is one commonly used extension of the factorial function to complex numbers.

For any positive integer $n$ 

$$
\Gamma\left(n\right)=\left(n-1\right)!
$$

For complex numbers with a positive real part:

$$
\Gamma\left(z\right)=\int_{0}^{\infty}x^{z-1}e^{-x}dx,\quad\text{Re}z>0
$$

