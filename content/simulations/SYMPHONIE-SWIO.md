---
section: Simulations
nav_order: 6
title: SYMPHONIE-IndOc configuration
---

# Indian Ocean configurations and simulations with SYMPHONIE hydrodynamic model


## People in charge and affiliation

Lisa Weiss (LEGOS, IRD) 


## Scientific context and background 

The SYM-IndOc.HR model configuration was developed to simulate the ocean circulation of the entire Indian Basin. It enables the  the study of meso and submesoscale processes in the coastal region, from the Mozambique Channel to the Bay of Bengal, at a resolution of 1 to 3 km. It has been designed to support studies on land-sea transfers and marine debris dispersion from coastal to basin scales. In addition to air-sea exchanges and tides, this configuration integrates the recently released high-resolution GloFAS river discharge dataset to force the physical simulations with daily freshwater inputs, as well as wave forcing through both the Stokes-Coriolis force and the Stokes drift (IndOc.HR-Sto). 

## Related publications

* Weiss, L., Herrmann, M., Marsaleix, P., Bompoil, M., and Maes, C. (2026). Modeling Indian Ocean circulation to study marine debris dispersion: insights into high-resolution and wave forcing effects with Symphonie 3.6.6, Geosci. Model Dev., 19, 827–865, https://doi.org/10.5194/gmd-19-827-2026.

* Weiss, L., Herrmann, M., Marsaleix, P. (2025). Model code and regional configuration for 'Modeling Indian Ocean circulation to study marine debris dispersion: insights into high-resolution and Stokes drift effects'. figshare. Journal contribution. https://doi.org/10.6084/m9.figshare.28903067.v4

* Thibault, M., Weiss, L., Fernandez, R., Avargues, N., Jaquemet, S., Lebreton, L., ... & Le Corre, M. (2024). Barau's petrel, Pterodroma baraui, as a bioindicator of plastic pollution in the South-West Indian Ocean: A multifaceted approach. Marine Environmental Research, 202, 106709, https://doi.org/10.1016/j.marenvres.2024.106709.

## Configurations, parameters, resolution, timestep, domain, span

* Existing configurations: IndOc.HR, IndOc.HR-Sto, IndOc.12
  
* Grid resolutions:
  
      - IndOc.HR and IndOc.HR-Sto: curvilinear Arakawa C-grid (3000 × 2800 cells) with a horizontal resolution of 1 to 3 km along East African and Indian coasts, 12 km toward Australia and a maximum mesh size of 23 km at the south boundary reaching Antarctica.
  
      - IndOc.12: regular Arakawa C-grid grid (1536 x 1100 cells) with a horizontal discretization at 1/12° (8-9 km).
 
<img src="figures/f01_grid_edit_review.png" alt="drawing" width="600"/>

**Fig. 1 : IndOc.HR grid (in km, gray scale), displaying every 50 gridlines (red lines). Blue dots show the 336 daily freshwater discharges simulated in the configuration.**

## Number of simulations (+ number of members if ensemble)

* IndOc.HR, IndOc.HR-Sto, IndOc.12: 3 sensitivity tests with daily mean outputs over 1 year (2017) 

* IndOc.HR-Sto: Air-Sea forcing, Tides, River forcing, Wave forcing
  
        - 3D daily mean outputs 2016-2020, saved variables = U,V, SSH, Temperature, Salinity, W_surface, vertical tracer diffusivity [log10difv], turbulent kinetic energy [log10tke], water transport UAH, VAH
  
        - 2D hourly outputs 2016-2019, saved variables =  U,V surface, U,V bottom, U,V tide, U,V Stokes drift

* IndOc.HR-Sto: 3D tri-hourly mean outputs from 02/2019 to 10/2019 

## Related processing tools

## Calculation cost, volume, access

Regular SYMPHONIE netCDF files 

* 2D hourly outputs = 4.8 To (1.2 To per year x4)
* 3D daily mean outputs = 4.2 To (840 Go per year x5)
* When decompressed, 1 2D hourly file = 257 Mo, 9 To for 4 years, and 1 3D daily file = 5.9 Go, 10.8 To for 5 years

Stored on: TGCC-Irene and IGE-cal1-summer 

## Other Useful information

The current version 3.6.6 of the SYMPHONIE source code (hydrodynamics and Lagrangian modules), together with both Indian Ocean configuration grid files, are archived under the following DOI: https://doi.org/10.6084/m9.figshare.28903067 (Weiss, 2025). Last version of the model can also be obtain from the INSU-certified service SIROCCO at https://sirocco.obs-mip.fr. Considering their size, raw threedimensional simulation outputs are not stored publicly but are available upon request to the corresponding author. New simulations based on this configuration can be produced for any specified years of interest and for any ocean parameters to be studied.


