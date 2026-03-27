# Call Center Demand Forecast

Simple project to simulate a call center operation and estimate workforce requirements based on historical demand.

## Dataset

The dataset contains daily operational data, including:

- call volume (calls_received)
- average handling time (aht_seconds)
- SLA target
- available agents
- shrinkage
- peak day and weekend flags

## Objective

Estimate demand patterns and calculate the number of agents required to handle the workload.

## Approach

- Load and preprocess data
- Analyze call volume trends
- Identify weekly seasonality
- Apply a simple forecasting approach (moving average)
- Estimate required workforce based on workload

## Workforce Calculation

Workload is calculated as:

calls * AHT

Agent capacity assumes ~6 productive hours per day, adjusted by shrinkage.

## Tools

- Python (Pandas, Matplotlib)
- SQL
- Git

## Analysis

The full analysis can be found in the notebook:

analysis.ipynb
<img width="1007" height="451" alt="download" src="https://github.com/user-attachments/assets/11fef124-b615-4b62-9fe2-b3062ea57b4a" />

## Results

- Demand is consistently higher during weekdays compared to weekends  
- Peak days require significantly more workforce to maintain service levels  
- The moving average approach captures short-term demand trends effectively  
- Workforce requirements vary significantly depending on demand and AHT  

## Business Impact

This analysis demonstrates how forecasting and workforce planning can support operational efficiency, reduce queue risk and improve service level performance.

## Notes

This is a simplified model intended for demonstration purposes.
