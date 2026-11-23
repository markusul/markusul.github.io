---
title: "Software"
hide_title: true
permalink: /software/
---

# Drug-Prot <a href="https://markus-ulmer.ch/DrugProt/"><img src="../images/software/drugprot-mark.png" align="right" style="height: 175px !important; width: auto; vertical-align: middle;" alt="DrugProt website" /></a>

[Drug-Prot](https://markus-ulmer.ch/DrugProt/) is a web application for exploring a large perturbation proteomics experiment in breast cancer.
In perturbation proteomics, cells are treated with drugs, and the abundance of thousands of proteins is measured afterwards.
The experiment behind Drug-Prot covers 18 breast cancer cell lines, 63 single drugs, and 59 drug pairs, with 5,078 proteins measured 6, 24, and 48 hours after treatment.

<a href="https://markus-ulmer.ch/DrugProt/"><img src="../images/software/drugprot-cover.jpg" alt="Two drugs act on a cell. Three rings show the protein expression at 6, 24 and 48 hours with the significant dependencies between them, and a panel shows the drug effects on one protein." style="width: 100%;" /></a>

You enter the proteins you care about, and Drug-Prot answers three questions.

- Which drugs change the abundance of these proteins, and at which time point?
- For which drug pairs does the combined effect differ from the sum of the two single-drug effects?
- Which other proteins change before or after yours?

Every answer comes with a p-value that is corrected only for the proteins you asked about.
A focused question therefore has more power than a search across all 5,078 proteins.
The drug effects have a causal interpretation, because the experimenter assigned the treatments.
The dependencies between proteins are associations ordered in time, and they serve to generate hypotheses.

Drug-Prot runs in the browser and needs no installation or access to the raw data.
Two built-in examples show what a query looks like, and the [preprint](https://doi.org/10.64898/2026.06.17.732914) describes the methods.

# SDModels <a href="https://markusul.github.io/SDModels/"><img src="../images/software/SDModels.png" align="right" style="height: 175px !important; width: auto; vertical-align: middle;" alt="SDModels website" /></a>

[![CRAN_Status_Badge](https://www.r-pkg.org/badges/version/SDModels)](https://CRAN.R-project.org/package=SDModels)
[![R-CMD-check](https://github.com/markusul/SDModels/actions/workflows/R-CMD-check.yaml/badge.svg)](https://github.com/markusul/SDModels/actions/workflows/R-CMD-check.yaml)
![CRAN Downloads overall](https://cranlogs.r-pkg.org/badges/grand-total/SDModels?color=brightgreen)

[SDModels](https://markusul.github.io/SDModels/) is an R package for estimating sparse nonlinear direct effects when unobserved confounders are present.
It builds on spectral deconfounding (Ćevid, Bühlmann, and Meinshausen (2020), Guo, Ćevid, and Bühlmann (2022)), a transformation of the data that reduces the bias from confounders affecting many covariates.
The estimates are reliable when the data has many covariates and the confounding is dense.
The package implements Spectrally Deconfounded Additive Models (SDAMs) (Scheidegger, Guo, and Bühlmann (2025)) and Spectrally Deconfounded Random Forests (SDForest) (Ulmer, Scheidegger, and Bühlmann (2026)).

![](../images/software/confModel.png)

# Ancestor Regression <a href="https://markusul.github.io/AncReg/"><img src="../images/software/AncReg.png" align="right" style="height: 175px !important; width: auto; vertical-align: middle;" alt="AncReg website" /></a>

[![CRAN_Status_Badge](https://www.r-pkg.org/badges/version/AncReg)](https://CRAN.R-project.org/package=AncReg)
[![R-CMD-check](https://github.com/markusul/AncReg/actions/workflows/R-CMD-check.yaml/badge.svg)](https://github.com/markusul/AncReg/actions/workflows/R-CMD-check.yaml)
![CRAN Downloads
overall](https://cranlogs.r-pkg.org/badges/grand-total/AncReg?color=brightgreen)

[AncReg](https://markusul.github.io/AncReg/) is an R package that tests for ancestral connections between variables, that is, whether one variable is a direct or indirect cause of another.
It covers linear structural equation models (Schultheiss and Bühlmann (2023)) and structural vector autoregressive models for time series (Schultheiss, Ulmer, and Bühlmann (2025)).
The tests control the rate of false causal discoveries asymptotically.
They draw their power from non-Gaussian distributions in the data.