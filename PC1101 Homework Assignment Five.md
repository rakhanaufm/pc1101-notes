Muhammad Rakha Naufal Maulana A0330820U
# 1. Non-relativistic Limit
Let's start from the Lorentz boost
$$
x' = \gamma(x-vt), \space t' = \gamma\left( t - \frac{vx}{c^{2}} \right)
$$
for $v \ll c$, we have $\gamma \approx 1$
and $\frac{vx}{c^{2}} \to 0$
Thus, we get 
$$
x' \approx x-vt, \space t'\approx t
$$
Q.E.D.
# 2. Composition of Co-linear Boosts
Using Lorentz boost,
$$
t'= \gamma\left( t- \frac{vx}{c^{2}} \right), \space x' = \gamma(x-vt)
$$
differentiating the two equations gives us
$$
dt' = \gamma\left( dt - \frac{vdx}{c^{2}} \right), \space dx' = \gamma(dx - vdt)
$$
taking $\frac{dx'}{dt'}$, we get
$$
\frac{dx'}{dt'} = \frac{\gamma(dx-vdt)}{\gamma\left( dt - \frac{vdx}{c^{2}} \right)} = \frac{\left( \frac{dx}{dt} - v \right)}{1 - \left( \frac{vdx}{dtc^{2}} \right)}
$$
Using $V = \frac{dx}{dt}, u = \frac{dx'}{dt'}$ and rearranging gives us
$$
u = \frac{V-v}{1- \frac{Vv}{c^{2}}} \Rightarrow V = \frac{v + u}{1 + \frac{uv}{c^{2}}}
$$

# 3. Composition of Boosts in Different Directions
a)
Let's first do the boost in the $z$-direction
$$
z' = \gamma_{u}(z-ut), \space ct' = \gamma_{u}(ct - \beta_{u}z), \space x'=x, y'=y
$$
now let's do the boost in the $x$-direction
$$
x'' = \gamma_{v}(x'-vt'), \space ct'' = \gamma_{v}(ct' - \beta_{v}x'), \space z'' =z', y''=y'
$$
Now let's substitute to get the form in question, because $x' = x$ and $t' = \gamma_{u} (t- \frac{uz}{c^{2}})$. 
We get for $x''$
$$
x'' = \gamma_{v} \left[ x-v\gamma_{u}\left( t - \frac{uz}{c^{2}} \right) \right] = \gamma_{v}[x-\beta_{v}\gamma_{u}(ct-\beta_{u}z)]
$$
now for $z''$
$$
z'' = \gamma_{u}(z-ut)
$$
for $y''$
$$
y''=y'=y
$$
lastly for $ct''$
$$
ct'' = \gamma_{v}[\gamma_{u}(ct-\beta_{u}z)-\beta_{v}x] = \gamma_{v}\gamma_{u}\left[ ct-\left( \beta_{u}z + \frac{\beta_{v}x}{\gamma_{u}} \right) \right]
$$
b)
Let's show that $\gamma_{u}\gamma_{v} = \gamma_{w}$. From the given definition we have
$$
\mathbf{w} = \mathbf{u} + \frac{1}{\gamma_{u}}\mathbf{v}
$$
Thus,
$$
w^{2} = u^{2} + \frac{v^{2}}{\gamma_{u}^{2}}
$$
because $\mathbf{u}$ and $\mathbf{v}$ are orthogonal with each other. Notice that because
$$
\gamma_{u}^{2} = \frac{1}{1 - \frac{u^{2}}{c^{2}}}
$$
then
$$
\frac{v^{2}}{\gamma_{u}^{2}} = v^{2}\left( 1 - \frac{u^{2}}{c^{2}} \right)
$$
Thus,
$$
\frac{w^{2}}{c^{2}} = \frac{u^{2}}{c^{2}} + \frac{v^{2}}{c^{2}} - \frac{u^{2}v^{2}}{c^{4}}
$$
$$
1 - \frac{w^{2}}{c^{2}} = \left( 1-\frac{u^{2}}{c^{2}} \right)\left( 1 - \frac{v^{2}}{c^{2}} \right)
$$
Take the square root, and we get
$$
\gamma_{w} = \frac{1}{\sqrt{ 1- \frac{w^{2}}{c^{2}} }} = \gamma_{u}\gamma_{v}
$$
c)
If this is a pure boost in the $\hat{w}$-direction, then it must be true that
$$
c_{w}z'' + s_{w}x'' = \gamma_{w}(c_{w}z+s_{w}x - wt)
$$
with
$$
\hat{w} = c_{w}\hat{z} + s_{w}\hat{x}
$$
Now let's check the coefficient of $z$. 
Let's calculate the left hand side, focusing only on the coefficients of $x$. 
$$
c_{w}z'' + s_{w}x'' = c_{w}\gamma_{u}(z-ut) + s_{w}\gamma_{v}[x-\beta_{v}\gamma_{u}(ct-\beta_{u}v)]
$$
Left hand side, we have
$$
s_{w}\gamma_{v}x
$$
Now let's observe the right hand side, the $z$ coefficient must be
$$
\gamma_{w}s_{w}x
$$
Now let's compare, for them to be equal this equation must hold true
$$
\gamma_{v}s_{w} = \gamma_{w}s_{w} \Rightarrow \gamma_{v} = \gamma_{w}
$$
$$
\gamma_{v} = \gamma_{v}\gamma_{u}
$$
$$
\gamma_{u} = \frac{1}{\sqrt{ 1 - \frac{u^{2}}{c^{2}} }} = 1
$$
However, this is never true. The reason is that $u$ is non-zero, or $\gamma_{u} \neq 1$
d)
If we instead flip the order of the boost, say doing $x$-direction and then the $z$-direction. We have for the $\mathbf{w}$ 
$$
\mathbf{w}^\star = \frac{\mathbf{u}}{\gamma_{v}} + \mathbf{v}
$$
It is obvious that $\mathbf{w}^\star \neq \mathbf{w}$ as the gamma factor appears in different components. However, the magnitude
$$
|\mathbf{w}^\star|^{2} = \frac{u^{2}}{\gamma_{v}^{2}} + v^{2}
$$
is the same as
$$
|\mathbf{w}^\star|^{2} = u^{2}\left( 1 - \frac{v^{2}}{c^{2}} \right) + v^{2} = u^{2} + v^{2} - \frac{u^{2}v^{2}}{c^{2}}
$$
$$
|\mathbf{w}|^{2} = u^{2} + v^{2} \left( 1- \frac{u^{2}}{c^{2}} \right) = u^{2} + v^{2} -\frac{u^{2}v^{2}}{c^{2}}
$$
