# Mathematical Statistics in R

Exercises from the Mathematical Statistics course at Aarhus University.
Each file covers a topic area, combining LaTeX derivations with R implementations
that verify results by hand and then confirm with built-in functions.

## Structure

```
├── 01_distributions_and_eda.Rmd       Distributions, QQ plots, boxplot outliers
├── 02_inference.Rmd                   CIs, one/two-sample t-tests, power
├── 03_likelihood.Rmd                  MLE, profile likelihood, Bartlett's LRT
├── 04_simple_regression.Rmd           SLR, model checking, inverse prediction
├── 05_anova_and_multiple_regression.Rmd  One-way/two-way ANOVA, ANCOVA, backward selection
└── data/                              Datasets (not tracked — see below)
```

## Topics covered

| File | Key methods |
|---|---|
| Distributions & EDA | `curve`, `optimize`, histograms, QQ plots, skewness/kurtosis, Monte Carlo |
| Inference | One-sample t, paired t, two-sample t (equal var + Welch), F-test power |
| Likelihood | Joint log-likelihood, MLE derivation, profile likelihood, Bartlett's test |
| Simple Regression | LSE estimation, residual diagnostics, CI/PI bands, inverse prediction |
| ANOVA & Multiple Reg | One-way ANOVA, two-way ANOVA, ANCOVA, backward selection, common slope tests |

## Data

Place all `.csv` and `.txt` dataset files in the `data/` folder.
Files referenced across the exercises:

`Alluvialfan.txt`, `Iron.csv`, `Cuckoo.csv`, `Chatbot.csv`,
`Moore.csv`, `Testtime.csv`, `RhodesiaHighveld.csv`, `LambertBeer.csv`,
`Lion.csv`, `Darcy.csv`, `Flies.csv`, `Smartphone.csv`, `fishchrome.csv`,
`Fault.csv`, `Bear.csv`, `Firms.csv`, `Rfunctions-2.R`

## Rendering

```r
# Render all files to PDF
library(quarto)
quarto_render("01_distributions_and_eda.Rmd")
quarto_render("02_inference.Rmd")
quarto_render("03_likelihood.Rmd")
quarto_render("04_simple_regression.Rmd")
quarto_render("05_anova_and_multiple_regression.Rmd")
```

## Requirements

```r
install.packages(c("resampledata3"))
```
