# Computational Statistics

Coursework for the **Computational Statistics** course (Faculty of Mechanics and Mathematics, Taras Shevchenko National University of Kyiv, Computer Mathematics, 3rd year).

The repository contains graded lab assignments and in-class seminar notebooks. Everything is written in Python as Jupyter notebooks; explanations inside the notebooks are in Ukrainian.

## Repository structure

```
comp_stat/
├── Homework/                 # graded labs and homework
│   ├── lab1.ipynb            # Lab 1: point & interval estimation on real data
│   ├── Lab-2.ipynb           # Lab 2: MLE vs method of moments
│   ├── homework3.ipynb       # Box plots: quantile (Tukey) vs mean ± 1.96·std
│   ├── Lab3.ipynb            # Lab 3: two-sample test for equality of means
│   ├── Lab4.ipynb            # Lab 4: linear regression
│   └── data.csv              # dataset for Lab 1 (1000 rows)
└── Lab/                      # seminar notebooks
    ├── 01_python_and_libs.ipynb
    ├── seminar.ipynb
    ├── sem3.ipynb
    ├── Untitled.ipynb
    ├── Untitled_1.ipynb
    ├── sem10.ipynb
    └── chi2_for_complex.ipynb
```

## Homework

| Notebook | Topic | What is done |
|---|---|---|
| `lab1.ipynb` | Point and interval estimation | Descriptive statistics implemented by hand, exponential model, method of moments, quantile method, MLE, confidence intervals, dependence check on `data.csv` (`total`, `return`, `special_proposition`) |
| `Lab-2.ipynb` | Parameter estimation | MLE and method-of-moments estimators for reparametrized families (e.g. Exp(λ + 1/λ)), compared via Monte Carlo simulation |
| `homework3.ipynb` | Robust visualization | Tukey box plot vs `mean ± 1.96·std` box on N(0, 1) and Cauchy(0, 1) samples; stability across repeated samples |
| `Lab3.ipynb` | Hypothesis testing | Test for equality of two means with known variances, applied to real daily-loss data (General Staff of the Armed Forces of Ukraine reports) |
| `Lab4.ipynb` | Linear regression | Generating regressors and noise, least-squares fit, analysis of estimator behaviour |

## Seminars

| Notebook | Topic |
|---|---|
| `01_python_and_libs.ipynb` | NumPy basics: arrays, shapes, reshape, transpose |
| `seminar.ipynb` | Expectation and consistency of estimators (simulation) |
| `sem3.ipynb` | Location and scale estimation, box plots |
| `Untitled.ipynb` | Method of moments: U[0, b], Gamma distribution |
| `Untitled_1.ipynb` | Estimation for the binomial distribution B(n, p) |
| `sem10.ipynb` | Tests for the mean (known / unknown variance), type I and II error probabilities |
| `chi2_for_complex.ipynb` | χ² test on the Steam user-behaviour dataset |

## Requirements

- Python 3.10+
- Jupyter Notebook / JupyterLab
- `numpy`, `scipy`, `pandas`, `matplotlib`, `tqdm`

```bash
pip install numpy scipy pandas matplotlib tqdm jupyter
```

## Usage

```bash
git clone https://github.com/kyrylobatrak/comp_stat.git
cd comp_stat
jupyter lab
```

Open any notebook and run the cells top to bottom (**Run → Run All Cells**).

> **Note:** `Lab/chi2_for_complex.ipynb` reads `steam_data/steam-200k.csv`, which is not included in the repository. Download the *Steam Video Games* dataset (`steam-200k.csv`) and place it in `Lab/steam_data/` before running.

## Author

**Kyrylo Batrak** — [GitHub](https://github.com/kyrylobatrak) · [LinkedIn](https://www.linkedin.com/in/kyrylo-batrak-0b8749361)
