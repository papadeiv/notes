# Reaction-diffusion system

It is a type of [high-dimensional dynamical system](HighDimensionalSystem.md) modelling an unsteady physical phenomena with the absence of advection/convection/transport.

The general equation for a scalar field $u(\boldsymbol{x},t)$ reads

$\partial_t u = \sigma\Delta u + f(u;\mu)$

where $f(u;\mu)$ is a (parametric) non-linear forcing term modelling reaction.

In $1$ spatial dimension the equation is known as the Kolmogorov-Petrovsky-Piskunov (KPP) equation. Notable cases are given:
* if $f(u;\mu)=0$ then the system reduces to the heat equation whose steady state $u^{* }(\boldsymbol{x})$ is a solution of the Laplace's equation;
* if $f(u;\mu)=u(1-u)$ the equation is known as [Fisher-KPP](https://en.wikipedia.org/wiki/KPP%E2%80%93Fisher_equation) and it describes travelling wavefront solutions connecting two (homogeneous) steady states;
* if $f(u;\mu)=u(1-u^2)$ the equation is known as Newell–Whitehead-Segel (NWS) and it describes [Rayleigh-Benard instability](https://en.wikipedia.org/wiki/Rayleigh%E2%80%93B%C3%A9nard_convection).

For $2-$ dimensional vector unknown $\boldsymbol{q}(x,t)=[u(x,t),v(x,t)]$ special cases are:
* if $\boldsymbol{f}(\boldsymbol{q};\boldsymbol{\mu})=[\mu u - u^3 -\lambda v, \epsilon^{-1}(u-v)]$ the equation is known as [FitzHugh-Nagumo](https://en.wikipedia.org/wiki/FitzHugh%E2%80%93Nagumo_model) (FHN) and it describes activatpr-inhibitor systems in which one component produces the growth of both $u$ and $v$ while the other inhibits their growth. 

[TBC](https://en.wikipedia.org/wiki/Reaction%E2%80%93diffusion_system)
