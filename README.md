# Real-time tephra forecast at Mt.Etna (Italy)

<p align="center">
  <img src="./logo_dir/Logo_INGV.png" width=150pt />
</p>


This repository provides volcanic hazard maps for tephra fallout and dispersal at Mt.Etna (Italy). Numerical forecasts are produced by an automated workflow which is activated in real-time when explosive eruptions with tephra emission occur. The workflow is informed about the state of the volcano by the Volcano Observatory Notifications for Aviation (VONAs) issued by the Italian National Institute of Geophysics and Volcanology - Osservatorio Etneo (INGV-OE), which is the reference institure for the monitoring of Mt.Etna. The numerical procedure has been developed and tested at the Italian National Institute of Geophysics and Volcanology - Sezione di Pisa (INGV-Sezione di Pisa), with the contribution of colleagues from the INGV-OE.

The main features of the workflow are:

* Meteo data source: ARPA-SIM Mesoscale Model
* Numerical models used: eruptive column model PLUME-MoM-TSM coupled with the TTDM HYSPLIT
* Ensemble of simulations are performed and probabilistic hazard maps are produced

### Forecast products

Forecasts are provided at hours +1, +2, +3, +6, +9 and +12 from the issuing of each red VONA and at hours +3, +6, +9 and +12 from the issuing of the orange VONA.

|Type of product|Description|
| :--- | :--- |
|MER, total mass of tephra in the air, total mass of tephra deposited on the ground|Tables showing the 5th, 50th and 95th percentiles of MER [kg/s¹], total mass in the air [kg], total mass on the ground [kg]|
|Ground load at strategic locations|Tables showing the ground load in kg/m² at a number of locations. For each location, we report the 5th, 50th and 95th percentiles of the ground load distribution resulting from the simulations forming the ensemble|
|Ground hazard maps|Probability in % that deposit load exceeds 0.5 kg/m² and 5 kg/m²|
|Atmospheric hazard maps|Probability in % that ash concentration between different atmospheric levels exceeds 0.2 g/m³, 2 g/m³ and 4 g/m³|

### How to display the results
* Go to the FORECAST_RESULTS directory
* Select the directory of interest (each directory is named according to the time of issue of the first red VONA of the event)
    * The main results are in the file *README.md* which is automatically displayed by selecting the directory of interest
    * Additional information are in *Supplementaty_page.md*
    * All the figures shown in the *README.md* and more are collected in the directory *figures*. Additional files reporting the eruptive source parameters used in the simulations are in the directory *input_data*

### Please note that the numerical procedure is currently under development and daily updated



