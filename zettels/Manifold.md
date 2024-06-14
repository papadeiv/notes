# Manifold
For a [dynamical system](ContinuousTimeSystem.md) it is an [invariant set](InvariantSet.md) associated to an [equilibria](Equilibrium.md). It is an important object that affects the local and global behaviour of trajectories in phase space.

They are associated to the eigenspaces of the Jacobian of the system evaluated at the equilibria.

They are indicated as $W^{(u,s,c)}(x_0)$ where $x_0$ is usually not the origin of the phase space.
In such case one has to find an [homeomorphism](Homeomorphism.md) $x = h(y)$ that maps orbits of $\dot{x}=f(x)$ close to $x_0$ to orbits of the linearised system $\dot{y}=D_{f}(y=0)y$ close to $0$ as per the [Hartman-Grobman theorem](HartmanGrobmaTheorem.md).

In order to compute a manifold one must use the __Stable manifold theorem__:
- linearise the system $\dot{x}=f(x)$ around its equilibrium $x_0$, i.e. computing $\dot{x}\approx D_{f}(x=x_0)x$;
- build the eigenspace $E$ of each eigenvalue $\lambda$:
  - if $\mathfrak{Re}(\lambda)<0$ the eigenspace $E^s$ is stable and flowing into $x_0$;
  - if $\mathfrak{Re}(\lambda)>0$ the eigenspace $E^u$ is unstable and flowing out of $x_0$;
  - if $\mathfrak{Re}(\lambda)=0$ the eigenspace $E^c$ is a [centre manifold](CentreManifold.md) and its dynamics has to be solved approximately; 
- the manifold $W$ has the same dimension and is locally tangent to $E$ close to $x_0$.

For planar systems (i.e. in $2D$) we have: 
  > $\det(D_f(x_0))=\lambda_1\lambda_2$  and $\text{tr}(D_f(x_0))=\lambda_1+\lambda_2$  meaning that:
  >   - $\det(D_f(x_0))>0$ and $\text{tr}(D_f(x_0))>0$ then $x_0$ is a repeller and it has a $2-$ dimensional unstable manifold $W^{(u)}(x_0)$;
  >   - $\det(D_f(x_0))>0$ and $\text{tr}(D_f(x_0))<0$ then $x_0$ is an attractor and it has a $2-$ dimensional stable manifold $W^{(s)}(x_0)$;
  >   - $\det(D_f(x_0))<0$ then $x_0$ is a saddle and it has a $1-$ dimensional unstable manifold $W^{(u)}(x_0)$ and a $1-$ dimensional stable manifold $W^{(s)}(x_0)$;
  >   - $\det(D_f(x_0))>0$ and $\text{tr}(D_f(x_0))=0$ then $x_0$ is a centre and it has a $2-$ dimensional centre manifold $W^{(c)}(x_0)$;
  >   - $\det(D_f(x_0))=0$ then $x_0$ is non-hyperbolic and it has a $1-$ or $2-$ dimensional centre manifold $W^{(c)}(x_0)$.

Saddle-like equilibria may form heteroclinic and homoclinic connections through their manifolds and in particular the former connects $2$ distinct saddles (or a saddle with a source or a sink) while the latter connects a saddle to it-self through a loop. 

## Examples
* ??
  > ??

* ??
  > ??
