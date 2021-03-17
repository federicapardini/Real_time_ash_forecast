
Supplementary for: Forecast from VONA bulletin - 20210318_1800Z
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
|Grid extension lat|3.0°|
|Grid extension lon|6.0°|
|Grid resolution lat|0.05°|
|Grid resolution lon|0.05°|
|Atmospheric levels|0 5000 15000 20000 m|

## HYSPLIT setting
  

|Parameters|Values|
| :--- | :--- |
|Pollutant type|Puff|
|Integration time step|10 min|
|Output resolution|10 min|

# Ensemble definition
  

|Parameters|Values|Type of distribution|
| :--- | :--- | :--- |
|Number of perturbed meteo data|3||
|Perturbation on horizontal wind direction |0 ± 15°|Gaussian|
|Perturbation on horizontal wind intensity|1 ± 0.5m/s|Gaussian|
|Number of eruptive scenarios|1||
|Number of perturbed ESP per scenario|3||
|Column height|[6000 m, 12000 m]|Uniform|
|Total Grain Size Distribution|μ = [-3 φ, 2 φ], σ = [0.6 φ, 1.5 φ]|Uniform|
|Number of ensemble members per scenario|9||
  
Go to [Main page](https://github.com/federicapardini/Real_time_ash_forecast/tree/main/FORECAST_RESULTS/20210318_1800Z)  
Go to [Main directory](https://github.com/federicapardini/Real_time_ash_forecast)