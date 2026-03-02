# The Core Problem
In flat space, straight lines are defined by constant velocity.
$$
\frac{d^{2}x^\mu}{d\tau^{2}} = 0
$$
However, this assumes
- Global Cartesian coordinates
- Constant basis vectors
- No curvature
In curved manifolds, we instead observe that
- Basis vectors vary from point to point
- Tangent spaces differ
- Ordinary derivatives break the covariance
We thus need a derivative that respects geometry.
# Failure of Ordinary Derivatives
Take a vector field $V^\mu(x)$. The ordinary derivative is thus,
$$
\partial_{\nu}V^\mu
$$
using the Einstein summation notation. 
Under a coordinate transform, this becomes
$$
x^\mu \to x^{\mu'}
$$
$$
\partial_{\nu}V^\mu \to \partial_{\nu'}V^{\mu'}
$$
$$
= \frac{\partial x^\alpha}{\partial x^{\nu'}} \frac{\partial x^{\mu'}}{\partial x^\beta}\partial_{\alpha}V^\beta + \frac{\partial^{2}x^{\mu'}}{\partial x^\alpha \partial x^\gamma} \frac{\partial x^\alpha}{\partial x^{\nu'}}V^\gamma
$$
and this second term ruins the transformation. The reason is that it differentiates the components, but it ignores the change in basis vectors. We must find a correction.
# The Covariant Derivative
We introduce a connection:
$$
\nabla_{\nu}V^\mu = \partial_{\nu}V^\mu + \Gamma^\mu_{\nu \rho}V^\rho
$$
That fulfills the conditions:
- Linearity
- Leibniz rule
- Reduces to partial derivative in flat space
The extra term fixes transformation behavior.
# How the Connection Transforms
Under a coordinate change,
$$
\Gamma^{\mu'}_{\nu' \rho'} = \frac{\partial x^{\mu'}}{\partial x^\alpha} \frac{\partial x^\beta}{\partial x^{\nu'}} \frac{\partial x^\gamma}{\partial x^{\rho'}} \Gamma^\alpha_{{\beta \gamma}} + \frac{\partial x^{\mu'}}{\partial x^\sigma} \frac{\partial^{2}x^\sigma}{\partial x^{\nu'}\partial x^{\rho'}}
$$
The second term is not a homogeneous term, which explains why $\Gamma$ is not a tensor. Though, it makes $\nabla V$ transform as one.
# Imposing Geometric Conditions
We want a unique connection, we can thus impose the following conditions.
- Metric compatibility
$$
\nabla_{\lambda} g_{\mu \nu}= 0
$$
- Torsion-free
$$
\Gamma^\mu_{\nu \rho} = \Gamma^\mu_{\rho \nu}
$$
These conditions uniquely determine the torsion-free, metric-compatible affine connection, the Levi-Civita connection.
# Full Derivation
Let's start with the metric compatibility condition,
$$
\nabla _{\lambda}g_{\mu \nu} = \partial_{\lambda}g_{\mu \nu} - \Gamma^\rho_{\lambda \mu}g_{\rho \nu} - \Gamma^\rho_{\lambda \nu}g_{\mu \rho} = 0
$$
We write two more equations by cyclic permutation:
$$
\nabla_{\mu}g_{\nu \lambda} = 0
$$
$$
\nabla_{\nu}g_{\lambda \mu} = 0
$$
Add the first two, then subtract the third to get,
$$
\Gamma^\mu_{\nu \rho} = \frac{1}{2}g^{\mu \sigma}(\partial_{\nu}g_{\rho \sigma} + \partial_{\rho}g_{\nu \sigma} - \partial_{\sigma}g_{\nu \rho})
$$
# Geodesics
Action $S$ is defined as,
$$
S = \int ds  = \int \sqrt{ g_{\mu \nu} \frac{dx^\mu}{d\tau} \frac{dx^\nu}{d\tau} }d\tau
$$
Apply Euler-Lagrange to this,
$$
\frac{d}{d\tau}\left(  \frac{\partial L}{\partial \dot{x}^\mu} \right) - \frac{\partial L}{\partial x^\mu} = 0
$$
$$
\frac{d^{2}x^\mu}{d\tau^{2}} + \Gamma^\mu_{\nu \rho}\dot{x}^\nu \dot{x}^\rho = 0
$$
# Parallel Transport
Parallel transport is defined by,
$$
\nabla_{\dot{\gamma}}V^\mu = 0
$$
$$
\frac{dV^\mu}{d\tau} + \Gamma^\mu_{\nu \rho}\dot{x}^\nu V^\rho = 0
$$
This defines how vectors rotate along curves, and curvature shows up as failure of loops to return vectors unchanged.
# Riemann Tensor
The commutator of covariant derivatives is defined as,
$$
[\nabla_{\mu},\nabla_{\nu}]V^\rho = R^\rho_{\sigma \mu \nu}V^\sigma
$$
Or, in explicit form,
$$
R^\rho_{\sigma \mu \nu} = \partial_{\mu}\Gamma^\rho_{\nu \sigma} - \partial_{\nu}\Gamma^\rho_{\mu \sigma} + \Gamma^\rho_{\mu \lambda}\Gamma^\lambda_{\nu \sigma} -\Gamma^\rho_{\nu \lambda}\Gamma^\lambda_{\mu \sigma}
$$
Curvature is connected with the derivative of connection.
# Locally Inertial Frames
At any point, we can choose coordinates such that:
$$
\Gamma^\mu_{\nu \rho} = 0
$$
But,
$$
\partial_{\sigma}\Gamma^\mu_{\nu \rho} \neq 0
$$
Which implies that gravity can be removed locally, but not globally. This is the equivalence principle.