# Temperature Effects on a Diode (1N4148)

The same diode-resistor circuit was simulated at 25 °C and 75 °C using the LTspice `.temp` directive. The forward voltage of the diode was observed at the output node while performing a DC sweep of the input source.

At 25 °C, the diode forward voltage is higher, while at 75 °C the forward voltage decreases by roughly 0.1 V. This occurs because increasing temperature increases carrier energy in the PN junction, reducing the voltage required for conduction. As a result, the diode conducts more easily at higher temperatures.

The diode current is also slightly higher at 75 °C for the same input voltage, since the lower forward voltage leaves more voltage across the series resistor. In reverse bias, diode leakage current increases significantly with temperature due to increased minority carrier generation.

This behavior is important in real electronic systems because temperature changes can shift bias points, increase leakage currents, and cause additional power dissipation. Designers must account for these effects in precision, low-voltage, and high-temperature applications.

