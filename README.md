# Real-time ash forecast at Mt. Etna (Italy)

This repository provides volcanic ash hazards maps at Mt. Etna produced by numerical simulations performed in real-time when explosive eruptions occur.

The numerical procedure for ash forecast has been developed at INGV-Sezione di Pisa and it runs automatically and in real-time when bulletins reporting Mt. Etna explosive activity are released by The Etnean Observatory of INGV.

Here the main features of the forecast procedure:

* Numerical models used: eruptive column model PLUME-MoM-TSM coupled with the VATDM HYSPLIT
* Meteo data:
* Ensemble of simulations are performed and statistical ash hazard maps are produced
  * The ensemble is created by defining probability distributions for  

  * Bullet 2a
  * Bullet 2b
* Bullet 3

|Parameters|Values|
| :--- | :--- |
|Numerical codes||
|Meteo data|Probability density histograms of ground load in kg/m² at a number of locations. 95th percentile is also reported|
|Atmospheric hazard maps|Probability in % that the ash concentration between differnt FL exceeds 2 g/m³|


The numerical codes used are the eruptive column model PLUME-MoM-TSM and the VATDM HYSPLIT.

For each RED VONA bulletin released at time YYYY-MM-DD/HH-mm Z, a directory named YYYYMMDD_HHmmZ is created and results uploaed automatically.

Select the directory of interest and the file XXX.md to see the latest results. For more details on the numerical procedure and results, select the YYY.md

# Forecast products

|Parameters|Values|
| :--- | :--- |
|Ground hazard maps|Probability in % that the deposit load exceeds 1 kg/m² and 10 kg/m²|
|Ground load at strategic locations|Probability density histograms of ground load in kg/m² at a number of locations. 95th percentile is also reported|
|Atmospheric hazard maps|Probability in % that the ash concentration between differnt FL exceeds 2 g/m³|




