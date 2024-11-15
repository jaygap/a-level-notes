# Thermal Physics

## Molecular Kinetic Theory Model

- This is a model of gaseous particles in a box.
- It makes several assumptions:
	- There are no intermolecular forces between the particles
	- The duration of a collision is negligible in comparison to the time between collisions
	- The motion of molecules is random
	- All collisions are perfectly elastic
	- The particles follow Newton's Laws
	- The particles move in straight lines
- The model is used to derive the equations for the energy of a **single** gas molecule in an ideal gas.

$$\frac{1}{2}m(c_{rms})^2=\frac{3}{2}kT=\frac{3RT}{2N_a}$$

- Where $m$ is the mass of the molecule, $c_{rms}$ is the average speed of a molecule in the gas, $k$ is the Boltzmann constant, $T$ is the temperature of the gas, $R$ is the molar gas constant, and $N_a$ is Avogadro's constant.

## Ideal Gases

### Charles' Law

$$V \propto T$$

$$V=kT$$

### Boyle's Law

$$p \propto \frac{1}{V}$$

$$pV=k$$

### Pressure Law

$$P \propto T$$

$$p=kT$$

- Putting these equations together gives:

$$pV=nRT=NkT$$

- Where $p$ is pressure, $V$ is volume, $n$ is the number of moles, $R$ is the molar gas constant, $T$ is temperature, $N$ is the number of molecules and $k$ is the Boltzmann constant.

- To calculate the number of moles of a substance is:

$$\textrm{mass (m) = molecular mass (M)} \times \textrm{number of moles (n)}$$

- To calculate the number of molecules in a substance is:

