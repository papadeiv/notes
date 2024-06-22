# Steady-state or stationary solution

For an [inifite-dimensional dynamical system](HighDimensionalSystem.md) defined by a spatio-temporal PDE it is the equivalent of an equilibrium solution for a [finite-dimensional dynamical system](ContinuousTimeSystem.md) defined by a system of ODEs.

They are thus described as time-independent functions $u(x,t)=u^{ * }(x)$ defined on a Banach space $V$ s.t. it sets the LHS of the system  $\partial_t u = f(\mathcal{L}(u),u) + g(u)$ to 0.
They are implicitly defined, same as low-dimensional systems, however, instead of being solutions of an algebraic problem, steady-states are solutions of a non-linear (partial) differential equation in space.

$u^{*}(x)\in V \quad \text{s.t.}\quad f(\mathcal{L}(u),u) = -g(u)$$

Typical stationary solutions are:
* __homogeneous states__;
* __standing waves__;
* __unsteady waves__ travelling at constant speed $c$ that are stationary in the moving coordinate frame $\xi=x-ct$;
* __solitons__ or __solitary waves__;
* __coherent structures__ or __patterns__.

## Stability

Roughly speaking, stability for a stationary solution of a high-dimensional systems means that, if the IC $u(x,0)$ starts near $u^{ * }(x)$ then it will converge to such steady-state forward in time.
Linearization of a non-linear PDE of the general form above around the steady-state yields

$\partial_t u(x,t)\approx D_{F}(u^{ * }(x))u(x,t) =: \mathcal{L}^{ * }u(x,t)$

In the analysis of the [stability](https://en.wikipedia.org/wiki/Stability_theory) of high-dimensional systems it is important the evaluation of the [spectrum](https://math.stackexchange.com/questions/2117107/spectrum-of-the-derivative-operator) of the linear operator $\mathcal{L}^{ * }$ acting on the Banach space $V$ w.r.t. the 0 steady-state.

In particular the stationary solution $u(x,t)=0$ is said to be stable if $\forall\varepsilon>0$ , $\exists\delta(\varepsilon)>0$ s.t. $\forall u(x,0)=:u_0(x)\in V$ with $ ||u_0(x)||_{V}\leq\delta(\varepsilon)$ then $ ||u(x,t)||_{V}\leq\varepsilon$ , $\forall t>0$.
