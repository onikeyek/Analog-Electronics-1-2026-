## Diode Selection Justification – 12 V DC Input Protection

For the 12 V DC input protection circuit, the 1N5819 Schottky diode was selected as a suitable protection component. The diode is used in series with the supply to protect the circuit against reverse polarity connection.

**Voltage rating:**
The 1N5819 has a maximum repetitive reverse voltage (VRRM) of 40 V, which is safely above the nominal 12 V input voltage. This provides sufficient margin for voltage variations, noise, and minor transients that may occur in real power supplies.

**Current rating:**
The diode is rated for an average forward current of approximately 1 A, with higher surge current capability. This makes it suitable for low-power and moderate-power DC input applications. In the simulation, a 12 Ω load was used, resulting in a current close to 1 A at 12 V, which is within the diode’s safe operating limits.

**Forward voltage drop:**
As a Schottky diode, the 1N5819 has a lower forward voltage drop (typically 0.2–0.4 V) compared to standard silicon diodes. This reduces power loss and heat generation, making it more efficient for input protection where voltage headroom is important.

**Cost and availability:**
The 1N5819 is inexpensive, widely available, and commonly used in power protection circuits, making it a practical choice for real-world designs.

**Simulation results:**
LTspice DC sweep simulation from −15 V to +15 V confirms correct operation. For positive input voltages, the diode conducts and supplies the load with a small voltage drop. For negative input voltages, the diode blocks current flow, protecting the load from reverse polarity.
