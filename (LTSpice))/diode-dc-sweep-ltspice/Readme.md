## Diode DC Sweep Analysis (Ideal vs Real Diode)

This project analyzes a simple diode circuit using LTspice by comparing an ideal diode model with a practical diode model (1N4148). The circuit consists of a DC voltage source swept from 0 V to 15 V, a 1 kΩ series resistor, and a diode connected from the output node to ground. A DC sweep analysis was performed for both cases to observe voltage and current behavior.

## Ideal Diode Model

The ideal diode was implemented using a voltage-controlled switch with very low on-resistance and zero turn-on threshold. In this case, the diode conducts immediately for any positive input voltage. The simulation results show a linear current–voltage relationship, where the current increases proportionally with the input voltage according to Ohm’s law. The output voltage remains approximately 0 V because the ideal diode has no forward voltage drop.

## Practical Diode Model (1N4148)

For the practical diode, a standard 1N4148 silicon diode model was used. The simulation shows that the diode does not conduct significantly until the forward voltage reaches approximately 0.6–0.7 V. Once conduction begins, the output voltage is clamped near this forward voltage, and the current increases as the input voltage rises. The current–voltage relationship is nonlinear at low voltages due to the diode’s PN-junction characteristics.

## Comparison and Discussion

The main difference between the two models is the turn-on voltage and current behavior. The ideal diode has zero turn-on voltage and no power loss, while the real diode exhibits a forward voltage drop and dissipates power. Ideal diode models are useful for simplifying circuit analysis and building intuition during early design stages. However, they become inaccurate in low-voltage circuits, power calculations, and precision applications where real diode characteristics must be considered.
