# Hill-Clohessy-Wiltshire Dynamics

The linearized relative dynamics between a chaser satellite and a target object in orbit can be described by the following set of equations:

![equation](http://latex.codecogs.com/gif.latex?\begin{align*}&space;\ddot{x}(t)&space;&=&space;2n&space;\cdot&space;\dot{y}(t)&space;&plus;&space;3n^2\cdot&space;x(t)&space;\\&space;\ddot{y}(t)&space;&=&space;-2n\cdot&space;\dot{x}(t)&space;\\&space;\ddot{z}(t)&space;&=&space;-n^2\cdot&space;z(t)&space;\end{align*})


Assumptions:
* Distance from target to chaser is much much smaller than the orbital radius, i.e.,
![equation](http://latex.codecogs.com/gif.latex?|\boldsymbol{\rho}(t)|&space;<<&space;|\boldsymbol{r}_{tgt}|&space;\Rightarrow&space;\boldsymbol{r}_{ch}&space;\approx&space;\boldsymbol{r}_{tgt})

* A first order approximation on the term ![equation](http://latex.codecogs.com/gif.latex?\left(&space;1&space;&plus;&space;\frac{2x}{r_{tgt}}&space;\right)^{-3/2}&space;\approx&space;1&space;-&space;\frac{3x}{r_{tgt}})

* Reduce to time invariant by assuming target orbit's eccentricity equal to zero.

## Discrete System Equations

This system 