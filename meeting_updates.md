# 24/10/2023

## Already done

Simulations for grid independency with 3-dimensional baffles and impeller's blade, turbulence model $k-\epsilon$ RNG:
Number of cells: 1M, 2M, 4M, 6M, 8M, 10M. 

Simulations for grid independency with 2-dimensional baffles and impeller's blade, turbulence model $k-\epsilon$ RNG:
Number of cells: 500k, 1M, 2M, 4M, 6M, 8M, 10M. 

## Currently running 

Simulations for grid independency with 3-dimensional baffles and impeller's blade, turbulence model Realizable $k-\epsilon$:
Number of cells: 1M, 2M, 4M, 6M, 8M, 10M. 

## Issues

The power number does not converge to the literature values. 
The power number calculated using torques differs from the one calculated using $\epsilon$, in values and in trend with respect to the number of cells.
Previous simulations with a number of cells $\sim$ 5M showed good agreement with the power number reported in the literature.

## To do

- [x] Plot the grid independences on the power number available.
    Include the values calculated both with $\epsilon$ and the ones calculated with the torque.

- [ ] Upload some of the previous simulations that were in agreement with the literature.

- [x] If possible, plot the grid independences on the velocity profile.

# 02/11/2023

## To do

- [x] Grid independence with First Order Upwind scheme only.

- [x] Check consistency with experimental data (Coroneo et al., 2011).

# 09/11/2023

## Results and Issues

First order schemes return very accurate values for the power number calculated using torques, but they are not in agreement with the expected velocity profiles.
There is high discrepancy between the power number calculated with torques and the one calculate with $\epsilon$.
The residuals are $\sim 10^{-6} - 10^{-5}$. 

Second order schemes present better results regarding $\epsilon$ and the power number calculated with it, but in general the power number obtained is less in agreement with the literature.
Also in this case the velocity profile does not follow the experimental/literature results.
The residuals are $\sim 10^{-4} - 10^{-3}$.

## To do

- [ ] Literature research for simulation of CSTR in similar conditions

- [ ] Simulation with 4M cells, 2nd order schemes, `slip` boundary condition for the `top_wall`.
    Plot velocity profile and power number.

- [ ] Increase non-orthogonal correctors

## Maybe

Consider the possibility of a transient simulation.
