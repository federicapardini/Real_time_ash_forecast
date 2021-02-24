# Real-time ash forecast at Mt. Etna (Italy)

This repository provides volcanic ash hazards maps at Mt. Etna produced by numerical simulations performed in real-time when explosive eruptions occur.

The numerical procedure for ash forecast has been developed at INGV-Sezione di Pisa and it runs automatically and in real-time when bulletins reporting Mt. Etna explosive activity are released by The Etnean Observatory of INGV.

The main features of the forecast procedure are:

* Numerical models used: eruptive column model PLUME-MoM-TSM coupled with the VATDM HYSPLIT
* Meteo data:
* Ensemble of simulations are performed and statistical ash hazard maps are produced
* The ensemble is created by considering uncertainties on the meteorologiacal data and eruptive source parameters (TGSD at the vent and column height). The uncertainty on the meteorological data is modelled by generating Nwind perturbed versions of a reference meteo data. Each perturbed meteo data derives from the original one by adding perturbations on wind intensity and direction. For the eruptive source parameters, we model as uncertain input variables the height of the eruptive column at the vent and the Total Grain Size Distribution (TGSD) defining the solid phase of the eruptive mixture. In particular, we assume that the TGSD is a lognormal one and thus the uncertain input parameters are the mean value and the standard deviation of the TGSD. The three uncertain input variables (i.e. column height, mean value of the TGSD and standard deviation) can be described with uniform or gaussian probability distributions. In the first case (uniform), the minimum and maximum values defining the bounds of the distribution can be chosen, while for the second case (gaussian), we specify mean value and standard deviation.

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




