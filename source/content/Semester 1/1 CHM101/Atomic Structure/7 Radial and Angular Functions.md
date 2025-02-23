In the polar coordinate system, the 3d coordinates are replaced by:

$x = r\sin\theta \cdot \cos \phi$
$y = r\sin\theta \cdot\sin \phi$
$z=r\cos\theta$

$r = \sqrt{ x^{2}+y^{2}+z^{2} }$

The Schrodinger eqn in 3 dimensions can be written as:

$\nabla^{2}\psi +\frac{8\pi^{2}m}{h^{2}}\cdot(E-V)\psi=0$

changing this to polar coordinate form:

$\nabla^{2}\psi=\frac{1}{r^{2}}\cdot \frac{\partial}{\partial r}\left( r^{2}\cdot \frac{\partial \psi}{\partial r} \right)+\frac{1}{r^{2}\sin\theta}\cdot \frac{\partial}{\partial\theta}\left( \sin\theta \cdot \frac{\partial \psi}{\partial \phi} \right)+\frac{1}{r^{2}\sin\theta}\cdot \frac{\partial \psi^{2}}{\partial \phi^{2}}$

Note:
1. $\psi = R(r)\cdot\Theta(\theta)\cdot \Phi(\phi)$
2. R(r) depends on the distance from the nucleus, which in turn depends on the quantum numbers n, l
3. $\theta(\theta)$ depends on quantum numbers m, l
4. $\phi(\phi)$ depends only on m

This makes the eqn: $\psi = R(r)_\text{n,l}\cdot A_\text{m,l}$

R = radial function --> has no physical meaning, but R^2 represents the probability density of finding an electron in small volume dv, near the point at which R is measured, for a given value of r, the small volumes measured are $4\pi r^{2}$, and the probability is $4\pi r^{2}R^{2}$.
A = angular function --> is independent of distance from the nucleus, and depends only on direction. A^2 is the angular probability density of finding an electron for a given phi and theta.










