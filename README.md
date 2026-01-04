
# Numerical Modeling - Practical Work

This repository contains the solution to the Practical Work of the subject **Numerical Modeling (CB051)**, corresponding to the first quarter of 2025 at the Faculty of Engineering of the University of Buenos Aires. The project focuses on the numerical resolution of initial value problems for vibratory systems, specifically the mass-spring-damper model, addressing both linear and nonlinear cases.

## Objectives

- Implement and compare numerical methods (Explicit Euler and Runge-Kutta of order 2) to solve second-order ordinary differential equations.
- Analyze the stability and accuracy of these methods based on the step size (h) and the relative damping coefficient (ζ).
- Validate numerical solutions against analytical solutions for the linear case.
- Extend the analysis to the nonlinear case (Duffing oscillator) and study qualitative behaviors such as periodic oscillations, damped or chaotic.
- Generate graphs and reports to visualize and compare results.

## Repository Structure

- **`apuntes/`**: Contains the practical work assignment (`consigna.md`), which details the objectives, physical models, and specific assignments.
- **`metodos/`**: Implementations of numerical methods in Python.
  - `euler_explicito.py`: Explicit Euler method.
  - `RK2.py`: Runge-Kutta method of order 2.
  - Other files related to additional methods if any.
- **`corridas_numericas/`**: Results of numerical simulations for different cases (underdamped, critically damped, overdamped) and h values. Text files with tabular data.
- **`resultados/`**: Additional graphs and analyses generated from the data.
- **`main.py`**: Main script to run simulations.
- **`generar_graficos.py`**: Script to generate graphs from results.
- **`informe.tex`**: Final report in LaTeX, including theoretical analysis, empirical results, comparisons, and conclusions.

## Installation and Execution

### Prerequisites

- Python 3.x
- Virtual environment (recommended)

### Environment Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/EnriHeller/modelacion_numerica_TP.git
   cd modelacion_numerica_TP
   ```

2. Create and activate a virtual environment:
   ```bash
   python -m venv .venv
   source .venv/bin/activate  # On Windows: .venv\Scripts\activate
   ```

3. Install dependencies (if there's a `requirements.txt`, otherwise install numpy and matplotlib manually):
   ```bash
   pip install numpy matplotlib
   ```

### Run Simulations

- To run the main simulations:
  ```bash
  python main.py
  ```

- To generate graphs:
  ```bash
  python generar_graficos.py
  ```

Results will be saved in the `corridas_numericas/` and `resultados/` folders.

### Compile the Report

To compile the report into PDF:
```bash
pdflatex informe.tex
```

Make sure LaTeX is installed (e.g., TeX Live).

## Authors

- **Enrique Heller**
- **Other collaborator** (if applicable, based on the report: Heller, Zaton)

## References

- Practical work assignment: `apuntes/consigna.md`
- Complete report: `informe.tex`

This project demonstrates the practical application of numerical methods in engineering, highlighting the importance of stability and accuracy in computational simulations.