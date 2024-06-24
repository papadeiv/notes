# Reaction-diffusion system
[Link](https://en.wikipedia.org/wiki/Reaction%E2%80%93diffusion_system#)

It is a type of [high-dimensional dynamical system](HighDimensionalSystem.md) modelling an unsteady physical phenomena with the absence of advection/convection/transport.

The general equation for a scalar field $u(\boldsymbol{x},t)$ reads

$\partial_t u = \mathcal{D}u + f(u;\mu)$

where $\mathcal{D}$ is a differential operator modelling diffusion and $f(u;\mu)$ is a (parametric) non-linear forcing term modelling reaction.

## Second-order diffusion (Laplacian operator)

We categorise some examples of the form $\mathcal{D}u=\sigma\Delta u$ .

In $1$ spatial dimension the equation is known as the [Kolmogorov-Petrovsky-Piskunov](KPPequation.md) (KPP) equation. Notable cases are given:
* if $f(u;\mu)=0$ then the system reduces to the heat equation whose steady state $u^{* }(\boldsymbol{x})$ is a solution of the Laplace's equation;
* if $f(u;\mu)=u(1-u)$ the equation is known as [Fisher-KPP](F-KPPequation.md) (F-KPP) equation;
* the generalisation $f(u;\mu)=u(1-u^p)$ where $p\geq2$ is known as the [Newell–Whitehead-Segel](NWSequation.md) (NWS) equation; 
* if $f(u)=-\varepsilon^{-2}\phi(u)$ where $\phi(u):=\Phi^{'}(u)$ is the derivative of a (non-negative) potential $\Phi(x)$ the equation is known as [Allen-Cahn](ACequation.md) (AC) equation;
* if $\boldsymbol{f}(\boldsymbol{q};\boldsymbol{\mu})=[\mu u - u^3 -\lambda v, \epsilon^{-1}(u-v)]$ the equation is known as [FitzHugh-Nagumo](FHNequation.md) (FHN) equation;
* if $\mathcal{D}u = (1+i\alpha)\Delta u$ and $f(u;\mu)=u(1-(1+i\beta)|u|^2)$ the equation is known as the [Ginzburg-Landau](GLequation.md) (GL) equation.

## Higher-order diffusion (Biharmonic operator) 

In the following we define $\Delta^2 = \Delta(\Delta)$ to be the (fourth-order) biharmonic operator.

* If $\mathcal{D}u = -(1+\Delta)^2 u = -u -2\Delta u - \Delta^2 u$ and $f(u;\mu)=\mu u + N(u)$ , with $N(u)$ smooth and non-linear, the equation is known as the [Swift-Hohenberg](SHequation.md) (SH) equation;
* if $\mathcal{D}u = -\Delta u - Delta^2 u$ and $f(u)=-\frac{1}{2}|\nabla u|^2$ the equation is known as the [Kuramoto-Sivashinsky](KSequation.md) (KS) equation.

## Bifurcations 

Reaction-diffusion models undergo various bifurcations of steady-states:
* at (spatial) wave number $k=0$ the homogeneous stable steady-state undergoes a [Hopf](HopfBifurcation.md) bifurcation to a oscillating homogeneous solution;
* at finite wave number the homogeneous steady-state undergoes a [Turing](TuringBifurcation.md) bifurcation to a spatially-patterned steady-state.

In @KJZ4BD7S#Dhillon_Milinkovitch_Zwicker_2017 extensive bifurcation analysis of reaction-diffusion systems is carried in a surface-FEM (sFEM) framework.
