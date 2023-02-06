## Purpose

We want to caluculate how $v_\parallel$ and $v_\perp$ intaract each other under **acclelation** and **mirror force** process.

---

## Situation

---

### Resonance

Some ion accelarated by something(like resonance). 

We imagine ion cycltron resonance.

For example, ion is accelareted by ion cylotron waves.

**Resonance condition**

$\Omega_i = \omega - k_\parallel v_\parallel$

Under this condition, ion is accelarated.

**Assumption**
- Wave is electrostatic
    - $B_1 = 0$

- Wave accelate only $v_\perp$ under ion cylctron resonance.
    - That's mean, $\frac{dv_\perp}{dt} = E\frac{q}{m}$
    - And, not accelate $v_\parallel$
    - Now, $E$ is constant

---

### Mirror force

$m\frac{dv_\parallel}{dt} = \mu \nabla_\parallel B$

**Assumption**
- Dipole magetic filed

---
## Resonance limitation

**Assume** that there are only waves with frequencies close to $\Omega_i$.
- Why?
    - Because, An upper limit to the acceleration of ions is seen by observation.
    - Waves of various frequency bands, especially those lower than $\Omega_i$, should accelerate the ions to a significant degree.

(Note : $\Omega_i = \omega - k_\parallel v_\parallel$)

Based on this assumption, the resonant ions, when accelerated **by the mirror force**, should leave the resonance condition and **no longer accelerate $v_\perp$**.

The magnitude of the mirror force depends on $v_\perp$. In other words, there is a nonlinear process.

→ We need simulation.

---

## Frame

$v_\perp$ is accelarated by $E$ (resonance).

Sometime, is not acclerated because $v_\parallel$ is over some value.

Because of mirror force, $v_\parallel$ decrease.

$v_\parallel$ is accelrated by mirror force.

---

## Equation

Mirror force does not give energy to systems.

So,  

$W = W_\parallel + W_\perp$ 

$\frac{dW_\parallel}{dt} + \frac{d W_\perp}{dt} = \frac{dW}{dt} = qE v_\perp$


$\frac{dW_\parallel}{dt} + \frac{d W_\perp}{dt} = qE v_\perp$

$\frac{1}{2}m \{\frac{d(v_\perp)^2}{dt} + \frac{d(v_\parallel)^2}{dt}\} = qE v_\perp $


$m \{v_\perp\frac{dv_\perp}{dt} + v_\parallel\frac{d v_\parallel}{dt}\} = qE v_\perp $

if $v_\perp \neq 0$, 


$\frac{dv_\perp}{dt} = \frac{qE}{m} - \frac{v_\parallel}{v_\perp}\frac{d v_\parallel}{dt} $

Mirror Force is...

$m\frac{dv_\parallel}{dt} = \mu \nabla_\parallel B$


$m\frac{dv_\parallel}{dt} = \frac{1}{2B}m v_\perp^2 \nabla_\parallel B$


$\frac{dv_\parallel}{dt} = v_\perp^2\frac{1}{2}  \frac{1}{R_EL}\frac{3\sin\lambda(5\sin^2\lambda^2+3)}{\cos^{2}\lambda(1+3\sin^2\lambda)^{\frac{3}{2}}}$ 

$\lambda$ : Invarialnt latitude

$L$ : L-shell

$R_E$ : Earth Radius

---

## Last equations

$\frac{dv_\perp}{dt} = \frac{qE}{m} - \frac{v_\parallel}{v_\perp}\frac{d v_\parallel}{dt} $

$\frac{dv_\parallel}{dt} = v_\perp^2\frac{1}{2}  \frac{1}{R_EL}\frac{3\sin\lambda(5\sin^2\lambda^2+3)}{\cos^{2}\lambda(1+3\sin^2\lambda)^{\frac{3}{2}}}$ 



---
## Appendix Grad-B

In dipole,

$B = \frac{\mu_0 M_E}{4\pi}\frac{1}{R_E^3L^3}\frac{(1+3\sin^2\lambda)^\frac{1}{2}}{\cos^6\lambda}$

$\lambda$ : Invarialnt latitude

$L$ : L-shell

$R_E$ : Earth Radius

(from Basic Space Plasma Physics)

$\nabla_\parallel B = \frac{dB}{ds} = \frac{d\lambda}{ds}\frac{dB}{d\lambda} =(\frac{ds}{d\lambda})^{-1}\frac{dB}{d\lambda} $..?

$\frac{ds}{d\lambda} = LR_E\cos\lambda(1+3\sin^2\lambda)^{\frac{1}{2}}$
(from Basic Space Plasma Physics)

