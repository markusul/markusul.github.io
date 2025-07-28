---
title: ""
permalink: /software/
---

# SDModels <a href="https://markusul.github.io/SDModels/"><img src="../images/software/SDModels.png" align="right" height="175" alt="SDModels website" /></a>

[![CRAN_Status_Badge](https://www.r-pkg.org/badges/version/SDModels)](https://CRAN.R-project.org/package=SDModels)
[![R-CMD-check](https://github.com/markusul/SDModels/actions/workflows/R-CMD-check.yaml/badge.svg)](https://github.com/markusul/SDModels/actions/workflows/R-CMD-check.yaml)
![CRAN Downloads overall](https://cranlogs.r-pkg.org/badges/grand-total/SDModels?color=brightgreen)

 [Spectrally Deconfounded Models (SDModels)](https://markusul.github.io/SDModels/) is a package with methods to
screen for and analyze non-linear sparse direct effects in the presence
of unobserved confounding using the spectral deconfounding techniques
(Ćevid, Bühlmann, and Meinshausen (2020), Guo, Ćevid, and Bühlmann
(2022)). These methods have been shown to be a good estimate for the
true direct effect if we observe many covariates, e.g., high-dimensional
settings, and we have fairly dense confounding. Even if the assumptions
are violated, it seems like there is not much to lose, and the SDModels
will, in general, estimate a function closer to the true one than
classical least squares optimization. SDModels provides software for
Spectrally Deconfounded Additive Models (SDAMs) (Scheidegger, Guo, and
Bühlmann (2025)) and Spectrally Deconfounded Random Forests
(SDForest)(Ulmer, Scheidegger, and Bühlmann (2025)).

![](../images/software/confModel.png)

# Ancestor Regression <a href="http://www.markus-ulmer.ch/AncReg/"><img src="../images/software/AncReg.png" align="right" height="175" alt="AncReg website" /></a>

[![CRAN_Status_Badge](https://www.r-pkg.org/badges/version/AncReg)](https://CRAN.R-project.org/package=AncReg)
[![R-CMD-check](https://github.com/markusul/AncReg/actions/workflows/R-CMD-check.yaml/badge.svg)](https://github.com/markusul/AncReg/actions/workflows/R-CMD-check.yaml)
![CRAN Downloads
overall](https://cranlogs.r-pkg.org/badges/grand-total/AncReg?color=brightgreen)

[Ancestor Regression (AncReg)](https://markusul.github.io/AncReg/) is a package with methods to test for
ancestral connections in linear structural equation models (C.
Schultheiss and Bühlmann (2023)) and structural vector autoregressive
models (Christoph Schultheiss, Ulmer, and Bühlmann (2025)). Ancestor
Regression provides explicit error control for false causal discovery,
at least asymptotically. To have power, however, it relies on
non-Gaussian distributions.