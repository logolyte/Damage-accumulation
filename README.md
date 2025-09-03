# Damage Accumulation Aging Simulation

This project simulates aging as a process of stochastic damage accumulation using differential equations. The model is based on the work of Karin et al. (2019) and is implemented in Python using Jupyter notebooks.

## Features

- Simulates damage accumulation and repair in organisms.
- Uses both single and two-damage-type models.
- Uses the Euler-Maruyama method for stochastic integration.
- Plots histograms of lifespans, survival curves, mortality, and average damage.
- Includes parameter sets for humans and mice, and simulates the effects of interventions.

## Main Equations

### Single Damage Type
$$
\\frac{dx}{dt} = \\eta t - \\beta \\frac{x}{x+\\kappa} + \\sqrt{2\\epsilon}\\xi
$$

### Two Damage Types
$$
\\begin{aligned}
\\frac{dA}{dt} &= \\alpha_1 t - \\beta_1 \\frac{A}{A + K_1} + \\sqrt{2 D_1} \\, \\xi \\\\
\\frac{dB}{dt} &= \\alpha_2 A - \\beta_2 \\frac{B}{B + K_2} + \\sqrt{2 D_2} \\, \\xi
\\end{aligned}
$$

## Parameters

- $\eta$, $\beta$, $\kappa$, $\epsilon$: Damage accumulation, repair, saturation, and noise parameters.
- For two-damage-type models: $\alpha_1$, $\beta_1$, $K_1$, $D_1$, $\alpha_2$, $\beta_2$, $K_2$, $D_2$.

See the notebook for specific values used for humans and mice.

## Usage

Open the Jupyter notebook `Damage accumulation.ipynb`. From this notebook, you can run all simulations.

## Requirements

All code was run with the versions specified below, and has not been tested with any other versions:

- Python 3.13
- numpy 2.2
- matplotlib 3.8
- multiprocess 0.7
```

## References

- Karin, O., et al. (2019). "A new model for the evolution of aging." *Nature Communications*, 10, 5075. [https://doi.org/10.1038/s41467-019-13192-4](https://doi.org/10.1038/s41467-019-13192-4)
- Yang, et al. (2025). Parameter values for human simulations. *Nature Communications*, 16, 57807. [https://doi.org/10.1038/s41467-025-57807-5](https://doi.org/10.1038/s41467-025-57807-5)
