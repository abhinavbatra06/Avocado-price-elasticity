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
- The dataset was compiled from publicly available data provided by the Hass Avocado Board. For more details, visit Hass Avocado Board's website and [Kaggle link](https://www.kaggle.com/datasets/neuromusic/avocado-prices)

# Results 
Results
1. [Model Insights](https://drive.google.com/file/d/1RKff-TGQjVrcYiGZahCmZO01zwru4W9Z/view?usp=drive_link)
- Intercept: The posterior distribution indicates a stable baseline value between 15 and 17, representing the scaled-down sales volume when the price is zero.
- Price Elasticity: The negative posterior mean for Avg_Price (~-5 to -6) confirms an inverse relationship between price and sales volume. A 1-unit increase in price leads to a decrease of approximately 5–6 units in scaled volume, aligning with economic theory.
- Uncertainty (sd): The standard deviation of the posterior distribution lies between 0.7 and 1.1, reflecting modest variability in the scaled sales volume across observations.

2. [Optimal Pricing Strategy](https://drive.google.com/file/d/1RLmVOYb3W4_1upy3Zbuc4GDb4dOYNw_i/view?usp=sharing)
- The forest plot reveals that profits peak at a price point of approximately 1.75, with both high expected profits and relatively narrow uncertainty.
- Lower price points (e.g., 0.5, 1.0) result in lower profits, while higher price points (e.g., 2.25, 2.5) show diminishing returns due to reduced sales volume.



  
