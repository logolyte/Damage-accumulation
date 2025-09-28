# Damage Accumulation Aging Simulation

This project simulates aging as a process of stochastic damage accumulation using differential equations. The model is based on the work of Karin et al. (2019) and Yang et al. (2025). It is implemented in Python using Jupyter notebooks.

## Features

- Simulates damage accumulation and repair in organisms.
- Uses both single and two-damage-type models.
- Uses the Euler-Maruyama method for stochastic integration.
- Plots histograms of lifespans, survival curves, mortality, and average damage.
- Includes parameter sets for humans and mice, and simulates the effects of interventions.

## Usage

Code, explanations and results are all found in the Jupyter notebook `Damage accumulation.ipynb`.

## Requirements

All code was run with the versions specified below, and has not been tested with any other versions:

- `Python`, 3.13.7
- `numpy`, 2.2.5
- `matplotlib`, 3.10.5
- `numba`, 0.61.2

## References

- Karin, O., et al. (2019). Senescent cell turnover slows with age providing an explanation for the Gompertz law. *Nature Communications*, 10, 5495. [https://doi.org/10.1038/s41467-019-13192-4](https://doi.org/10.1038/s41467-019-13192-4)
- Yang, et al. (2025). Compression of morbidity by interventions that steepen the survival curve. *Nature Communications*, 16, 3340. [https://doi.org/10.1038/s41467-025-57807-5](https://doi.org/10.1038/s41467-025-57807-5)
