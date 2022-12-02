1. a. Write the Lagrangian
$$
\begin{align*}
L &= T - V\\
T &= \frac{1}{2}m\dot{x}^{2}\\
V &= mgh\\
&= mgx\sin \theta\\
L &= \frac{1}{2}m\dot{x}^{2} - mgx\sin \theta\\
\end{align*}
$$
b. Write the Hamiltonian
$$
\begin{align*}
H &= T + V\\
H &= \frac{1}{2}m\dot{x}^{2}+ mgx\sin \theta \\
p &= m\dot{x} \implies \dot{x} = \frac{p}{m}\\
H &= \frac{p^{2}}{2m} + { mgx\sin \theta} \\
\end{align*}
$$
c. Solving for Lagrange:
$$
\begin{align*}
L &= \frac{1}{2}m\dot{x}^2-mgx\sin \theta\\
\frac{ \partial L }{ \partial x } &= -mg\sin \theta\\
\frac{d}{dt} \frac{ \partial L }{ \partial \dot{x} } &= m\ddot{x}\\
-mg\sin \theta &= m\ddot{x}\\
\ddot{x} &= -g\sin \theta \\
\end{align*}
$$
Solving for Hamiltonian:
$$
\begin{align*}
H &= \frac{1}{2}m\dot{x}^{2}+ mgx\sin \theta\\
-\frac{ \partial H }{ \partial x }  &= mg\sin \theta \implies \dot{p} = mg\sin \theta\\
\frac{d}{dt}\frac{ \partial H }{ \partial p } &= \frac{d}{dt}\frac{p}{m} = \frac{\dot{p}}{m} \implies \ddot{x} = \frac{\dot{p}}{m} \\
mg\sin \theta &= m\ddot{x}\\
\ddot{x} &= g\sin \theta 
\end{align*}
$$
2. 
a. 
$$
\begin{align*}
L &= T - V\\
T &= \frac{1}{2}m\dot{y}^2\\
V &= \frac{1}{2}ky^{2} + mgy\\
L &= \frac{1}{2}m\dot{y}^{2} - \frac{1}{2}ky^{2} - mgy\\
\end{align*}
$$
b. 
$$
\begin{align*}
H &= T + V\\
H &= \frac{1}{2}m\dot{y}^{2} + \frac{1}{2}ky^{2} + mgy\\
p &= m\dot{y} \implies \dot{y} = \frac{p}{m}\\
H &= \frac{p^{2}}{2m} + \frac{1}{2}y^{2} + mgy\\
\end{align*}
$$
c.  Solving using Lagrangian
$$
\begin{align*}
L &= \frac{1}{2}m\dot{y}^{2} - \frac{1}{2}ky^{2} - mgy\\
\frac{ \partial L }{ \partial y } &= -ky - mg\\
\frac{d}{dt} \frac{ \partial L }{ \partial \dot{y} } &= m\ddot{y}\\
m\ddot{y} &= -ky - mg\\
\ddot{y} &= -\frac{k}{m}y - g\\
\end{align*}
$$
Solving using Hamiltonian
$$
\begin{align*}
H &= \frac{p^{2}}{2m} + \frac{1}{2}y^{2} + mgy\\
-\frac{ \partial H }{ \partial y } &= -y -mg \implies \dot{p} = -ky -mg\\
\frac{d}{dt}\frac{ \partial H }{ \partial p } &= \frac{\dot{p}}{m} \implies \ddot{y} = \frac{\dot{p}}{m}\\
-ky - mg &= m\ddot{y}\\
\ddot{y} &= -\frac{k}{m}y - g
\end{align*}
$$
3. Lagrangian for projectile
$$
\begin{align}
L &= \frac{1}{2}m\dot{x}^{2} \\
\frac{ \partial L }{ \partial x } &= \frac{d}{dt}\frac{ \partial L }{ \partial \dot{x} }\\
m\ddot{x} &= 0 \implies \ddot{x} = 0 \\
L &= \frac{1}{2}m\dot{y}^{2} -mgy \\
\frac{ \partial L }{ \partial y } &= \frac{d}{dt}\frac{ \partial L }{ \partial \dot{y} }\\
m\ddot{y} &= -mg \implies \ddot{y} = -g
\end{align}
$$

