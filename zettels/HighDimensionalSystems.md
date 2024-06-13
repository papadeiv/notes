# High-dimensional dynamical systems

It is the generalization of [continuous-time dynamical systems](ContinuousDynamicalSystems.md) to infinite dimensional variables, i.e. instead of a finite dimensional vector variable, whose temporal evolution is described through a set of ordinary differential equations

$\dot{\boldsymbol{x}}=f(\boldsymbol{x};\boldsymbol{\mu}),\quad\boldsymbol{x}\in\mathbb{R}^n$

these systems describe the time dynamics of scalar and vector fields defined over a spatial domain

$\partial_t \boldsymbol{u} = \boldsymbol{f}(\mathcal{L}(\boldsymbol{u}),\boldsymbol{u}) + \boldsymbol{g}(\boldsymbol{u})$

where $\mathcal{L}$ represents a (differential) spatial linear operator while $\boldsymbol{f}(\boldsymbol{u})$ and $\boldsymbol{g}(\boldsymbol{u})$ are (in general) non-linear functions of the unknown.

In the analysis of the [stability](https://en.wikipedia.org/wiki/Stability_theory) of high-dimensional systems it is important the evaluation of the [spectrum](https://math.stackexchange.com/questions/2117107/spectrum-of-the-derivative-operator) of the linear operator $\mathcal{L}$.
