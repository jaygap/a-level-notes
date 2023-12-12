## Current, Voltage and Resistance
### Current
The rate of flow of charge.
$$I = \frac{Q}{t}$$
Electrons flow from the negative terminal to the positive terminal.
Measured by an ammeter placed in series to other components.
### Voltage
The work done to move charge around the circuit, per unit charge.
$$V = \frac{W}{Q}$$
Measured by a voltmeter placed in parallel to other components.
### Resistance
How hard it is for current to flow.
$$R = \frac{V}{I}$$
## Ohm's Law
$$V = IR$$
## Kirchhoff's Laws
**Kirchhoff's 1st Law** - the current flowing into a junction is equal to the current flowing out of that junction
**Kirchhoff's 2nd Law** - in any complete loop in a circuit, the sum of all the voltages across components that supply electrical energy (cells, batteries) is equal to the sum of voltages across all other components in that loop

## Current-Voltage (I-V) Characteristics
A current-voltage (I-V) graph shows the relationship between the current and voltage of a component.
### Ohmic & non-Ohmic Conductors
An ohmic conductor is one that follows Ohm's Law ($V=IR$) which means that current and voltage have a linear relationship. At high voltages and currents this can break down, and so the component is no longer ohmic.
#### Diodes
A diode only allows current to flow in one direction.

![[Pasted image 20230918182227.png]]
This is only broken when the potential difference across the diode is too large, then current will flow even against the diode. The potential difference that causes this is called the breakdown voltage
#### Filament Bulbs
A filament bulb is a non-ohmic conductor. As current flows through the filament, it causes the filament's temperature to increase. This causes the resistance to increase which causes limits the current that can flow.

## Resistivity
Resistance is dependant on the material through which current is flowing. Resistivity is an intrinsic property of a material independent of its shape or size.
The equation for resistivity is:
$$\rho = \frac{RA}{L}$$
Where $\rho$ is the resistivity, $R$ is the resistance, $A$ is the cross-sectional area the current is flowing through, and $L$ is the length of material the current flows through.
## Types of resistors
### Thermistors
Thermistors come in 2 types, positive temperature coefficient and negative temperature coefficient.
In NTC (negative temperature coefficient) thermistors, increasing the temperature lowers the resistance. In PTC (positive temperature coefficient) thermistors the opposite is true.
### Light Dependent Resistor (LDR)
LDRs are made of semiconductors that are sensitive to light. As light intensity increases, its resistance decreases
## Determining the Resistivity of a Wire
### Equipment
- Wire
- Micrometre (to calculate the cross-sectional area of the wire)
- Ruler (to measure the length of the wire)
- Ammeter
- Voltmeter
- Cell
- Flying leads (to connect the wire to the rest of the circuit)
### Method
1. Measure the length of the wire
2. Use the micrometer to find the diameter of the wire at multiple points, calculate a mean and then use it to calculate the cross-sectional area
3. Construct the circuit so that the ammeter is in series with the wire and the voltmeter is connect to the circuit on either side of the wire.
4. Use the reading on the ammeter and voltmeter to calculate resistance
5. Substitute values into resistivity equation.
## Superconductors
A material that has a resistivity of zero at or below a critical temperature. This temperature is an inherent property of the material.
## Power
Power is the rate of energy transfer. The unit of power is Watts (W)
$$P = \frac{W}{\Delta t}$$
$$P = IV$$
$$P = I^2R$$
$$P = \frac{V^2}{R}$$
## EMF and Internal resistance
All power sources (cells, batteries, etc.) have a value of their EMF (electromotive force). EMF can be defined as the amount of energy supplied by the source per unit charge.
The terminal potential difference (potential difference between the positive and negative terminals of the cell/battery) is never equal to the EMF. This is because cells and batteries have an internal resistance.
The equation for resistivity is:
$$\varepsilon = V + Ir$$
$$\varepsilon = I(R + r)$$
## Potential Dividers
A potential divider is a combination of two resistors in series, which results in the potential difference in the circuit being split into a specific ratio. By changing the resistance of the resistors a desired voltage (V-Out) can be achieved. A component's potential difference as a fraction of the total EMF must be equal to its resistance as a fraction of the total resistance.
$$\frac{V}{\Sigma \varepsilon} = \frac{R_1}{\Sigma R}$$