4. 
a. Write the Lagrangian
$$
\begin{align*}
L &= T - V\\
L &= \frac{1}{2}m\dot{x}^{2} + \frac{1}{2}m\dot{y}^2 - \frac{1}{2}k(x^2+y^2)\\
\end{align*}
$$
b. Write the Hamiltonian
$$
\begin{align*}
H &= T + V\\
H &= \frac{1}{2}m\dot{x}^{2} + \frac{1}{2}m\dot{y}^2 + \frac{1}{2}k(x^2+y^2)\\
p_{x} &= m\dot{x}, p_{y} = m\dot{y}\\
H &= \frac{p_{x}^2}{2m} + \frac{p_{y}^2}{2m} + \frac{1}{2}k(x^2+y^2)
\end{align*}
$$
c. 
Using Langrangian to find equation of motion $x(t)$
$$
\begin{align*}
\frac{ \partial L }{ \partial x } &= -kx\\
\frac{d}{dt} \frac{ \partial L }{ \partial \dot{x} } &= m\ddot{x}\\
m\ddot{x} &= -kx\\
\ddot{x} &= -\frac{k}{m}x\\ 
\end{align*}
$$
Using Hamiltonian to find equation of motion $x(t)$
$$
\begin{align*}
-\frac{ \partial H }{ \partial x } &= -kx \implies \dot{p} = -kx\\ 
\frac{d}{dt} \frac{ \partial H }{ \partial p_{x} } &= \frac{\dot{p}}{m} \implies \ddot{x} = \frac{\dot{p}}{m}\\
m\ddot{x} &= -kx\\
\ddot{x} &= -\frac{k}{m} x
\end{align*}
$$
5. 
a. Writing the Lagrangian
$$
\begin{align*}
L &= T - V\\
T &= \frac{1}{2}m \dot{r}^{2} + \frac{1}{2}m(r\dot{\theta})^{2} \\
V &= \frac{1}{2}kr^2\\
L &= \frac{1}{2}m(\dot{r}^{2} + r^{2}\dot{\theta}^{2}) - \frac{1}{2}kr^2\\
\end{align*}
$$
b. Write the Hamiltonian
$$
\begin{align*}
H &= T + V \\
T &= \frac{1}{2}m \dot{r}^{2} + \frac{1}{2}m(r\dot{\theta})^{2} \\
p_{r} &= m \dot{r} \implies \dot{r} = \frac{p_{r}}{m} \\
p_{\theta} &= \frac{ \partial L }{ \partial \dot{\theta} } = mr^{2}\dot{\theta} \implies \dot{\theta} = \frac{p_{\theta}}{mr^{2}} \\
V &= \frac{1}{2}kr^2 + mgr(1-\cos \theta) \\
H &= \frac{p_{r}^2}{2m} + \frac{p_{\theta}^{2}}{2mr^{2}} + \frac{1}{2}kr^2\\
\end{align*}
$$

c. Solving the Lagrangian for radial and angular acceleration:
$$
\begin{align}
L &= \frac{1}{2}m(\dot{r}^{2} + r^{2}\dot{\theta}^{2}) - \frac{1}{2}kr^2\\
\frac{ \partial L }{ \partial r } &= mr\dot{\theta}^2 - kr \\
\frac{d}{dt} \frac{ \partial L }{ \partial \dot{r} } &= m\ddot{r}  \\
\ddot{r} &= r\dot{\theta}^2 -\frac{k}{m}r \\
\frac{ \partial L }{ \partial \theta } &= 0 \\
\frac{d}{dt} \frac{ \partial L }{ \partial \dot{\theta} } &= \frac{d}{dt} m\dot{\theta}r^{2} = 2mr\dot{\theta} + mr^{2} \ddot{\theta} \\
2mr\dot{\theta} + mr^{2}\ddot{\theta} &= 0 \implies \ddot{\theta} = \frac{-2\dot{\theta}\dot{r}}{r} \\
\end{align}
$$
Solving the Hamiltonian :
$$
\begin{align}
H &= \frac{p_{r}^2}{2m} + \frac{p_{\theta}^{2}}{2mr^{2}} + \frac{1}{2}kr^2\\
-\frac{ \partial H }{ \partial r } &= \dot{p_{r}} = -mp_{\theta}^{2}r^{-3} + kr \\ 
\frac{d}{dt} \frac{ \partial H }{ \partial p_{r}} &= \ddot{r} = \frac{\dot{p_{r}}}{m} \\
m \ddot{r} &= -mp_{\theta}^{2}r^{-3} - kr \implies \ddot{r} = -r\dot{\theta}^{2} + \frac{k}{m}r \\
-\frac{ \partial H }{ \partial \theta } &= \dot{p_{\theta}}  = 0 \\
\frac{d}{dt} \frac{ \partial H }{ \partial p_{\theta} } &\implies \dot{p}_{\theta} = \frac{d}{dt}mr^{2}\dot{\theta} \\
2mr \dot{r}\dot{\theta} + mr^{2}\ddot{\theta} &= 0 \implies \ddot{\theta} = -2\frac{\dot{\theta}\dot{r}}{r}
\end{align}
$$

5. a. Kinetic and potential energy in terms of Cartesian coordinates:
$$
\begin{align}
T &= \frac{1}{2} m (\dot{x}^{2} + \dot{y}^2) + \frac{1}{2}M\dot{Y}^{2} \\
V &= mg(Y + r\cos \theta)
\end{align}
$$
b. Holonomic Constraints: 
$$
\begin{gather*}
X = 0 \\
Z = 0 \\
z = 0 \\
[x^{2} + (y-Y)^{2}] = l^2
\end{gather*}
$$
c. Transforming the coordinates to have **3 degrees of freedom**
$$
\begin{gather}
x = l\sin \theta \implies \dot{x} = l\dot{\theta}\cos \theta\\
y = l\cos \theta + Y \implies \dot{y} = -l\dot{\theta}\sin \theta + \dot{Y} \\
\end{gather}
$$
$$
\begin{align}
T &= \frac{1}{2}m[(l\dot{\theta}\cos \theta)^{2} + (\dot{Y} - l\dot{\theta}\sin \theta)^{2}] + \frac{1}{2}M\dot{Y}^2 \\
T &= \frac{1}{2}m[\dot{Y}^{2} + (l\dot{\theta})^{2} + { 2\dot{Y}l\dot{\theta}\cos \theta}] + \frac{1}{2}M\dot{Y}^2 \\
V &= mg(Y + l\cos \theta)
\end{align}
$$
d. The new expressions make sense because the kinetic energy is now a function of the radial and tangential velocities and the masses, and the potential energy is a function of $Y$ and the component of the pendulum length along the y-axis.

e. Lagrangian in generalized coordinates:
$$
L = \frac{1}{2}m[\dot{Y}^{2} + (l\dot{\theta})^{2} + { 2\dot{Y}l\dot{\theta}\cos \theta}] + \frac{1}{2}M\dot{Y}^2 - mg(Y + mgl\cos \theta)
$$