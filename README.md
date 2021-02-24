# Real-time ash forecast at Mt. Etna (Italy)

This repository provides volcanic ash hazards maps at Mt. Etna produced by numerical simulations performed in real-time when explosive eruptions occur. The numerical procedure has been developed at INGV-Sezione di Pisa and it runs automatically and in real-time when bulletins reporting Mt. Etna explosive activity are released by The Etnean Observatory of INGV.

The main features of the forecast procedure are:

* Meteo data source: ARPA-SIM Mesoscale Model
* Numerical models used: eruptive column model PLUME-MoM-TSM coupled with the VATDM HYSPLIT
* Ensemble of simulations are performed and statistical ash hazard maps are produced
    * The ensemble is created by considering uncertainties on the meteorologiacal data and eruptive source parameters. The uncertainty on the meteorological data is modelled by generating Nwind perturbed versions of a reference meteo data. Each perturbed meteo data derives from the original one by adding perturbations on wind intensity and direction. For the eruptive source parameters, we model as uncertain input variables the height of the eruptive column at the vent and the Total Grain Size Distribution (TGSD) defining the solid phase of the eruptive mixture. In particular, we assume as uncertain parameters the mean value and the standard deviation defining the lognormal TGSD. The three uncertain input variables (i.e. column height, mean value of the TGSD and standard deviation) are described as probability distributions which can be uniform or gaussian. In the first case (uniform), the minimum and maximum values defining the bounds of the distribution are chosen, while for the second case (gaussian), we specify the mean value and the standard deviation. By sampling the three distributions, we end with Nesp that, combined with the Nwind meteo data, form a total of N (= Nwind * Nesp) simulations.
* When a RED VONA bulletin is released, the simulations are initialized at the VONA issued time and a continous ash emission lasting 12 h is simulated. In case a new VONA is issued, the numerical simulations are updated considering the latest information.

### Forecast products

For each RED VONA, continous ash emission is simulated for 12 h from the beginning of the event. A total of 4 forecasts are provided at hours +3, +6, +9 and +12 from the beginnig of the eruption.

|Type of product|Description|
| :--- | :--- |
|Ground hazard maps|Probability in % that the deposit load exceeds 1 kg/m² and 10 kg/m²|
|Ground load at strategic locations|Tables showing the ground load in kg/m² at a number of locations. For each location, we report 5th, 50th and 95th percentiles of the ground load distribution resulting from the N simulations forming the ensemble|
|Atmospheric hazard maps|Probability in % that the ash concentration between differnt FL exceeds 2 g/m³|

### How to see the results

Select the directory of interest (each directory is named as the RED VONA release time) and the file Supplementary_page.md to see the latest results.




