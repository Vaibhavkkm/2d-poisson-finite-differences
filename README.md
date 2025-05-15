# 2D Poisson Equation Solver

This project provides a comprehensive numerical solution to the **2D Poisson problem** over a square domain, with a focus on understanding and comparing the performance of various linear system solvers. It is a numerical analysis assignment for the University of Luxembourg.

## Overview

The Poisson equation is central in physics and engineering (e.g., electrostatics, fluid mechanics, heat conduction). This repository contains Python code to:

- **Discretize the 2D Poisson equation** using the finite difference method (FDM)
- **Implement and validate the solver** using an exact test solution
- **Analyze solver accuracy and convergence**
- **Compare direct and iterative solvers** for the resulting linear system, using both dense and sparse matrix approaches

## Main Features

1. **Finite Difference Discretization**
   - Uniform grid creation over the square domain Ω = {(x, y) | 0 ≤ x ≤ 1, 0 ≤ y ≤ 1}
   - Homogeneous Dirichlet boundary conditions (u = 0 on boundary)
   - Assembly of the discrete Laplacian matrix and right-hand side

2. **Validation and Error Analysis**
   - Validation using the known solution u(x, y) = sin²(πx) sin²(πy)
   - Calculation of the corresponding source term f(x, y)
   - Evaluation of solver accuracy (relative error in maximum norm)
   - Convergence plot in log-log scale

3. **Solving the Linear System**
   - **Direct Methods**
     - Dense and sparse matrix representations
     - Use of `scipy.sparse` for memory-efficient computation
     - Timing and performance comparison of dense vs. sparse solvers
   - **Iterative Methods**
     - Implementation of Jacobi, Gauss-Seidel, and SOR algorithms
     - Theoretical analysis of convergence (eigenvalues, convergence radius)
     - Residual and iteration count analysis for different grid sizes and methods
     - Visualization of residual decrease and computational performance



## Results

The project includes code and visualizations for:

- Solution accuracy and convergence behavior
- Performance comparison of direct and iterative solvers
- Detailed comments and explanations for educational purposes

---

**For academic use.**  
Feel free to fork, modify, and use for learning or research!
