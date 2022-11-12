# Introduction

- SHM for simple pendulums only works for small angles
- Integral is used for nonlinear pendulum relationship
-  $\sin(\theta) = \theta$ only holds true for small angles
- Authors want to find a simple and accurate expression for beyond small angle

# Approximation

![[Screenshot_20221111_114816.png]]

Using torque and rotational inertia, we find that that:
$\frac{d^{2}\theta}{dt^{2}}+ \frac{g}{L}sin\theta = 0$ , which we can solve for $T = 2\pi \sqrt{\frac{L}{g}}$ 

Using Conservation of Energy to integrate for period:
$$
\begin{align*}
mgL(1- \cos\theta_0) &= \frac{1}{2} mL^{2}(\frac{d\theta}{dt})^{2}+ mgL(1-\cos(\theta)) \\
\frac{d\theta}{dt} &= \pm \sqrt{\frac{2g}{L}(\cos\theta - cos\theta_{0)}}\\
\end{align*} 
$$
Integrate from $\theta = 0$ to $\theta = \theta_0$ to find $\frac{T}{4}$
$$
\begin{align*}
T&=  2\sqrt{2}\sqrt{\frac{L}{g}} \int_{0}^{\theta_0} \frac{1}{(\sqrt{\cos\theta - \cos \theta_{0})}} d \theta\\
\end{align*}
$$
The above integral for $T$ is hard because there is an asymptote at $\theta = \theta_0$. By replacing $\cos \theta$ with $1 - 2\sin^2(\frac{\theta}{2})$ and changing variable with $\sin \varphi = \frac{\sin(\frac{\theta}{2})}{\sin(\frac{\theta}{2})}$, we can change the bounds as shown below
$$
\begin{align*}
T &= 4\sqrt{\frac{L}{g}} \int_{0}^{\frac{\pi}{2}} \frac{1}{\sqrt{1-k^{2}\sin^{2} \varphi}}d\varphi 
\end{align*}
$$