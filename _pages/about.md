---
permalink: /
title: "About me"
excerpt: "PhD student in statistics at ETH Zürich, working on perturbation data science from a statistical and causal perspective."
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a PhD student at the [Seminar for Statistics at ETH Zürich](https://math.ethz.ch/sfs), supervised by [Prof. Peter Bühlmann](https://people.math.ethz.ch/~peterbu/).
My research focuses on perturbation data science, which I approach from a statistical and causal perspective.

A perturbation experiment measures a system, such as cancer cells, under different interventions, such as drugs.
The goal behind such experiments is to find good interventions, for example, a drug combination that stops a tumor from growing.
This is a causal question, because it asks what will happen when we act on the system, not what tends to occur together.
Perturbation data is a natural place to answer it, since the experimenter sets the interventions.
I develop methods that answer such questions with quantified uncertainty.
I work on three questions about interventional data.

* **Inference about observed perturbations.** Which drugs change which proteins, and which drug pairs interact? [Drug-Prot](/software/) answers these questions for a perturbation proteomics experiment in breast cancer.
* **Prediction in new perturbations.** A model should still predict well when the data comes from a perturbation it has not seen. [Anchor Forests](https://markus-ulmer.ch/SDModels/articles/AnchorForest.html) regularize a random forest so that its predictions stay stable across perturbations, in the sense of distributional robustness.
* **Prediction of new perturbations.** Which untested drug pairs will interact, and which pair should be measured next? My current work extrapolates interaction patterns from a few measured pairs and uses them to choose the next experiment, since the number of possible combinations is far too large to measure them all.

The third question is my current focus.

Earlier in my PhD, I worked on two problems in causal inference, spectral deconfounding for nonlinear models ([SDModels](https://markusul.github.io/SDModels/)) and ancestor regression for time series ([AncReg](https://markusul.github.io/AncReg/)).
Both are available as R packages on CRAN.

Before ETH, I was a research assistant at the [Institute of Data Analysis and Process Design at ZHAW](https://www.zhaw.ch/en/engineering/institutes-centres/idp), where I worked on anomaly detection and predictive maintenance with [Dr. Lilach Goren Huber](https://www.zhaw.ch/en/about-us/person/gorn).