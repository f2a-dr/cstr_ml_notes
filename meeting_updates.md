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
Previous simulations with a number of cells $\similar$ 5M showed good agreement with the power number reported in the literature.

## To do

[ ] Plot the grid independences on the power number available.
    Include the values calculated both with $\epsilon$ and the ones calculated with the torque.

[ ] Upload some of the previous simulations that were in agreement with the literature.

[ ] If possible, plot the grid independences on the velocity profile.
