
Supplementary for: Forecast from VONA bulletin - 20210216_1631Z
===============================================================

Contents
========

* [Input data](#input-data)
	* [Meteorological data](#meteorological-data)
	* [Volcanological data](#volcanological-data)
	* [Computational domain](#computational-domain)
	* [HYSPLIT setting](#hysplit-setting)
* [Ensemble definition](#ensemble-definition)

# Input data

## Meteorological data
  

|Parameters|Values|
| :--- | :--- |
|Data source|ARPA-SIM Mesoscale Model|
|Data type|Forecast|
|Temporal resolution|3 h|
|Grid resolution|0.05°|

## Volcanological data
  

|Parameters|Values|
| :--- | :--- |
|Volcano|Mt. Etna|
|Vent height|3300 m|
|Vent lat|37.73°|
|Vent lon|15.00°|
|Total Grain Size Distribution|Lognormal|
|Mixture temperature|[1300] K|
|Water vapour content|[0.03]|
|Particle density|[900]|
|Particle sphericity|[0.5]|
|Particle specific heat|[1100] J/KgK|

## Computational domain
  

|Parameters|Values|
| :--- | :--- |
|Grid center lat|37.73°|
|Grid center lon|15.0°|
|Grid extension lat|0.5°|
|Grid extension lon|0.5°|
|Grid resolution lat|0.01°|
|Grid resolution lon|0.01°|
|Atmospheric levels|0 5000 10000 20000 m|

## HYSPLIT setting
  

|Parameters|Values|
| :--- | :--- |
|Pollutant type|Puff|
|Integration time step|2 min|
|Output resolution|10 min|

# Ensemble definition
  

|Parameters|Values|Type of distribution|
| :--- | :--- | :--- |
|Number of perturbed meteo data|16||
|Perturbation on horizontal wind direction |0 ± 15°|Gaussian|
|Perturbation on horizontal wind intensity|1 ± 0.5m/s|Gaussian|
|Number of eruptive scenarios|1||
|Number of perturbed ESP per scenario|16||
|Column height|6000 ± 500 - from VONA|Gaussian|
|Total Grain Size Distribution|μ = [-4 φ, 0 φ], σ = [0.5 φ, 1.5 φ]|Uniform|
|Number of ensemble members per scenario|16||
  
Go to [Main page](https://github.com/federicapardini/Real_time_ash_forecast/tree/main/FORECAST_RESULTS/20210216_1631Z)  
Go to [Main directory](https://github.com/federicapardini/Real_time_ash_forecast)