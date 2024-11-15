# Further Mechanics
## Circular Motion

$$1 \mbox{ } rad =\frac{180}{\pi}^o$$

Arc length:

$$l=r\theta$$

where $l$ is the length of the arc, $r$ is the radius of the circle and $\theta$ is the angle in radians.

Angular velocity:

$$\omega = \frac{\Delta \theta}{\Delta t}$$
where $\omega$ is angular velocity, $\Delta \theta$ is the change in the angle, and $\Delta t$ is the change in time. The unit is $rad \mbox{ }s^{-1}$


### Comparison to linear velocity

Linear velocity is when an object is travelling in a straight line:

$$v=\frac{\Delta s}{\Delta t}$$

The equation for arc length helps compare linear and angular velocity:

$$\Delta s = r \Delta \theta$$

By substituting one in to the other we get the equation:

$$v = r \omega$$

Which means that linear velocity is proportional to the distance from the centre, $r$.

### Periodic motion

$$T = \frac{1}{f}$$

The equation for angular velocity is $\omega = \frac{ \Delta \theta}{\Delta t}$, by assuming the object performs a full rotation of $2\pi$ radians, the equation becomes $\omega = \frac{2\pi}{\Delta t}$. Since a full rotation (1 oscillation) has been completed, the change in time is equal to the time period. With this, the equation could be written in two different ways:

$$\omega = \frac{2\pi}{T}$$

and:

$$\omega = 2\pi f$$

### Centripetal Acceleration

While moving in a circle, the velocity of an object is always changing, meaning it is always accelerating.

During circular motion, acceleration always points towards the centre of the circle.

$$a_c = \frac{\Delta v}{\Delta t}$$

Is the equation for centripetal acceleration where $a_c$ is the centripetal acceleration.

This could also be written as:

$$a_c = \frac{v^2}{r}$$

since $v = \frac{r}{t}$ and rearranging for $t$ gives $\frac{r}{v}$ which simplifies to the equation above. By substituting $v=r\omega$ into the equation, you get:

$$a_c = r\omega^2$$

### Centripetal Force

According to Newton's second law:

$$F=ma$$

and by substituting $a_c = \frac{v^2}{r}$ or $a_c = r\omega^2$ into the equation we get that centripetal force is:

$$F_c=\frac{mv^2}{r}$$

and:

$$F_c = mr\omega^2$$


## Simple Harmonic Motion

Simple harmonic motion (SHM) is any motion in which the acceleration is directed towards a fixed point <b>AND</b> is directly proportional to the negative of the displacement.

SHM can be expressed as:

$$a = -\omega^2x$$

Where $a$ is the acceleration, $\omega$ is the angular velocity, and $x$ is the displacement.

### Acceleration-displacement graph

An acceleration-displacement graph of an object in SHM would be a straight line that passes through the origin with a negative gradient such that $gradient = -\omega^2$which gives the equation $\omega = \sqrt{-gradient}$

The maximum acceleration is given by $a_{max} = \omega^2A$ where $A$ is the maximum displacement.

### SHM Graphs

Displacement-time, velocity-time and acceleration-time graphs of objects in SHM are some type of $sin$ or $cos$ graph.

For example, if a pendulum is released from a high point, its corresponding displacement-time, velocity-time and acceleration-time graphs would be the following:

| Graph $y$-axis | Equation |
|---| --- |
| Displacement | $cos(t)$
| Velocity | $-sin(t)$
| Acceleration | $-cos(t)$

<b> Note </b> that the equation for an acceleration-time graph is the equation for a velocity-time graph differentiated in respect to $t$. The same is true for the equation of the velocity-time graph being the differential of the equation of the displacement-time graph. Also the equation wouldn't always be just $cos(t)$ or $-sin(t)$, these are just examples.

The maximum displacement of an object in SHM can be found when $cos(\omega t) = 1$, which is represented by $A$.

The maximum speed is given by $v = \omega A$. The maximum acceleration is given by $a = \omega^2A$.

### Simple Harmonic Systems

#### Mass-Spring System

The equation for the time period of a mass-spring system is:

$$T = 2\pi \sqrt{\frac{m}{k}}$$

Where $T$ is the time period, $m$ is the mass in kg, and $k$ is the spring constant of the spring.

#### Simple Pendulum System

The equation for the time period of a simple pendulum system is:

$$T = 2\pi \sqrt{\frac{l}{g}}$$

Where $T$ is the time period, $l$ is the length of the string, and $g$ is the gravitational field strength.

### Energy in SHM Systems

In an isolated system (one where neither matter nor energy is able to enter or leave) the total energy would always be the same. So:

$$E_T = E_k + E_g + Ee$$

Where $E_T$ is the total energy, $E_k$ is the kinetic energy, $E_g$ is the gravitational potential energy, and $E_e$ is the elastic potential energy.

Each of which are given by:

$$E_k=\frac{1}{2}mv^2$$

$$E_g = mgh$$

$$E_e = \frac{1}{2}kx^2$$


#### Damping
\
Real world systems aren't usually isolated systems, so the forces such as friction reduce the energy of the object(s) in SHM.

Damping is when the amplitude of a wave decreases but the frequency/period remains the same.

### Resonance

# Thermal Physics

## Ideal Gases

**Boyle's Law** : $pV = constant$

**Charles' Law** : $\frac{V}{T}=constant$

**Pressure Law** : $\frac{p}{T}=constant$

$$\frac{pV}{T}=constant$$

$$\frac{p_1V_1}{T_1}=\frac{p_2V_2}{T_2}$$

T is in kelvin.

Use the equation above when evaluating a change/difference in a gas.

For the equations to work, the gas must be an ideal gas.

**Ideal gas** $-$ a gas that obeys the gas laws at all pressures and temperatures. The internal energy of an ideal gas is only dependent on the kinetic energy of its particles, that particles do not have any energy.

### Ideal gas assumptions

- All gas particles are identical
- All particle motion is continual and random (Brownian motion)
- All particles move in a straight line
- All particles have a negligible volume compared to the volume of the container
- There is no attraction between the practicals
- The internal energy of a gas is only kinetic energy and has no potential energy
- All collisions are elastic
- The duration of each collision is negligible compared to the time between collisions

$$\frac{pV}{T}=R$$

The equation above is true for all ideal gases and $R$ is the molar gas constant, $8.31 \textrm{ }JK^{-1}mol^{-1}$.

If the volume and temperature of a gas are kept constant then the pressure depends on R and the number of particles in the container.

$$\frac{pV}{T}=nR$$

Where $n$ is the number of moles in the gas. The equation can be rearranged to give $pV=nRT$.

Number of moles can be calculated with $n = \frac{m}{M}$ where $n$ is the number of moles, $m$ is the mass in kg and $M$ is the molar mass

### Particle in a box model

- Gas is ideal (described above)