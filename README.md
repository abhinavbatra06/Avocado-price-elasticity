# Overview 

This project leverages Bayesian Regression to determine the optimal pricing strategy for avocados. By modeling the price elasticity of demand, it provides insights into consumer behavior and helps identify profit-maximizing price points while accounting for uncertainty in predictions.

# Objectives
- Estimate Price Elasticity: Utilize Bayesian regression to quantify the relationship between price and sales volume.
- Quantify Uncertainty: Incorporate posterior distributions to capture the uncertainty in elasticity estimates.
- Predict Sales Volumes & profits: Use the Bayesian model to predict sales volumes for various price points.
- Propose Optimal Pricing: Identify the price that maximizes profits while explicitly considering uncertainty.

# Methods
- Bayesian Regression: A robust method that combines prior information with observed data to estimate price elasticity and its associated uncertainty.
- Profit Maximization: Simulate outcomes for different price points to identify the most profitable strategy.

# Dataset 
This project uses data from the Hass Avocado Board, downloaded in May 2018. The dataset aggregates weekly retail scan data for Hass avocados across multiple retail channels (grocery, mass, club, drug, dollar, and military) and includes information on both conventional and organic avocado sales.
Key columns in the dataset:
- Date: Observation date.
- AveragePrice: Average price of a single avocado.
- Type: Avocado type (conventional or organic).
- Year: Year of the observation.
- Region: City or region of the observation.
- Total Volume: Total number of avocados sold.
- 4046, 4225, 4770: Sales volumes for specific PLU codes.

Acknowledgements
- The dataset was compiled from publicly available data provided by the Hass Avocado Board. For more details, visit Hass Avocado Board's website.
- [Kaggle link](https://www.kaggle.com/datasets/neuromusic/avocado-prices)
  
