
Supplementary for: Forecast from VONA bulletin - 20210223_0446Z
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
  

|Parameters|Values|
| :--- | :--- |
|Number of perturbed meteo data|10|
|Perturbation on horizontal wind direction |Gaussian 0 ± 15°|
|Perturbation on horizontal wind intensity|Gaussian 1 ± 0.5m/s|
|Number of eruptive scenarios|1|
|Number of perturbed ESP per scenario|10|
|Column height|Uniform [5000 m, 10000 m]|
|Total Grain Size Distribution|Gaussian μ = 2.3 ± 0.5 φ,  σ = 1.5 ± 0.5 φ|
|Number of ensemble members per scenario|100|
  
Go to [Main page](https://github.com/federicapardini/Real_time_ash_forecast/tree/main/20210223_0446Z)  
Go to [Main directory](https://github.com/federicapardini/Real_time_ash_forecast)
