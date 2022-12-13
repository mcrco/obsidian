# Moment of Inertia for Water Spout

To solve for the moment of inertia of the water spout, we split up the water spout into 3 components: the inner hub, the 6 spokes, and the outer ring. We found the volume density of the PLA filament used in the water spout (1.24 g/cm^3) online and by multiplying that value by a height of 0.508 cm^3, we get an area density of 0.63 g/cm^3. Approximating the shape of the spokes to be rectangles, we get the following expression for rotational inertia:

$$
\begin{align}
I &= \int_{0}^{1} r^{2} \cdot 0.63 \cdot 2\pi r \, dr + 6 \int_{x=-0.7239}^{0.7239} \int_{y=1}^{y=8.5725} (x^{2}+y^{2}) \cdot 0.63 \, dy  \, dx + \int_{8.5725}^{9.8425} r^{2}\cdot 0.63 \cdot 2\pi r \, dr \\ 
&= 0.99 + 1154.63 + 3942.85 \\
&= 5098.48

\end{align}
$$

The first integral term is the hub, the second integral is the spokes, and the third integral is the outer ring.

# Moment of Inertia of Wheels

To find the moment of inertia of the wheels, I first calculated the area density of the wheel by dividing the mass by the area of the cross-section perpendicular to the axle. The area of the cross section was approximated by assuming the hub was of negligible mass and that the wheel was composed of three sections: the inner ring with inner and outer radii of 32 and 43 cm, respectively, 12 spokes with a length of 2 cm and a width of 0.4 cm.

$$
\begin{align}
A &= 42^{2}\pi - 32^{2}\pi + 72^{2}\pi - 62^{2}\pi + 12(0.4)(2) \\
&= 74.945 \\
\rho &= \frac{56}{A} = 0.7472 \\
\end{align}
$$

Now for the rotational inertia:

$$
\begin{align}
I &= \int_{3.2}^{4.2} r^{2}\cdot 0.7472 \cdot 2\pi \, dr + \int_{x=-0.2}^{x=0.2} \int_{4.2}^{6.2} (x^{2}+y^{2}) 0.7472 \, dy  \, dx + \int_{6.2}^{7.2} r^{2} \cdot 0.7472 \cdot 2\pi \, dr \\
&= 242.15 + 16.37 + 1419.88 \\
&= 1419.88  
\end{align}
$$

