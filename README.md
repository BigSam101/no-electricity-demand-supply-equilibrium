# Norway (NO1) Electricity Demand and Supply Equilibrium

This repository presents an empirical electricity market analysis of Norway’s NO1 price area using economic theory and econometric modelling techniques. The project estimates electricity demand and supply relationships, identifies market equilibrium outcomes, and analyses how weather conditions, fuel-related variables, and market fundamentals influence electricity prices and traded quantities.

The analysis combines structural market modelling with econometric methods commonly used in electricity market research, including Ordinary Least Squares (OLS), Instrumental Variables (IV/2SLS), and Generalized Method of Moments (GMM).

---

## Project Objectives

The main objectives of the project are to:

- Estimate electricity demand and supply curves for the NO1 market area
- Identify equilibrium electricity prices and quantities
- Analyse the effect of temperature and market conditions on electricity demand
- Address simultaneity and endogeneity in electricity market estimation
- Compare OLS, IV, and GMM estimation approaches
- Visualize market equilibrium and comparative statics

---

## Data

The project uses electricity market and economic data for Norway’s NO1 price area. The dataset includes variables such as:

- Electricity prices
- Electricity demand and supply
- Temperature
- Heating degree indicators
- CO₂ allowance prices
- Oil prices
- Reservoir levels
- Interest rates
- Weekend effects

Hourly observations are cleaned and prepared for econometric analysis.

---

## Methodology

### 1. Demand Estimation

Electricity demand is modelled as a function of:

- Electricity prices
- Heating demand driven by temperature
- Weekend effects

The analysis begins with OLS estimation before applying:

- Instrumental Variables (IV / 2SLS)
- Generalized Method of Moments (GMM)

to correct for endogeneity between prices and quantities.

The repository also includes:

- Weak instrument tests
- Hausman-Wu endogeneity tests
- Sargan overidentification tests
- Heteroskedasticity diagnostics

---

### 2. Supply Estimation

The supply side models electricity prices as a function of:

- Electricity generation
- CO₂ prices
- Interest rates
- Weather conditions

Alternative instrument specifications are explored to evaluate model robustness and instrument validity.

---

### 3. Market Equilibrium Analysis

Estimated demand and supply curves are combined to identify equilibrium outcomes under different market conditions.

The project examines how equilibrium changes under scenarios such as:

- Cold versus warm weather conditions
- Low versus high CO₂ prices
- Alternative econometric specifications

Comparative statics are used to illustrate shifts in market equilibrium.

---

## Repository Structure

```text
├── data/               # Raw and processed datasets
├── notebooks/          # Jupyter notebooks for analysis
├── figures/            # Generated plots and equilibrium figures
└── README.md
```

---

## Tools and Libraries

The project is implemented in Python using:

- pandas
- numpy
- matplotlib
- scipy
- statsmodels
- linearmodels

---

## Example Outputs

The repository includes:

- Estimated demand and supply curves
- Market equilibrium plots
- Instrument validity diagnostics
- Weak instrument tests
- GMM estimation results
- Weather-driven demand shift analysis
- CO₂-price-driven supply shift analysis

---

## Key Findings

The analysis highlights several important features of electricity markets:

- Electricity demand in Norway is strongly influenced by temperature conditions
- Endogeneity between prices and quantities leads to biased OLS estimates
- IV and GMM approaches provide more economically meaningful elasticity estimates
- Market equilibrium is highly sensitive to weather conditions and fuel-related costs

---

## Limitations

This project is intended as a simplified structural equilibrium analysis and abstracts from several real-world electricity market complexities, including:

- Transmission constraints
- Cross-border electricity trade
- Hydropower reservoir optimization
- Unit commitment constraints
- Renewable intermittency
- Zonal congestion effects

---

## Future Extensions

Possible future extensions include:

- Multi-zone Nordic electricity market analysis
- Dynamic hydropower modelling
- Renewable generation integration
- Time-varying elasticities
- Machine learning approaches for electricity market analysis
- Scenario-based stochastic modelling

---

## Author

Samuel Kumi  
MSc Applied Economics and Sustainability  
Norwegian University of Life Sciences (NMBU)
