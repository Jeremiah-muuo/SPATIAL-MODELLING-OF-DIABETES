# Diabetes Risk Mapping – Bayesian Spatial Modeling with INLA

**Where does diabetes hit hardest?**  
A Bayesian spatial modeling project in **R** using **INLA**. Compares **ICAR, BYM, Leroux, and spatial lag models** with beautiful county‑level maps for Kenya.

## 📌 Overview

This repository fits spatial regression models to diabetes prevalence data at the county level in Kenya.  
Using the **INLA** (Integrated Nested Laplace Approximations) package, we estimate and compare four spatial models:

- **ICAR** (intrinsic conditional autoregressive)  
- **BYM** (Besag‑York‑Mollié)  
- **Leroux** (generic1 with custom C‑matrix)  
- **Spatial lag model (SLM)**

Posterior mean, median, and credible intervals are mapped to visualise where diabetes risk is highest.

## 📁 Repository contents

- `Inla_modelling.R` – Main R script (data prep, adjacency matrix, model fitting, mapping)  
- `README.md` – Project documentation

## 🔧 Required R packages

```r
install.packages(c("INLA", "sf", "spdep", "ggplot2", "tmap", 
                   "dplyr", "tidyr", "gridExtra"))
