# Real-time ash forecast at Mt. Etna (Italy)

<img src="./Logo_INGV.png" width=150pt/>

This repository provides volcanic ash hazards maps at Mt. Etna produced by numerical simulations performed in real-time when explosive eruptions occur. The numerical procedure has been developed at INGV-Sezione di Pisa and it runs automatically and in real-time when bulletins reporting Mt. Etna explosive activity are released by The Etnean Observatory of INGV.

The main features of the forecast procedure are:

* Meteo data source: ARPA-SIM Mesoscale Model
* Numerical models used: eruptive column model PLUME-MoM-TSM coupled with the VATDM HYSPLIT
* Ensemble of simulations are performed and statistical ash hazard maps are produced
    * The ensemble is created by considering uncertainties on the meteorologiacal data and eruptive source parameters. The uncertainty on the meteorological data is modelled by generating Nwind perturbed versions of a reference meteo data. Each perturbed meteo data derives from the original one by adding perturbations on wind intensity and direction. For the eruptive source parameters, we model as uncertain input variables the height of the eruptive column at the vent and the Total Grain Size Distribution (TGSD) defining the solid phase of the eruptive mixture. In particular, we assume as uncertain parameters the mean value and the standard deviation defining the lognormal TGSD. The three uncertain input variables (i.e. column height, mean value of the TGSD and standard deviation) are described as probability distributions which can be uniform or gaussian. In the first case (uniform), the minimum and maximum values defining the bounds of the distribution are chosen, while for the second case (gaussian), we specify the mean value and the standard deviation. By sampling the three distributions, we produce Nesp possible eruptive scenarios that, combined with the Nwind meteo data, form a total of N (= Nwind * Nesp) simulations.
* When a RED VONA bulletin is released, the N simulations are initialized at the VONA time of issue and a continous ash emission lasting 12 h is simulated. In case a new VONA is issued, the numerical simulations are updated considering the latest information.

### Forecast products

For each RED VONA, a total of 4 forecasts are provided at hours +3, +6, +9 and +12 from the beginnig of the eruption.

|Type of product|Description|
| :--- | :--- |
|MER, Ash mass in the air, Ash mass on the ground|Tables showing the 5th, 50th and 95th percentiles of MER [kg/s¹], Mass in the air [kg], Mass on the ground [kg]|
|Ground load at strategic locations|Tables showing the ground load in kg/m² at a number of locations. For each location, we report 5th, 50th and 95th percentiles of the ground load distribution resulting from the simulations forming the ensemble|
|Ground hazard maps|Probability in % that the deposit load exceeds 1 kg/m² and 10 kg/m²|
|Atmospheric hazard maps|Probability in % that the ash concentration between differnt FL exceeds 0.1 g/m³|

### How to display the results
* Go to FILES directory
* Select the directory of interest (each directory is named as the RED VONA time of issue)
    * The main results are in the file *README.md* which is automatically displayed by selecting the directory of interest. 
    * Additional information are in *Supplementaty_page.md*. 
    * All the figures shown in *README.md* and more are collected in the directory *figures* and .txt files reporting the eruptive source parameters used in the simulations are in the directory *input_data* 

### Please note that the numerical procedure is currently under development and daily updated



