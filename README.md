# Composite Design Optimization Projects

This repository contains a collection of mini‑projects demonstrating how scripting and optimisation can accelerate composite design workflows.  The examples cover everything from implementing and benchmarking optimisation algorithms in Python, to automating finite element analyses (FEA), to generating composite layups in Rhino/Grasshopper.  These projects are deliberately concise and self‑contained so you can use them as a starting point for your own research or teaching.

## Contents

| Project | Highlights | Technologies |
| --- | --- | --- |
| [`vat_optimizer`](vat_optimizer/) | Implements Classical Laminate Theory (CLT) to compute stiffness of variable–angle tow (VAT) laminates.  Demonstrates gradient‑based (BFGS) and metaheuristic (Differential Evolution) algorithms to optimise ply angles for maximum bending stiffness.  Benchmarks both approaches and produces a reproducible report. | Python, NumPy, SciPy |
| [`fea_automation`](fea_automation/) | Scripts a parametric finite element analysis for a one‑dimensional beam using Euler–Bernoulli theory.  Design variables (cross‑sectional areas) are optimised via gradient‑based and global search algorithms to minimise compliance.  Demonstrates how to assemble stiffness matrices, apply boundary conditions, and run batch simulations programmatically. | Python, NumPy, SciPy |
| [`design_exploration`](design_exploration/) | Contains a Rhino/Grasshopper script skeleton for generating variable–angle tow fibre paths over a rectangular panel.  The script is written in Python using `rhinoscriptsyntax` and outputs fibre geometry that can be used with Automated Fibre Placement (AFP) constraints.  Includes a placeholder Grasshopper file for further visual programming. | Python (RhinoScript), Grasshopper |

## Motivation

Three core themes are explored throughout these projects:

1. **Exploring and benchmarking optimisation algorithms** (metaheuristics, gradient‑based, hybrid) for composite design.
2. **Integrating optimisers into a Python–based toolchain coupled with Rhino/Grasshopper** for variable–angle tow (VAT) laminate design.
3. **Verifying results via FEA** and ensuring fair comparison through mesh‑independence and consistent post‑processing.

This repository provides concrete examples for each theme.  The code is deliberately concise and well‑documented so you can extend it or adapt it to your own research.  Feel free to fork this repository and build upon it!
