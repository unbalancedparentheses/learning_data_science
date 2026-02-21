# datatudes

Data science études — explorations of statistical concepts through code.

# Not yet reviewed

> These resources were recently found and have not been reviewed yet.

### Information Theory
- [Information Theory chapter — Dive into Deep Learning (d2l.ai)](https://d2l.ai/chapter_appendix-mathematics-for-deep-learning/information-theory.html) - Interactive notebook covering entropy, KL divergence, mutual information
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

## About

This repository contains Jupyter notebooks that explore fundamental statistical concepts, with a focus on understanding how different measures capture relationships in data.

## Notebooks

### Pearson Correlation vs Mutual Information

**File:** `pearson_correlation_coefficient_vs_mutual_information.ipynb`

This notebook explores the relationship between Pearson correlation and mutual information:

- **Pearson Correlation**: Shows how correlation coefficient (ρ) scales non-linearly — the perceptual gap between ρ=0.5 and ρ=0.9 is much larger than between ρ=0 and ρ=0.5
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
