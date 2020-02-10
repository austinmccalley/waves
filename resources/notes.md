# Notes

## Rays Waves and Scattering Chapter 13

A two-dimensional ocean is a constant depth *h*. 

The variable $\Phi$ wll be used to signify the velocity potential.
The variable $\xi$ will be used to signify the free surface displacement.

The governing equations are 
$$ \bigtriangledown^2\Phi=0, \Phi=\Phi(x,z,t) $$
on the free upper surface
$$ \frac{\partial\xi}{\partial t} = \frac{\partial\Phi}{\partial z}, z = 0$$
and
$$ \frac{\partial\Phi}{\partial t} = g\xi=\frac{-P_a(x,t)}{\rho},z=0 $$
where $P_a(x,t)$ is the prescribed atmospheric pressure. 

The seafloor has a displacement $H(x,t)$ due to an earthquake so that now
$$ z = -h + H(x,t)$$

If the ground motion is known, the lower boundray is
$$F(x,z,t)=0$$
where
$$F(x,z,t)=z+h-H(x,t)$$

The total derivative of F is
$$ \frac{\partial\Phi}{\partial z}=\frac{\partial H}{\partial t}+\frac{\partial\Phi}{\partial x}\frac{\partial H}{\partial x}; z = -h + H $$

If we neglect the quadratically small terms,
$$ \frac{\partial\Phi}{\partial z}=\frac{\partial H}{\partial t} \equiv W(x,t), z \approx -h$$

We define the Laplace transform of the function $f(t)$ by
$$ f(s)= \int_{0}^{\infty} e^{-st}f(t)dt$$

and its inverse is
$$ f(t)= \frac{1}{2\pi i}\int_\Gamma e^{st}f(s)ds $$
where $\Gamma$ is a vertical line to the right of all singularities in the complex s-plane.
