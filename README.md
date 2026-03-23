# 🚀 Spacecraft Solar Array Deployment Dynamics using Kane’s Method

This project reproduces key results from the paper: 

> **Modeling and Simulation of Spacecraft Solar Array Deployment**
> Wie, B., Furumoto, N., Banerjee, A. K., & Barba, P. M. (1986)

- Derived equations of motion using Kane’s method (SymPy)
- Simulated dynamics using SciPy ODE solvers
- Reproduced:
    - Figure 6 (INTELSAT-V)
    - Figure 8 (INSAT planar)
    - Figure 9a (INSAT free-base)

---

## 🧠 Technical Highlights

<table>
  <tr>
    <td align="center"><b>Paper</b></td>
    <td align="center"><b>Replication</b></td>
  </tr>
  <tr>
    <td><img src="results/fig6.png" width="100%"></td>
    <td><img src="results/fig6_replication.png" width="100%"></td>
  </tr>
</table>

<div align="center">
  <img src="results/fig8.png" width="45%" />
  <img src="results/fig8_replication.png" width="45%" />
  <p>
    <em>Left: Original Figure 8 | Right: Reproduced result</em>
  </p>
</div>

<div align="center">
  <img src="results/fig9a.png" width="45%" />
  <img src="results/fig9a_replication.png" width="45%" />
  <p>
    <em>Left: Original Figure 9a | Right: Reproduced result</em>
  </p>
</div>

---

## 📊 Results

- Multibody dynamics with:
    - Tree topology (INTELSAT)
    - Closed-loop constraints (INSAT)
- Symbolic → numerical pipeline
- Handling:
    - Nonlinear coupling
    - Constraint forces
    - Switching dynamics (slotted link)

---

## 🛠️ Stack

- Python
- SymPy (Kane’s equations)
- SciPy (integration)
- NumPy / Matplotlib

---

## 📚 References

- Wie, B. et al. (1986)
- Space Vehicles Dynamics and Control — B. Wie

---

## 🛰️ Contact

If you have questions or want to collaborate, feel free to reach out:
**Tomás Suárez**
Mechatronics Engineering Student
📧 [suareztomasm@gmail.com](mailto:suareztomasm@gmail.com)