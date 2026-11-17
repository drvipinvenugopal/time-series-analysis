# 22AIE463 Time Series Analysis: Quarto Coursebook & Lab Manual

This repository contains the complete source code for the **Quarto Book** deliverable for course **22AIE463: Time Series Analysis** (Amrita Vishwa Vidyapeetham, Department of AI & Computer Science Engineering).

## Project Structure

```
time_series_quarto_book/
├── _quarto.yml                           # Quarto project configuration
├── index.qmd                             # Course syllabus, CO-PO mapping, evaluation, notations
├── references.bib                        # Prescribed textbooks & seminal citations (BibTeX)
├── references.qmd                        # Bibliography rendering page
├── README.md                             # Repository instructions
└── chapters/
    ├── 01_unit1_linear_models.qmd        # Unit 1: Stationarity, Ergodicity, ACF/PACF, AR, MA
    ├── 02_unit2_arima_var_garch.qmd      # Unit 2: ARMA, ARIMA, SARIMA, VAR, ARCH, GARCH
    ├── 03_unit3_nonlinear_statespace.qmd # Unit 3: Nonlinear models, ADF/KPSS, State-Space/Kalman
    └── 04_unit4_ml_dl_catastrophic.qmd   # Unit 4: ML, LSTM/TCN/Transformers, Catastrophic Tipping
```

## Prescribed Textbooks & Citations

All chapters feature strict in-text citations linking directly to the prescribed curriculum references:
- **Cryer & Chan (2008)**: *Time Series Analysis With Applications in R*, 2nd Ed., Springer `[@cryer2008time]`.
- **Shumway & Stoffer (2011)**: *Time Series Analysis and Its Applications with R examples*, 3rd Ed., Springer `[@shumway2011time]`.
- **Box, Jenkins, Reinsel, & Ljung (2016)**: *Time Series Analysis: Forecasting and Control*, 5th Ed., Wiley `[@box2016time]`.
- **Nielsen (2019)**: *Practical Time Series Analysis: Prediction with Statistics and Machine Learning*, O'Reilly `[@nielsen2019practical]`.
- **Seminal Literature**: Engle (1982), Bollerslev (1986), Kalman (1960), Scheffer et al. (2009).

## How to Render the Quarto Book

### Prerequisites
- Install **Quarto CLI** (version >= 1.3): [https://quarto.org/docs/get-started/](https://quarto.org/docs/get-started/)
- Python 3.9+ with `numpy`, `pandas`, `scipy`, `matplotlib`, `statsmodels`, `arch`

### Compilation Commands

To build the interactive HTML website book:
```bash
quarto render --to html
```
The compiled output is generated inside the `docs/` directory, which GitHub Pages serves as the course website.

To preview live in a browser with hot-reloading:
```bash
quarto preview
```

To compile a publication-grade PDF book (requires XeLaTeX/LuaLaTeX):
```bash
quarto render --to pdf
```
