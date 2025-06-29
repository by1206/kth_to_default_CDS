# k-th to Default CDS Pricing using Copula and Monte Carlo Simulation

This project implements a pricing model for **k-th to default Credit Default Swaps (CDS)** using a **copula-based dependency structure** and **Monte Carlo simulation with low-discrepancy sequences**. It also models **piecewise constant hazard rates** for each reference entity, enabling flexible calibration to market spreads.

## 🔍 Overview

- **Instrument**: k-th to default CDS (a basket credit derivative)
- **Dependency model**: Gaussian copula
- **Numerical method**: Monte Carlo simulation with Sobol sequences
- **Default times**: Simulated from exponential distributions with piecewise constant hazard rates
- **Payout logic**: Based on the first *k* defaults in the basket
- **Programming Language**: Python 3.13
- **Notebook format**: Fully self-contained with explanations, visual outputs, and numerical validation

## 📦 Packages Used

This project was built and tested in **Python 3.13**. Key libraries include:

- `numpy` — vectorized numerical operations
- `scipy.stats` — copula construction and distribution tools
- `matplotlib` — for plotting and visualization
- `sobol_seq` — low-discrepancy sequence generation
- `pandas` — data manipulation
- `seaborn` — optional, for plot styling

To install all dependencies:

```bash
pip install -r requirements.txt
