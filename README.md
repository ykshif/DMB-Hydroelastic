# DMB-Hydroelastic
Hydroelastic analysis of large floating structures using discrete-module methods (DMB, DM-FEM, RODM)

# Hydroelastic Analysis Based on Discrete-Module Methods

This repository provides a teaching-oriented and research-consistent implementation of hydroelastic analysis for large-scale floating structures based on discrete-module approaches.

---

## 🌊 Overview

Hydroelastic analysis is essential for very large floating structures (VLFS), where structural flexibility interacts with wave-induced hydrodynamic loads.  

This repository demonstrates a simplified workflow using the **Discrete-Module-Beam (DMB)** concept, where a continuous structure is represented by:

- Discrete rigid modules  
- Equivalent beam-type structural connections  

The example is implemented in a single Jupyter Notebook for clarity and teaching purposes.

---

## 🧠 Methodological Framework

### 1. Discrete-Module-Beam (DMB) Method

The DMB method approximates a continuous floating structure as a chain of discrete modules connected by beam elements.

Core idea:

- Hydrodynamic forces are computed at the **module level**
- Structural continuity is enforced through **beam stiffness**
- The coupled system is solved in the **frequency domain**

This approach provides a balance between:

- Computational efficiency  
- Physical interpretability  
- Implementation simplicity  

---

### 2. Extensions of Discrete-Module Methods

The DMB method belongs to a broader family of discrete-module hydroelastic approaches.

#### (1) DM-FEM (Discrete-Module-Finite-Element Method)

- Combines module-based hydrodynamics with **finite element structural modeling**
- Allows more detailed structural representation
- Suitable for:
  - Complex structural layouts
  - Higher-fidelity deformation analysis

#### (2) RODM (Reduced-Order-Discrete-Module Method)

- Introduces **model order reduction** into discrete-module frameworks
- Retains dominant structural modes while reducing DOFs
- Particularly suitable for:
  - Large-scale systems
  - parametric studies
  - fast evaluation and optimization

---

## ⚙️ What This Repository Demonstrates

This notebook includes:

- Hydrodynamic coefficient loading or computation (Capytaine)
- Beam-based structural coupling
- Single-frequency RAO solution
- Deflection reconstruction
- Comparison with reference results

📌 The focus is on **clarity and reproducibility**, not on building a full engineering solver.

---

## 📊 Example Result

<img width="366" height="288" alt="image" src="https://github.com/user-attachments/assets/2edda636-d8e1-450c-b592-8261177c65f6" />

---

## 📌 Applications

Discrete-module hydroelastic methods are suitable for:

- Very Large Floating Structures (VLFS)
- Floating solar platforms
- Floating airports and infrastructure
- Modular floating systems
- Long-span floating bridges

They are particularly effective for:

> Structures dominated by global, beam-like deformation

---
## 📊 References

1. Shi, Y., & Wei, Y. (2025).  
   *Application of the Reduced-Order-Discrete-Module Hydroelastic Analysis for Offshore Floating Photovoltaic Systems.*  
   Ocean Engineering, 339, 121968.

2. Shi, Y., Wei, Y., & Chen, Z. (2025).  
   *Analysis of hydroelastic response and failure mechanisms of floating offshore photovoltaic under wind and wave.*  
   Ocean Engineering, 328, 121028.

3. Shi, Y., Wei, Y., Tay, Z. Y., et al. (2025).  
   *Frequency-domain approach of hydroelastic response for flexible offshore floating photovoltaic under combined wind and wave loads.*  
   Ocean Engineering, 323, 120565.

4. Shi, Y., Wei, Y., & Chen, Z. (2024).  
   *Development of Reduced-Order-Discrete-Module method for hydroelastic analysis of floating flexible structures.*  
   Journal of Fluids and Structures, 130, 104188.

5. Shi, Y., Wei, Y., Tay, Z. Y., et al. (2023).  
   *Hydroelastic analysis of offshore floating photovoltaic based on frequency-domain model.*  
   Ocean Engineering, 289, 116213.

## 🚀 Usage

Open the notebook:

```bash
DMB_hydroelastic_demo.ipynb