$$\textrm{number of molecules (N) = number of moles (n)} \times \textrm{Avogadro's constant } (N_a)$$

$$\frac{m}{M}=n$$

$$N=n \times N_a$$

## Thermal Energy Transfer

- The internal energy of a body is the sum of potential and kinetic energies of all its particles.
- The internal energy of a system can be increased by giving it more energy (by heating or doing work)
- When a substance changes state its internal energy also changes.
	- $\textrm{solid} \rightarrow \textrm{liquid = increased energy}$
	- $\textrm{liquid} \rightarrow \textrm{gas = increased energy}$
	- The opposite is also true.
	- $\textrm{gas} \rightarrow \textrm{liquid = decreased energy}$
	- $\textrm{liquid} \rightarrow \textrm{solid = decreased energy}$
- The equation for the change in temperature of a substance is:

$$Q=mc\Delta \theta$$

- Where $Q$ is the energy required to change temperature, $m$ is the mass of the substance, $c$ is the specific heat capacity of the substance (the amount of energy required to increase the temperature of $1$kg of the substance by $\textrm{1 }^oC$ (or $K$ as they are proportional to each other)) and $\Delta \theta$ is the change in temperature.
- The equation for the change in state of a substance is:

$$Q=ml$$

- Where $Q$ is the energy required to change state, $m$ is the mass of the substance and $l$ is the specific latent heat (the amount of energy needed to change the state of $1$kg of the substance without changing its temperature.
- When a substance is being heated, the energy it is given is "used" to heat the substance (giving the particles more kinetic energy). Once it reaches the melting/boiling point, the energy will no longer be used to increase the kinetic energy of the particles but to overcome the intermolecular forces between the molecules, changing the state of the substance.

# Fields & Their Consequences

## Gravitational Fields

- Affect anything with mass.
- Newton's law of gravitation - the magnitude of the gravitational force between 2 masses is directly proportional to the product of their masses and inversely proportional to the square of the distance between them.
- Always attractive.

|  | $\frac{1}{r^2}$ | $\frac{1}{r}$ | 
| :-: | :-: | :-: |
| **2 masses** | $F=\frac{Gm_1m_2}{r^2}$ | $WD =\frac{Gm_1m_2}{r}$ |
| **1 mass**| $g = \frac{GM}{r^2}$ | $V=\frac{GM}{r}$|

- $G$ is the gravitational constant, $WD$ is work done, $g$ is the gravitational field strength, $V$ is the potential at that point.
- Potential is defined as the work done per unit mass to move an object to that point from infinity (as at infinity it has 0 potential as the gravitational field does not affect it).

### Kepler's Third Law

$$T^2 \propto r^3$$

- The square of the orbital period of an object is proportional to the cube of the radius of the orbit.
- Derivation:

$$\frac{mv^2}{r}=\frac{GMm}{r^2}$$
$$v^2=\frac{GM}{r}$$

$$v=\omega r=\frac{2\pi r}{T}$$
$$v^2 = \frac{4\pi^2 r^2}{T^2}$$
$$\frac{GM}{r}=\frac{4\pi^2 r^2}{T^2}$$
$$T^2=\frac{4\pi^2}{GM} \times r^3$$

### Satellites

- The total energy of a satellite is equal to the sum of its kinetic energy and potential energy.
- The velocity required for an orbit can be derived from the equations for centripetal force and gravitational force.

$$\frac{GMm}{r^2}=\frac{mv^2}{r}$$
$$\frac{GM}{r}=v^2$$
$$v=\sqrt{\frac{GM}{r}}$$

- Satellites can be in (geo)synchronous orbits and geostationary orbits. A geosynchronous orbit is one in which the orbit period is the same as the rotational period of the object it is orbiting. A geostationary orbit is a geosynchronous orbit directly above the equator, so its always in the same position relative to the earth.
- Low-orbit satellites have smaller orbital periods and have a higher velocity. This is useful for monitoring the weather.

### Escape Velocity

 - The escape velocity is minimum velocity an object must be traveling at to escape the gravitational field at the surface of a mass. For the object to escape, its kinetic energy must be equal to its potential energy
-  Derivation:

$$\frac{1}{2}mv^2=\frac{GMm}{r}$$
$$v^2=\frac{2GM}{r}$$
$$v=\sqrt{\frac{2GM}{r}}$$

## Electric Fields

- Affect anything with charge

### Coulomb's Law &  other equations

- The equation for force is Coulomb's law.
- All of these equations are only valid for radial fields.

$$F=\frac{Q_1Q_2}{4\pi \varepsilon_0 r^2}$$

$$WD = \frac{Q_1Q_2}{4\pi \varepsilon_0 r}$$

$$E \textrm{ (electric field strength)} = \frac{Q}{4\pi \varepsilon_0 r^2}$$

$$V \textrm{ (potential)} = \frac{Q}{4\pi \varepsilon_0 r}$$

- The equations below are valid for uniform fields.

$$E=\frac{F}{Q}=\frac{V}{d}$$

- The force in the Coulomb's Law equation can be either positive or negative depending on the charges of the 2 point charges. If the force is negative, then it means it is attractive, if the force is positive, then its repulsive.
- The electrostatic forces between subatomic particles in the nucleus is much greater than the gravitational forces, this suggests the existence of another force (the strong nuclear force) which is attractive and keeps the nucleus together.

### Capacitance

- Capacitance is the charge stored per unit potential difference.
- Capacitors are usually made out of 2 parallel conductive plates separated by an insulating material (known as a dielectric).
- The energy stored by a capacitor is:

$$E=\frac{1}{2}QV$$

- Equation for charging a capacitor:

$$V=V_0(1-e^{\frac{-t}{RC}})$$

- Equation for discharging a capacitor:

$$V=V_0e^{\frac{-t}{RC}}$$

- Where $V$ is the potential difference between the 2 plates, $V_0$ is the maximum potential difference between the 2 plates, $t$ is time, $R$ is the resistance of the circuit, and $C$ is the capacitance of the capacitor (unit is Farads, $F$)

## Magnetic Fields & Electromagnetic Induction

- When a current passes through a wire, a magnetic field is induced.
- Magnetic Flux Density ($B$) is the same thing as the field strength.
- Force on a current-carrying wire:

$$F=BIL$$

- Force on a charged particle in a magnetic field:

$$F=BQv$$

- The force exerted on a particle is perpendicular to its motion, so $F=\frac{mv^2}{r}$
	- Combining the equation for the force on a charged particle with the equation for centripetal force:

$$BQv=\frac{mv^2}{r}$$
$$r=\frac{mv}{BQ}$$

- A cyclotron is made of 2 semi-circular electrodes  with a uniform magnetic field acting perpendicular to the plane the electrodes lie in. A high-frequency alternating voltage is applied between the electrodes, which causes any particle between the electrodes to accelerate in a spiral.
- Magnetic flux ($\phi$) describes the magnetic field lines passing through an area.

$$\phi = BAcos\theta$$

- Where $A$ is the area the field lines are passing through and $\theta$ is the angle the normal of the area makes to the field lines

$$N\Phi = BANcos\theta$$

- Where $N\Phi$ is the magnetic flux linkage, $B$ is the magnetic flux density, $A$ is the area, $N$ is the number of turns, and $\theta$ is the angle the normal of the area makes to the field lines.

### Electromagnetic Induction

- **Faraday's Law** - the magnitude of induced emf is equal to the rate of change of flux linkage
- **Lenz's Law** - the direction of induced current is opposite to the motion causing it

$$\varepsilon = \frac{\Delta N\Phi}{\Delta t}$$

$$\varepsilon =  BAN\omega sin(\omega t)$$

### Transformers

- A transformer is used to change the voltage of alternating current.
- In a step-up transformer increases the voltage across the secondary coil (More turns on the secondary coil than the primary)
- A step-down transformer decreases the voltage across the secondary coil (Less turns on the secondary coil than the primary)

# Nuclear Physics

## Radiation & Decay

### Radiation

- **Alpha ($\alpha$)**
	- $\alpha =\textrm{ } ^4_2He$ nucleus
	- Weak penetrative power
	- Highly ionising
	- Only emitted by nuclei with atomic number greater than 60
	- Cannot penetrate a piece of paper or a few millimetres of air
	- Used in smoke detectors, as the alpha particles cannot penetrate the smoke
	- $^X_Y Z=^{X-4}_{Y-2}W+^4_2\alpha$
- **Beta ($\beta$)**
	- $\beta^+$ or $\beta^-$ decay
		- Beta-plus decay is a proton decaying into a neutron, positron and electron-neutrino.
		- Beta-plus decay occurs in proton rich nuclei.
		- Beta-minus decay is a neutron decaying into a proton, electron and anti-electron-neutrino.
		- Beta-minus decay occurs in neutron rich nuclei.
	- Moderately penetrative
	- Moderately ionising
	- Used to monitor the thickness of aluminium foil as if its too thick the beta particles cannot penetrate it
	- Also used in PET scanning
- **Gamma ($\gamma$)**
	- Does not change the atomic number or atomic mass of a nucleus
	- Makes nucleus more stable by emitting a high-energy photon (gamma photon)
	- Highly-penetrative
	- Follows the inverse-square law
	- Used in medical imaging and cancer treatments
	- Used to sterilise medical equipment
	- Used to irradiate food to stop it from going bad
- Background radiation
	- Is always present
	- Comes from many sources
		- Radon gas
		- Bricks
		- Cosmic rays
		- Medical procedures

### Decay

- Decay is random and spontaneous so it cannot be predicted
- However at large scales (with millions of nuclei that could decay) we can estimate how many of them will have decayed after a certain time

$$\frac{\Delta N}{\Delta t} = -\lambda N$$

- The equation shows that the rate of decay is proportional to the number of nuclei
- This relationship can be re-written as:

$$N=N_0e^{-\lambda t}$$

- Activity is just another name for the rate of decay of a radioactive source.

$$A=\lambda N$$

### Rutherford Scattering

- Fired $\alpha$ particles at a thin gold sheet
- Most $\alpha$ particles passed straight through or were deflected at small angles, suggesting most of an atom is empty space.
- Some $\alpha$ particles were deflected at very large angles, suggesting that the nucleus is small (in relation to the size of an atom) and it is positively charged

## Fusion & Fission

### Fusion

- Two smaller nuclei combine to make a larger, more stable nucleus
- All nuclei have less mass than the mass of its constituent particles
- Nuclei release binding energy when formed
- Energy per nucleon is highest at iron
- So nuclei smaller than iron can undergo fusion and release energy
- Requires very high temperatures and pressures

### Fission

 - Splitting of a larger nucleus into 2 smaller daughter nuclei that are more stable
- The 2 daughter nuclei have a greater energy per nucleon than the parent nucleus
- This means a large amount of energy is released
- Also results in neutron being released which can induce other fission reactions

## Nuclear Reactors

- **Moderators**
	- Reduce the kinetic energy of neutrons so that they can be absorbed by the radioactive nuclei
	- Usually water or graphite
- **Control rods**
	- Absorbs neutrons to control the rate fission reactions
	- Usually boron or cadmium
- **Coolant**
	- Transfers heat away from the reactor to the heat exchanger
	- Must be a liquid with a low specific heat capacity
	- Usually water, helium or sodium
- **Shielding**
	- Reduces penetration of radiation into surroundings
	- Usually concrete

## Nuclei

### Nuclear Instability

- An N-Z graph shows the number of neutrons on the y-axis and the number of protons on the x-axis.
- The band of stability shows the values of protons and neutrons for which nuclei are stable.
- Above the band of stability, $\beta^-$ decay occurs
- Below the band of stability, $\beta^+$ decay occurs
- After Z=60, $\alpha$ decay occurs

### Nuclear Radius

- Electron diffraction experiment shows the size of a nucleus

$$sin\theta =1.22\frac{\lambda}{d}$$

- Liquid drop model
	- Assume the nucleus is a sphere of constant density
	- Volume is proportional to the number of nucleons

$$V=kA=\frac{4}{3}\pi r^3$$

- Rearranging for r gives:

$$r=\sqrt[3]{\frac{3kA}{4\pi}}$$
$$r=r_0A^{\frac{1}{3}}$$
$$r_0=1.05 \textrm{ fm}$$

### Half-life

- The half-life of a sample is the time taken for the number of radioactive nuclei to half.

$$A=\lambda N$$

$$\lambda = \frac{ln2}{T_{\frac{1}{2}}}$$

- Where $\lambda$ is the decay constant, and $T_{\frac{1}{2}}$ is the half-life in seconds.