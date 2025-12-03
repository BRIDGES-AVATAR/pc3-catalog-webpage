---
section: Simulations
nav_order: 4
title: SWIOSE simulations
---

## SouthWest Indian Ocean Stochastic Ensembles (SWIOSE): Probabilistic modeling of the Southwest Indian Ocean dynamics to quantify uncertainties in surface currents


### People in charge and affiliation

Lisa WEISS (LEGOS, IRD), Jean-Michel Brankart (IGE, CNRS), Pierre Brasseur (IGE, CNRS),


### Scientific context and background

***ADAPTED FROM WEISS ET AL., 2025***

The SouthWest Idian ocean Stochastic Ensembles (SWIOSE) are a set of numerical runs that were produced in the BRIDGES-AVATAR workframe. They aim at providing a realistic simulation of the Southwest Indian ocean physics (temperature, salinity, water speed, free surface, vorticity, etc.). In particular, their main objective is to identify and describe the importance of several sources of uncertainty, as they affect significantly the regions's surface circulation. Therefore, it is crucial to better assess these various sources of uncertainty, in order to develop an accurate, reliable avatar of the SWIO (see the [BRIDGES-AVATAR website](https://www.bridges-wio.com/fr/projet/pc-3-avatar/) for more information).

<img src="figures/bathy.png" alt="drawing" width="600"/>

**Fig. 1: Bathymetry of the SWIOSE simulations.**

The SWIOSE were produced as follows:

+ Development of a realistic configuration for the SWIO region, forced and validated with the CMEMS and ECMWF operational / satellite products,
+ Implementation of a [stochastic perturbation generator](https://github.com/brankart/stogen/tree/main) - initially developped for the NEMO model - into the Coastal and Regional Ocean COmmunity model (CROCO),
+ Production of stochastic ensembles of 30 members each,
+ Generation of stochastic processes with varying correlation structures, in the defined regional setting. This allows to test the cumulative effect of different sources of uncertainty associated with surface ocean circulation.

To date, three ensembles have been generated:
+ INI (perturbation of inital conditions),
+ CD (perturbation of the wind drag coefficient),
+ GLS (perturbation of vertical mixing terms, that is productive/destructive terms in the GLS turbulence equations).

A fourth ensemble (perturbation of the open boundary conditions) may also be produced later. These experiments describing prior uncertainties and the associated modeling testbed will then be used for 4D inversions (Popov et al., 2024) exploiting high-resolution spatial (real or simulated) altimetry, surface currents, high-resolution temperature and ocean colour data to reduce uncertainties in surface ocean Lagrangian transport. The integration of stochastic methodologies within CROCO may facilitate scenario exploration and uncertainty quantification, providing a basis for informed decision-making and collaborations with ocean actors in the SWIO region.


### Related publications

+ Weiss, L., Brankart, J.-M., Jamet, Q., and Brasseur, P.: *Probabilistic modeling of the Southwest Indian Ocean dynamics to quantify uncertainties in surface currents*, One Ocean Science Congress 2025, Nice, France, 3–6 June 2025, OOS2025-613, https://doi.org/10.5194/oos2025-613, 2025.

+ Phillips, H. E., Tandon, A., Furue, R., Hood, R., Ummenhofer, C. C., Benthuysen, J. A., Menezes, V., Hu, S., Webber, B., Sanchez-Franks, A., Cherian, D., Shroyer, E., Feng, M., Wijesekera, H., Chatterjee, A., Yu, L., Hermes, J., Murtugudde, R., Tozuka, T., Su, D., Singh, A., Centurioni, L., Prakash, S., and Wiggert, J.: *Progress in understanding of Indian Ocean circulation, variability, air–sea exchange, and impacts on biogeochemistry*, Ocean Sci., 17, 1677–1751, https://doi.org/10.5194/os-17-1677-2021, 2021.

+ Brankart, J.-M., Candille, G., Garnier, F., Calone, C., Melet, A., Bouttier, P.-A., Brasseur, P., and Verron, J.: *A generic approach to explicit simulation of uncertainty in the NEMO ocean model*, Geosci. Model Dev., 8, 1285–1297, https://doi.org/10.5194/gmd-8-1285-2015, 2015.

+ Popov, M., Brankart, J.-M., Capet, A., Cosme, E., and Brasseur, P.: *Ensemble analysis and forecast of ecosystem indicators in the North Atlantic using ocean colour observations and prior statistics from a stochastic NEMO–PISCES simulator*, Ocean Sci., 20, 155–180, https://doi.org/10.5194/os-20-155-2024, 2024.


### Number of simulations (+ number of members if ensemble)

+ 3 ensembles of 30 members : INI, CD, GLS (90 runs total)


### Configurations, parameters, resolution, timestep, domain, span

+ Domain: (SWIO region)
+ Resolution: 1/12°, sigma levels
+ Timespan: 3 years (2017-2019)


### Target variables

+ Physics: u, v, w, omega, T, S, zeta


### Related processing tools

+ [STOGEN module (Brankart)](https://github.com/brankart/stogen/tree/main) : production of stochastic ensembles


### Calculation cost, volume, access

+ Volume: 60 TB (daily average outputs)
+ These data are stored on the Adastra cluster (CINES). Please reach to [Jean-Michel Brankart or Aurélie Albert](https://meom-group.github.io/people/) if you are interested, or for further information.


### Other Useful information