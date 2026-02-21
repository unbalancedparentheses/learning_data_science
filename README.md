# datatudes

Data science études — explorations of statistical concepts through code.

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