$\frac{dB}{d\lambda} = \frac{\mu_0 M_E}{4\pi}\frac{1}{R_E^3L^3}\frac{\cos^6\lambda(1+3\sin^2\lambda)^\frac{-1}{2}(\frac{1}{2}6.0\sin\lambda\cos\lambda)-(1+3\sin^2\lambda)^\frac{1}{2}*6\cos^5\lambda(-\sin(\lambda))}{\cos^{12}\lambda}$
$= \frac{\mu_0 M_E}{4\pi}\frac{1}{R_E^3L^3}\frac{\cos^2\lambda(1+3\sin^2\lambda)^\frac{-1}{2}(3\sin\lambda)-(1+3\sin^2\lambda)^\frac{1}{2}*6(-\sin(\lambda))}{\cos^{7}\lambda}$


$\nabla_\parallel B = (\frac{ds}{d\lambda})^{-1}\frac{dB}{d\lambda} $

$= \frac{1}{LR_E\cos\lambda(1+3\sin^2\lambda)^{\frac{1}{2}}} \frac{\mu_0 M_E}{4\pi}\frac{1}{R_E^3L^3}\frac{\cos^2\lambda(1+3\sin^2\lambda)^\frac{-1}{2}(3.0\sin\lambda)-(1+3\sin^2\lambda)^\frac{1}{2}*6(-\sin(\lambda))}{\cos^{7}\lambda}$


$= \frac{\mu_0 M_E}{4\pi}\frac{1}{R_E^3L^3(R_EL)}\frac{\cos^2\lambda(3\sin\lambda)-(1+3\sin^2\lambda)*6(-\sin(\lambda))}{\cos^{8}\lambda(1+3\sin^2\lambda)}$


$= \frac{\mu_0 M_E}{4\pi}\frac{1}{R_E^3L^3(R_EL)}\frac{\sin\lambda(3\cos^2\lambda+6(1+3\sin^2\lambda))}{\cos^{8}\lambda(1+3\sin^2\lambda)}$


$= \frac{\mu_0 M_E}{4\pi}\frac{1}{R_E^3L^3(R_EL)}\frac{3\sin\lambda(\cos^2\lambda+2(1+3\sin^2\lambda))}{\cos^{8}\lambda(1+3\sin^2\lambda)}$


$= \frac{\mu_0 M_E}{4\pi}\frac{1}{R_E^3L^3(R_EL)}\frac{3\sin\lambda(5\sin^2\lambda^2+3)}{\cos^{8}\lambda(1+3\sin^2\lambda)}$



$\frac{\nabla_\parallel B}{B}$

$= \frac{\mu_0 M_E}{4\pi}\frac{1}{R_E^3L^3(R_EL)}\frac{3\sin\lambda(5\sin^2\lambda^2+3)}{\cos^{8}\lambda(1+3\sin^2\lambda)} \frac{4\pi}{\mu_0 M_E}R_E^3L^3
 \frac{\cos^6\lambda}{(1+3\sin^2\lambda)^\frac{1}{2}}$


$=\frac{1}{R_EL}\frac{3\sin\lambda(5\sin^2\lambda^2+3)}{\cos^{2}\lambda(1+3\sin^2\lambda)^{\frac{3}{2}}}$ 

The first equation is the formula for the magnetic field (B) of a magnetic dipole at a certain radial distance (R) from the center of the Earth. $M_E$ is the Earth's magnetic moment, $\mu_0$ is the vacuum permeability, $\lambda$ is the invariant latitude (angle between the magnetic field vector and the Earth's surface), and $L$ is the L-shell (a measure of the radial distance from the center of the Earth).

The second equation is the formula for the derivative of the magnetic field along the radial direction (parallel to the radial direction), which is referred to as $\nabla_\parallel B$. The derivative is calculated by taking the partial derivative of the magnetic field with respect to the invariant latitude ($\frac{dB}{d\lambda}$) and multiplying it by the reciprocal of the derivative of the invariant latitude with respect to the radial distance along the Earth's surface ($(\frac{ds}{d\lambda})^{-1}$).

The third equation is an expression for the derivative of the invariant latitude with respect to the radial distance along the Earth's surface.

Finally, the last equation is the ratio of the derivative of the magnetic field along the radial direction to the magnetic field itself. This equation can be used to determine the relative variation of the magnetic field along the radial direction.

Methods:

In this study, we calculated the gradient of the magnetic field, $\nabla_\parallel B$, in a dipole magnetic field. The magnetic field, $B$, was first expressed as a function of the invariant latitude, $\lambda$, L-shell, $L$, and Earth's radius, $R_E$. The gradient of the magnetic field was then calculated by taking the derivative of $B$ with respect to $\lambda$.

To obtain this derivative, we first calculated $\frac{ds}{d\lambda}$, the derivative of the distance along a field line with respect to the invariant latitude. We then calculated $\frac{dB}{d\lambda}$ and expressed the gradient of the magnetic field, $\nabla_\parallel B$, as the product of $\frac{dB}{d\lambda}$ and $(\frac{ds}{d\lambda})^{-1}$. The resulting expression for $\nabla_\parallel B$ was further simplified and expressed as a function of $\lambda$.

Finally, we expressed the ratio of the gradient of the magnetic field to the magnetic field itself, $\frac{\nabla_\parallel B}{B}$, in terms of $\lambda$.