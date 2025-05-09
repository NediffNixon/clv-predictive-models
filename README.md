# Customer Lifetime Value Prediction with Darts and dunnhumby Dataset

[![Darts](https://img.shields.io/badge/Darts-Time_Series_ML-orange.svg)](https://unit8co.github.io/darts/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> **Note**: This project is in the early development stage. Currently working on data exploration and feature engineering.

## Project Overview

This project aims to build an advanced Customer Lifetime Value (CLV) prediction model using the dunnhumby dataset (The Complete Journey). The approach combines traditional probabilistic CLV modelling techniques with time series forecasting powered by the Darts library to create a more accurate and actionable CLV prediction system.

CLV prediction is critical for retail businesses to:
- Identify high-value customers for personalized retention strategies
- Optimize marketing spending based on expected returns
- Improve resource allocation across the customer base
- Forecast future revenue streams with greater accuracy

## Dataset

The project uses the [The Complete Journey dataset](https://www.dunnhumby.com/source-files/), specifically:

1. **The Complete Journey** - Contains household-level transactions over two years from approximately 2,500 households who are frequent shoppers at a retailer. Includes demographic information and marketing campaign history.

This dataset provide comprehensive information about purchase patterns, customer attributes, campaign responses, and product categories - offering an excellent foundation for CLV modeling.

## Approach

The project takes a hybrid approach to CLV prediction:

1. **Probabilistic Models**
   - BG/NBD (Beta-Geometric/Negative Binomial Distribution) for purchase frequency
   - Gamma-Gamma model for monetary value prediction

2. **Time Series Forecasting with Darts**
   - Utilizing advanced forecasting models (NBEATS, RNNs, TCNs)
   - Incorporating seasonal patterns and promotional effects
   - Leveraging multi-series training capabilities

3. **Hybrid Integration**
   - Combining insights from both modeling approaches
   - Creating customer-specific predictions based on purchase history
   - Accounting for temporal factors that influence CLV

## Project Structure

```
clv-prediction-models/
├── data/                      # Data directory (not included in repo)
│   ├── raw/
├── dashboards/                # Result dashboards (future development)
├── docs/
│   ├── dunnhumby - The Complete Journey User Guide.pdf
├── notebooks/                 # Jupyter notebooks for analysis
│   ├── 01_data_exploration.ipynb    # Current stage
│   └── ... (planned)
├── src/                       # Source code (future development)
├── environment.yml           # Dependencies
├── LICENSE                   # MIT License
└── README.md                  # Project documentation
```

## Current Progress

- [x] Project setup and initial exploration
- [ ] Feature engineering and RFM analysis
- [ ] Probabilistic CLV model implementation
- [ ] Time series model implementation with Darts
- [ ] Hybrid model development and evaluation
- [ ] Customer segmentation based on CLV
- [ ] Interactive dashboard for CLV insights

## Installation

```bash
# Clone this repository
git clone https://github.com/nediffnixon/clv-predictive-models.git
cd clv-predictive-models

# Create and activate conda environment
conda env create -f environment.yml
conda activate clv_prediction_env
```

## Usage

To explore the current stage of development:

```bash
# Launch Jupyter notebook
jupyter notebook notebooks/01_data_exploration.ipynb
```

## Future Work

- Implement comprehensive RFM analysis
- Develop BG/NBD and Gamma-Gamma models for traditional CLV prediction
- Create time series models with Darts to capture temporal patterns
- Integrate models for hybrid CLV prediction approach
- Build interactive dashboard for CLV insights
- Evaluate different segmentation approaches based on CLV

## Dependencies

- pandas
- numpy
- matplotlib
- seaborn
- darts
- pymc-marketing
- scikit-learn
- streamlit (for future dashboard)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [dunnhumby](https://www.dunnhumby.com/) for providing the dataset
- [Darts](https://unit8co.github.io/darts/) team for the time series library
- [PyMC-Marketing](https://www.pymc-marketing.io/) for probabilistic marketing models

## Contact

For questions or collaboration, please open an issue in this repository.
