# Learning Data Science

Data science etudes -- explorations of statistical concepts through code.

Conformal prediction is the standout recent development: it provides distribution-free prediction intervals with guaranteed coverage -- no assumptions about the data-generating process. Chatterjee's Xi coefficient and distance correlation address a fundamental limitation of Pearson correlation: they detect arbitrary nonlinear associations, which matters for feature selection, independence testing, and understanding complex data relationships. The information-theoretic ML foundations connect Shannon entropy to generalization bounds and PAC-Bayes theory -- this is the theoretical frontier of understanding why deep learning works.

## About

This repository contains Jupyter notebooks that explore fundamental statistical concepts, with a focus on understanding how different measures capture relationships in data.

## Notebooks

### Pearson Correlation vs Mutual Information

[`pearson_correlation_coefficient_vs_mutual_information.ipynb`](pearson_correlation_coefficient_vs_mutual_information.ipynb) - Compares how Pearson correlation and mutual information capture dependence in bivariate normal data, inspired by Nassim Taleb

This notebook explores the relationship between Pearson correlation and mutual information:

- **Pearson Correlation**: Shows how correlation coefficient (rho) scales non-linearly -- the perceptual gap between rho=0.5 and rho=0.9 is much larger than between rho=0 and rho=0.5
- **Mutual Information**: Demonstrates how mutual information scales linearly with information content, providing a more intuitive measure of dependence
- **Comparison**: Visualizes bivariate normal distributions across both metrics to illustrate their differences

The notebook is based on [this tweet](https://twitter.com/nntaleb/status/1150457625877864450) by Nassim Taleb.

## Requirements

- Python 3.7+
- Jupyter
- NumPy
- Matplotlib

## Running

1. Install dependencies:
   ```bash
   pip install jupyter numpy matplotlib
   ```

2. Start Jupyter:
   ```bash
   jupyter notebook
   ```

3. Open `pearson_correlation_coefficient_vs_mutual_information.ipynb` and run the cells.

## License

See LICENSE file for details.

## Not yet reviewed

> These resources were recently found and have not been reviewed yet.

### Information Theory

- [Information Theory chapter -- Dive into Deep Learning (d2l.ai)](https://d2l.ai/chapter_appendix-mathematics-for-deep-learning/information-theory.html) - Interactive notebook covering entropy, KL divergence, mutual information
- [Probabilistic Machine Learning: An Introduction - Kevin Murphy (MIT Press, 2022, free)](https://probml.github.io/pml-book/book1.html) - 944-page textbook with Colab notebooks covering information theory and Bayesian reasoning

### Statistical Methods

- [Kernel Partial Correlation Coefficient (JMLR 2022)](https://www.jmlr.org/papers/volume23/21-493/21-493.pdf) - Nonparametric conditional dependence measure extending Pearson/MI comparisons
- [hyppo: Multivariate Hypothesis Testing Python Package](https://hyppo.neurodata.io/tutorials/independence.html) - Unified library for distance correlation, HSIC, MGC with tutorials
- [Causal Inference for the Brave and True - Matheus Facure](https://matheusfacure.github.io/python-causality-handbook/landing-page.html) - Free Python notebook handbook on DAGs, propensity scoring, heterogeneous effects

### Notable Notebook Collections

- [pytudes - Peter Norvig](https://github.com/norvig/pytudes) - Gold-standard exploratory Python notebooks on probability, puzzles, algorithms
- [Probably Overthinking It notebooks - Allen Downey (2023)](https://github.com/AllenDowney/ProbablyOverthinkingIt) - Base-rate fallacy, Simpson's paradox, distributional thinking with real datasets

### Correlation & Dependence

- [Semi-Distance Correlation (JASA 2024)](https://www.tandfonline.com/doi/abs/10.1080/01621459.2023.2284988) - Extends distance correlation to mixed categorical-continuous data
- [Copula models in Python using sympy](https://williamsantos.me/posts/2022/copula-from-scratch-with-sympy/) - From-scratch Gaussian and Archimedean copulas, good companion to Pearson/MI comparison

### Books

- [Probably Overthinking It - Allen Downey (2023)](https://www.amazon.com/Probably-Overthinking-Questions-Statistical-Decisions/dp/0226822583) - Data-first statistical reasoning exposing common traps; all code in open notebooks
- [Causal Inference in Python - Matheus Facure (O'Reilly, 2023)](https://www.oreilly.com/library/view/causal-inference-in/9781098140243/) - DiD, IV, synthetic control applied to industry problems

### Dependence Measures Beyond Pearson/MI (New)
- [Chatterjee's Xi Correlation in SciPy (scipy.stats.chatterjeexi, v1.15, 2024)](https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.chatterjeexi.html) - Rank-based asymmetric dependence measure detecting non-monotonic associations; now in SciPy
- [KDist: Kernel and Distance Methods for Statistical Inference - Zhang (R, 2025)](https://github.com/zhangxiany-tamu/KDist) - R package unifying HSIC, distance correlation, energy statistics, change-point detection, and conditional independence tests

### Information-Theoretic Approaches (New)
- [Information-Theoretic Foundations for Machine Learning - Jeon et al. (arXiv, 2024)](https://arxiv.org/abs/2407.12288) - 200+ page monograph unifying generalization, meta-learning, and misspecification through Shannon information theory
- [Mutual Information Estimation via Normalizing Flows - Butakov et al. (NeurIPS 2024)](https://arxiv.org/abs/2403.02187) - Maps data to tractable distribution for closed-form MI estimation with provable error bounds

### Conformal Prediction (New)
- [Introduction to Conformal Prediction with Python - Christoph Molnar (2023)](https://christophmolnar.com/books/conformal-prediction/) - Practical book with Jupyter notebooks on distribution-free uncertainty quantification for any ML model
- [Conformal Prediction Notebooks - Angelopoulos & Bates (GitHub, 2024)](https://github.com/aangelopoulos/conformal-prediction) - Hands-on notebooks applying conformal prediction to ImageNet, medical, toxic text, and tumor segmentation

### Books with Open Notebooks (New)
- [Think Stats 3rd Edition - Allen Downey (O'Reilly, 2025)](https://allendowney.github.io/ThinkStats/) - Major rewrite entirely in Jupyter notebooks; EDA, distributions, hypothesis testing, regression
- [Statistical Rethinking 2024 Course - Richard McElreath (GitHub, 2024)](https://github.com/rmcelreath/stat_rethinking_2024) - Full Bayesian modeling course with video lectures and code in R, Python/PyMC, Julia/Turing

### Fat Tails Notebooks (New)
- [Statistical Consequences of Fat Tails: Notebooks - MarcosCarreira (GitHub)](https://github.com/MarcosCarreira/StatisticalConsequencesOfFatTails) - Python/R/Mathematica notebooks reproducing every chapter of Taleb's Technical Incerto
- [fattails: Python Notebooks for Fat-Tailed Statistics - FergM (GitHub)](https://github.com/FergM/fattails) - CLT failure under fat tails, S&P500 geometric averages, power-law diagnostics

### Julia & Python Tools (New)
- [Julia for Data Analysis - Bogumil Kaminski (Manning, 2023)](https://www.manning.com/books/julia-for-data-analysis) - Hands-on guide to DataFrames.jl, time series, and predictive models; most current practical Julia data science book
- [dcor: Distance Correlation and Energy Statistics in Python - Ramos-Carreno & Torrecilla (SoftwareX, 2023)](https://github.com/vnmabus/dcor) - Efficient distance correlation, energy distance, and independence tests; natural extension of Pearson/MI comparison
