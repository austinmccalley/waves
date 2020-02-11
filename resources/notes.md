# Notes on Wave Modeling

## Waves on the Water Surface - Mathemtical Models - Part 2
We are going to work with the linear problem first.

The wave amplitude is negligible in comparison to the wave length which thus simplifies the problem.

The linear system of equations are defined below

$$ \frac{\partial ^2 \phi}{\partial x^2} + \frac{\partial^2\phi}{\partial y^2} + \frac{\partial ^2 \phi}{\partial z^2}=0 $$

$$ \frac{1}{g}\frac{\partial ^2 \phi}{\partial t^2}+\frac{\partial\phi}{\partial z}=0, z=0 $$

$$ \frac{\partial \phi}{\partial x}\frac{\partial d}{\partial x}  + \frac{\partial\phi}{\partial y}\frac{\partial d}{\partial y} + \frac{\partial \varphi}{\partial z}=0, z =-d  $$

$$ \frac{\partial \phi}{\partial t} = f_1(x,y,0),t=0,z=0$$

$$ \phi = f_2(x,y,0),t=0,z=0$$

This is where $t$ = time; $x,y,z$ = Cartesian coordinates; $d$ = depth; $g$ = gravitational acceleration; $\phi$ = velcoity potentional.

For small bed slopes $|\frac{\partial d}{\partial x}|, |\frac{\partial d}{\partial y}|<<1$ this is asymptotic ray methods. This allows more simplificiation of the problem.

#### Example
A frontal approach of waves to the shore for a non-breaking wave is
$$\eta= \sqrt{\frac{C_{g0}}{C_g}}a_0cos[\omega t-\int_{x_0}^{x}k(x)dx]$$
where $\eta$ = wave profile; $a$ = wave amplitude; $C_g$ = group speed; $\omega = \frac{2\pi}{T}$ = angular velocity; $T$ = wave period; $k = \frac{2\pi}{\lambda}$ = wave number; $\lambda$ = wave length; $\omega^2 = gk*\tanh{kd}$; the index $\ll0\gg$ is the data in the entry range $x=x_0$. The expression for the wave height $H$ is
$$h(x)=\sqrt{\frac{C_{g0}}{C_{g}}}H_0$$

First solve the plane problems, which calculates the rays along with how the weave energy is propgating. Next use the law of energy flux conersion - the wave parameters. This is the standard approach to calculating the wave transofmration in the costal zone of the sea. An intersection of the wave rays is possible, which makes the calculating much more complex, since there is a need to apply various smoothing methods.



## Rays Waves and Scattering Chapter 13

A two-dimensional ocean is a constant depth *h*. 

The variable ![\Phi](https://render.githubusercontent.com/render/math?math=%5CPhi) wll be used to signify the velocity potential.
The variable ![\xi](https://render.githubusercontent.com/render/math?math=%5Cxi) will be used to signify the free surface displacement.

The governing equations are 
![\bigtriangledown^2\Phi=0, \Phi=\Phi(x,z,t)](https://render.githubusercontent.com/render/math?math=%5Cbigtriangledown%5E2%5CPhi%3D0%2C%20%5CPhi%3D%5CPhi(x%2Cz%2Ct))


on the free upper surface
![\frac{\partial\xi}{\partial t} = \frac{\partial\Phi}{\partial z}, z = 0](https://render.githubusercontent.com/render/math?math=%5Cfrac%7B%5Cpartial%5Cxi%7D%7B%5Cpartial%20t%7D%20%3D%20%5Cfrac%7B%5Cpartial%5CPhi%7D%7B%5Cpartial%20z%7D%2C%20z%20%3D%200)


and


![\frac{\partial\Phi}{\partial t} = g\xi=\frac{-P_a(x,t)}{\rho},z=0](https://render.githubusercontent.com/render/math?math=%5Cfrac%7B%5Cpartial%5CPhi%7D%7B%5Cpartial%20t%7D%20%3D%20g%5Cxi%3D%5Cfrac%7B-P_a(x%2Ct)%7D%7B%5Crho%7D%2Cz%3D0)


where ![P_a(x,t)](https://render.githubusercontent.com/render/math?math=P_a(x%2Ct)) is the prescribed atmospheric pressure. 

The seafloor has a displacement ![$H(x,t)](https://render.githubusercontent.com/render/math?math=%24H(x%2Ct)) due to an earthquake so that now
![z = -h + H(x,t)](https://render.githubusercontent.com/render/math?math=z%20%3D%20-h%20%2B%20H(x%2Ct))



If the ground motion is known, the lower boundray is
![F(x,z,t)=0](https://render.githubusercontent.com/render/math?math=F(x%2Cz%2Ct)%3D0)
where
![F(x,z,t)=z+h-H(x,t)](https://render.githubusercontent.com/render/math?math=F(x%2Cz%2Ct)%3Dz%2Bh-H(x%2Ct))

The total derivative of F is
![\frac{\partial\Phi}{\partial z}=\frac{\partial H}{\partial t}+\frac{\partial\Phi}{\partial x}\frac{\partial H}{\partial x}; z = -h + H](https://render.githubusercontent.com/render/math?math=%5Cfrac%7B%5Cpartial%5CPhi%7D%7B%5Cpartial%20z%7D%3D%5Cfrac%7B%5Cpartial%20H%7D%7B%5Cpartial%20t%7D%2B%5Cfrac%7B%5Cpartial%5CPhi%7D%7B%5Cpartial%20x%7D%5Cfrac%7B%5Cpartial%20H%7D%7B%5Cpartial%20x%7D%3B%20z%20%3D%20-h%20%2B%20H)



If we neglect the quadratically small terms,
![\frac{\partial\Phi}{\partial z}=\frac{\partial H}{\partial t} \equiv W(x,t), z \approx -h](https://render.githubusercontent.com/render/math?math=%5Cfrac%7B%5Cpartial%5CPhi%7D%7B%5Cpartial%20z%7D%3D%5Cfrac%7B%5Cpartial%20H%7D%7B%5Cpartial%20t%7D%20%5Cequiv%20W(x%2Ct)%2C%20z%20%5Capprox%20-h)



We define the Laplace transform of the function ![f(t)](https://render.githubusercontent.com/render/math?math=f(t)) by
![f(s)= \int_{0}^{\infty} e^{-st}f(t)dt](https://render.githubusercontent.com/render/math?math=f(s)%3D%20%5Cint_%7B0%7D%5E%7B%5Cinfty%7D%20e%5E%7B-st%7Df(t)dt)

and its inverse is
![ f(t)= \frac{1}{2\pi i}\int_\Gamma e^{st}f(s)ds](https://render.githubusercontent.com/render/math?math=%20f(t%3D%20%5Cfrac%7B1%7D%7B2%5Cpi%20i%7D%5Cint_%5CGamma%20e%5E%7Bt%7Df(s)ds)


where ![\Gamma](https://render.githubusercontent.com/render/math?math=%5CGamma) is a vertical line to the right of all singularities in the complex s-plane.
