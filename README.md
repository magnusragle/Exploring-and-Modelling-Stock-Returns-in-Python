## Stock Returns Analysis with CAPM

Welcome to the **Stock Returns Analysis with CAPM** project. This repository provides tools and examples for exploring and modeling stock returns using Python, with a focus on the Capital Asset Pricing Model (CAPM).

---

## Table of Contents

- [Overview](#overview)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Data](#data)
- [Usage](#usage)
  - [Running the CAPM Analysis Script](#running-the-capm-analysis-script)
  - [Notebooks](#notebooks)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)

---

## Overview

This project demonstrates how to:

1. Download and preprocess historical stock price data (e.g., SPY, MSFT).
2. Compute returns adn descreptive statistics.
3. Apply the Capital Asset Pricing Model (CAPM) to estimate beta and alpha.
4. Visualize price series, returns, and regression results.
5. Experiment interactively within Jupyter notebooks.

Whether you are learning financial modeling or building your own analytics pipeline, this repository offers a solid starting point.

---

## Prerequisites

- Python 3.8 or higher
- `pandas`
- `numpy`
- `matplotlib`
- `statsmodels`
- `jupyterlab` or `notebook` (for running the notebooks)

You can install dependencies using pip:

```bash
pip install pandas numpy matplotlib statsmodels jupyterlab
```

---

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/stock-capm-analysis.git
   cd stock-capm-analysis
   ```
2. (Optional) Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate    # on Linux/macOS
   venv\Scripts\activate     # on Windows
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

---

## Data

This repository includes example historical price data for two tickers over the past 5 years:

- `HistoricalData_SPY_5Y.csv`: S&P 500 ETF (SPY)
- `HistoricalData_MSFT_5Y.csv`: Microsoft Corp. (MSFT)

Feel free to replace these with your own chosen market and stock tickers.

---

## Usage

### Running the CAPM Analysis Script

A standalone Python script `stock_market_CAPM_analysis.py` performs a CAPM regression on a user chosen stock and index:

The script will:

1. Load data from yfinance.
2. Compute daily returns.
3. Calculate the descriptive statistics.
4. Fit an OLS regression to estimate alpha and beta.
5. Output results to the console and save diagnostic plots (e.g., return scatterplot).

### Notebooks

Two Jupyter notebooks offer interactive exploration:

- `Exploring and Modelling Stock Returns in Python.ipynb`: A step-by-step guide to data loading, visualization, and CAPM theory.
- `Exploring and Modelling Stock Returns in Python_hardcoded.ipynb`: Similar analysis with hardcoded parameters for quick experimentation.

Launch them with:

```bash
jupyter lab    # or jupyter notebook
```

---

## Project Structure

```
├── HistoricalData_SPY_5Y.csv
├── HistoricalData_MSFT_5Y.csv
├── stock_market_CAPM_analysis.py
├── Exploring and Modelling Stock Returns in Python.ipynb
├── Exploring and Modelling Stock Returns in Python_hardcoded.ipynb
└── README.md
```

- **CSV Files**: Example price history data.
- **Python Script**: Automated CAPM analysis.
- **Notebooks**: Interactive tutorials.

---

## Contributing

Contributions are welcome! Feel free to:

- Submit issues for bugs or feature requests.
- Open pull requests for improvements (e.g., additional models, enhanced visualizations).

Please follow the standard GitHub flow:

1. Fork the repository.
2. Create a feature branch (`git checkout -b feature/YourFeature`).
3. Commit your changes (`git commit -m "Add new feature"`).
4. Push to your branch (`git push origin feature/YourFeature`).
5. Open a pull request.

---

## License

This project is released under the MIT License. See [LICENSE](LICENSE) for details.
