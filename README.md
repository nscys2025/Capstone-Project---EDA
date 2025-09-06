### Project Title
Proactive Prediction of Electricity Shortages Using Renewable Generation and Demand Data

**Author**
Chan-Young Song

#### Executive summary
This project investigates the feasibility of proactively planning for electricity shortages by leveraging multi-year, high-frequency data on solar and wind energy generation alongside electricity demand in California. Using a combination of exploratory data analysis and predictive modeling, the study identifies key patterns and risk factors that precede shortages. Results will demonstrate that historical weather and production data can be used to anticipate supply-demand gaps, supporting smarter grid management and more resilient integration of renewable energy. These insights can inform utilities and policymakers in optimizing storage, backup generation, and demand-side strategies to minimize blackout risks and ensure reliable electricity delivery.

#### Rationale
As renewable energy sources like solar and wind become a larger part of the electricity grid, their inherent variability introduces new challenges for maintaining a stable and reliable power supply. Traditional energy sources can be dispatched on demand, but renewables depend on weather and time of day, making shortages more likely if not properly managed. By analyzing historical data on renewable generation and electricity demand, we can identify patterns and anticipate periods of potential shortage. This proactive approach enables utilities and policymakers to optimize grid operations, plan for storage and backup resources, and implement demand-side strategies, ultimately reducing blackout risks and supporting a resilient transition to clean energy.

#### Research Question
Can electricity shortages be proactively predicted using multi-year data on solar and wind power generation, weather, and electricity demand?

#### Data Sources
[Renewable Energy and Electricity Demand Time Series Dataset with Exogenous Variables at 5-minute Interval - Mendeley Data Links to an external site.](https://data.mendeley.com/datasets/fdfftr3tc2/1): Data collected by California Independent System Operator (CAISO) and the National Renewable Energy Laboratory (NREL).

#### Methodology
- CRISP-DM for overall process framework
- EDA - will study and analyze the data and clean up the data (data preprocessng).
- Feature Engineering - to introduce more meaningful attributes for training
- Classification model - Logistic Regression/ Decision Tree to identify potential shortage windows.
- Regularization - to prevent overfitting and improve generalization
- Scaling - to ensure the features are equally contributing to training.
- Forecasting model - ARIMA/SARIMA and Prophet for time-series prediction for electricity demand and supply
- Grid Search & Cross Validation - to find best hyper parameters and reduce the overfitting
- Visualization - using plots to understand the data better and show results of modeling


#### Results
- Shortages are Predictable: The analysis showed that electricity shortages can be proactively predicted using historical data on renewable generation, weather, and demand. Logistic regression provided a reasonable baseline for identifying shortage periods.
- Key Predictors Identified: Features such as season, temperature, hour of day, humidity, and wind speed were found to be the most important predictors of shortages, indicating recurring patterns that precede supply-demand gaps.
- Seasonal and Temporal Patterns: Shortages were most likely to occur during summer months and in the early evening hours (6–8pm), when demand peaks and renewable generation may be lower.
- Model Performance: The baseline model achieved high accuracy in predicting non-shortage periods, but recall for shortage events was lower, suggesting further model refinement is needed for rare event prediction.
- Forecasting Potential: Time series model, SARIMA, demonstrated the ability to forecast demand trends (which also can be done for electricity production) supporting proactive planning and grid management.

#### Next steps
- Model Improvement - Tune Logistic Regression and SARIMA models for better results or try using more advanced models.  Use GridSearchCV to find most optimal hyper parameters to optimize the training and prediction/forecast results.

#### Outline of project

[Link to EDA notbook](Final_Capstone_EDA.ipynb)


##### Contact and Further Information