# Optimization of ASP Rehabilitation Scheduling through Machine Learning Predictions

[![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)](https://www.python.org/downloads/)
[![Pandas](https://img.shields.io/badge/Library-Pandas-150458?logo=pandas)](https://pandas.pydata.org/)
[![Scikit-Learn](https://img.shields.io/badge/ML-Scikit--Learn-F7931E?logo=scikit-learn)](https://scikit-learn.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

## 📌 Project Overview

This project represents the experimental thesis work dedicated to optimizing the **Rehabilitation Shift Scheduling** problem (**STR** — *Schedulazione dei Turni di Riabilitazione*). The goal is to integrate the expressive power of **Answer Set Programming (ASP)** with **Machine Learning** predictive models to estimate the number of possible assignments given the resources and clinical constraints of a specific day.

The main focus of the research involves engineering a complex dataset derived from raw JSON files, with particular attention to **Data Leakage** prevention and **Multicollinearity** management to improve the models' generalization capabilities.

---

## 🛠️ System Architecture

The workflow is divided into three main phases:

**1. Data Extraction & Cleaning**
Transformation of nested data (JSON) into a tabular format (CSV).

**2. Feature Engineering**
- Distinction between **A Priori** features (extracted from the `Board` object) and **A Posteriori** features (extracted from the `Agenda` object).
- Prevention of Data Leakage by eliminating variables known only after the ASP solver has completed the scheduling.

**3. Predictive Modeling**
Training regression models to estimate the target variable (`totalAssignments`).

---

## 📊 Results

| Model | MAE | RMSE | R² |
|-------|-----|----|----|
| Random Forest | TBD | TBD | TBD |
| XGBoost | TBD | TBD | TBD |
| TabPFN | TBD | TBD | TBD |

---

## 👨‍🎓 Author

**Matteo Mammoliti**

- 🏛️ University: University of Calabria (Unical), Department of Mathematics and Computer Science (DeMaCs)
- 🎓 Degree: Computer Science (*Informatica*)
- 👨‍🏫 Supervisor: Prof. Marco Maratea
- 👩‍🔬 Co-supervisor: Dr. Pierangela Bruno

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.
