# Lab 2 for CEE 4530


#### Team 10: Victor Khong & Jacqueline Wong ####

```python
from aguaclara.core.units import unit_registry as u
import aguaclara.research.environmental_processes_analysis as epa
from scipy import optimize
import numpy as np
import matplotlib.pyplot as plt
import pandas as pd
```
---
Use CMFR equation to find ANC of the samples

- Graph should go to -0.001
- Should delete comments in data file for lab

---

$K_1 = 10^{-6.3}, \text{ }K_2 = 10^{-10.3}, \text{ }
K_H = 10^{-1.5} \text{ mol L}^{-1} \text{atm}^{-1}, \newline P_{CO_2}=10^{-3.5} \text{ atm}, \text{ }K_w = 10^{-14}$

<b>1. Plot measured pH of the lake versus dimensionless hydraulic residence time (t/θ).</b>

<b>2. Assuming that the lake can be modeled as a completely mixed flow reactor and that ANC is a conservative parameter, equation (25) can be used to calculate the expected ANC in the lake effluent as the experiment proceeds. Graph the expected ANC in the lake effluent versus the hydraulic residence time (t/θ) based on the completely mixed flow reactor equation with the plot labeled (in the legend) as conservative ANC.</b>

$${ANC}_{{0}} {\; }=\left[{ANC}_{out} - ANC_{in} \cdot \left(1 - {\mathop{e}\nolimits^{-t/\theta}} \right)\right]{\mathop{e}\nolimits^{t/\theta}}$$

<b>3. If we assume that there are no carbonates exchanged with the atmosphere during the experiment, then we can calculate ANC in the lake effluent by using equation (14) describing the ANC of a closed system. Calculate the ANC under the assumption of a closed system and plot it on the same graph produced in answering question #3 with the plot labeled (in the legend) as closed ANC.</b>

$$ANC=C_T \left(\alpha_1 +2\alpha_2 \right)+\frac{K_w}{\left[H^+ \right]} - \left[H^+ \right]$$

<b>4.If we assume that there is exchange with the atmosphere and that carbonates are at equilibrium with the atmosphere, then we can calculate ANC in the lake effluent by using equation (18) describing the ANC of an open system. Calculate the ANC under the assumption of an open system and plot it on the same graph produced in answering question #3 with the plot labeled (in the legend) as open ANC.</b>

$$ANC=\frac{P_{CO_2} K_H }{\alpha_0 } (\alpha_1 +2\alpha_2 ) + \frac{K_w }{\left[H^+ \right]} - \left[H^+ \right]$$

<b>5. Analyze the data from the second experiment and graph the data appropriately. What did you learn from the second experiment?</b>