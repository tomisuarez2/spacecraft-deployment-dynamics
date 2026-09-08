# Reproduction of Spacecraft Solar Array Deployment Dynamics using Lagrange and Kane’s Methods

This repository contains symbolic and numerical models developed to reproduce selected results from:

> **Modeling and Simulation of Spacecraft Solar Array Deployment**  
> Wie, B., Furumoto, N., Banerjee, A. K., & Barba, P. M. (1986)

The implementation follows exercises from the book:

> **Space Vehicle Dynamics and Control** — B. Wie

The models are implemented in Python using SymPy for symbolic mechanics and SciPy for numerical integration.

The main objective is to reproduce the deployment dynamics presented in the paper and to compare different formulations of the equations of motion, particularly Lagrange's method and Kane's method.

Lagrange's method theory:

> **Analytical Mechanics** - L. H. Hand & J. D. Finch 

Kane's method theory:

> **Dynamics, Theory and Applications** - T. R. Kane & D. A. Levinson

---

# Models

**INTELSAT-V**

The INTELSAT-V model represents the solar-array deployment dynamics using a tree-topology multibody system.

The implementation reproduces the deployment response presented in Figure 6 of Wie et al. (1986), following Exercise 1.27 from Space Vehicle Dynamics and Control.

**INSAT**

The INSAT model is represented as a planar closed-loop multibody system.

The model includes:

- Holonomic loop-closure constraints
- Dependent coordinates and generalized speeds
- Nonlinear coupling between the bodies
- Spring torques
- Symbolic derivation of the equations of motion

The implementation reproduces the planar deployment response presented in Figure 8 of Wie et al. (1986), following Exercise 1.28a.

---

## Methodology

The computational workflow is:

- Define the multibody geometry and reference frames.
- Define generalized coordinates and generalized speeds.
- Derive the kinematic constraints.
- Derive the equations of motion symbolically.
- Integrate the resulting nonlinear equations numerically.
- Compare the simulated response with the published results.

The symbolic derivations are performed using SymPy, while the numerical simulations use SciPy ODE solvers.

---

## Reproduced Results

The following figures from the paper are reproduced using the corresponding exercises:

- **Figure 6 (INTELSAT-V deployment)**  
  → Reproduced using *Exercise 1.27*

- **Figure 8 (INSAT planar model)**  
  → Reproduced using *Exercise 1.28a*

---

## Technical Highlights

The project explores:

- Multibody spacecraft dynamics
- Tree-topology systems
- Closed-loop multibody systems
- Holonomic constraints
- Dependent coordinates and generalized speeds
- Nonlinear dynamic coupling
- Symbolic-to-numerical workflows
- Lagrange's equations
- Kane's equations
- Numerical integration and simulation validation

---

## 🛠️ Stack

- Python
- SymPy (Kane’s equations)
- SciPy (integration)
- NumPy / Matplotlib

---

## ▶️ How to Run

Create and activate a virtual environment on Windows, then install the required dependencies:

```bash
python -m venv test_env
test_env\Scripts\activate
pip install -r requirements.txt
```

## Running the notebooks

With the virtual environment activated, launch Jupyter:

```bash
jupyter notebook
```

This will open Jupyter in your default web browser. From there, navigate to the repository folder and open any `.ipynb` notebook.

---

## 📊 Results

<div align="center">
  <img src="results/fig6.png" width="45%" />
  <img src="results/fig6_replication.png" width="45%" />
  <p>
    <em>Left: Original Figure 6 | Right: Reproduced result</em>
  </p>
</div>

<div align="center">
  <img src="results/fig8.png" width="45%" />
  <img src="results/fig8_replication.png" width="45%" />
  <p>
    <em>Left: Original Figure 8 | Right: Reproduced result</em>
  </p>
</div>

---

## 🛰️ Contact

If you have questions or want to collaborate, feel free to reach out:
**Tomás Suárez**
Mechatronics Engineer
📧 [suareztomasm@gmail.com](mailto:suareztomasm@gmail.com)