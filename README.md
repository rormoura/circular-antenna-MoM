# Method of Moments for a Circular Wire Antenna

## Overview

This repository contains a Python implementation of the Method of Moments (MoM) for the analysis of a thin circular wire antenna. The implementation discretizes the antenna into wire segments, builds the impedance matrix, solves the resulting linear system, computes the input impedance, and evaluates the radiation pattern.

The notebook also investigates the convergence of the input impedance as the number of discretization segments increases.

## Features

* Implementation of the Method of Moments for a thin circular wire antenna.
* Construction of the impedance matrix from the electric field integral equation.
* Solution of the linear system for the segment currents.
* Computation of the antenna input impedance.
* Evaluation of the normalized radiation pattern.
* Analysis of impedance convergence with different discretization levels.

## Numerical Model

The implementation defines the antenna geometry and electromagnetic parameters, including:

* Circular antenna radius.
* Wire radius.
* Electrical conductivity.
* Wavelength.
* Wave number.
* Angular frequency.
* Medium permeability.
* Medium permittivity.

The antenna is divided into `N` segments. Piecewise linear basis functions are used to assemble the impedance matrix. The resulting linear system is solved with NumPy's linear solver.

## Project Structure

```text
.
├── MoM_Ant_Circular_Código.ipynb
└── README.md
```

## Requirements

* Python 3
* NumPy
* SciPy
* Matplotlib

Install the required packages with:

```bash
pip install numpy scipy matplotlib
```

## Usage

Open the notebook and execute the cells in sequence.

The notebook performs the following steps:

1. Defines the antenna and electromagnetic parameters.
2. Constructs the impedance matrix.
3. Builds the excitation vector.
4. Solves the linear system.
5. Computes the input impedance.
6. Evaluates the radiation pattern.
7. Plots the convergence of the real and imaginary parts of the input impedance.

## Output

The notebook generates:

* Segment current distribution.
* Input impedance.
* Normalized radiation pattern.
* Convergence plots of the real and imaginary parts of the input impedance as the number of segments increases.

## License

This project is distributed under the MIT License.
