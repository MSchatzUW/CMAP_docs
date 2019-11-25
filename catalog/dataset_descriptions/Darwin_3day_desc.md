This dataset contains 3 Day Averaged Model nutrient outputs for the global ocean at 50 depth levels.

This version of the model is modified from Dutkiewicz et al. (2015) and Ward et al. (2012). It includes the biogeochemical cycling of carbon, nitrogen, phosphorus, silica, iron and oxygen, a complex marine ecosystem, incorporating both functional and size diversity of phytoplankton and zooplankton, as well as dissolved organic matter (including an explicit colored component, CDOM), and organic particulate matter. An explicit radiative transfer component and spectral treatment of irradiance provides output that is similar to data provided by ocean color satellite instruments (surface reflectance) and also subsurface optical characteristics such as absorption and scattering.
There are 35 phytoplankton types (2 pico-prokaryotes, 2 pico-eukaryotes, 5 coccolithophore, 5 diazotrophs, 11 diatoms, 10 mixotrophic dinoflagellates) and 16 zooplankton types ranging from 0.6µm to 2500 µm equivalent spherical diameter. Parameters influencing growth, grazing, and sinking are related to size (following Ward et al., 2012) with specific differences between functional groups. This simulation uses Monod kinetics, and C:N:P:Fe stoichiometry are constant over time (though do differ between different phytoplankton groups). The zooplankton preferentially graze on plankton 10 times smaller than themselves with a Holling III function. The distributions of the plankton in this model compare well with both observations based on functional types as well as size distributions. We have incorporated distinct absorption and scattering spectra for the different phytoplankton (as in Dutkiewicz et al., 2015) as well as flattening of the spectra with size for absorption and scattering.


In **Darwin_v0.2_cs510**, this ecosystem model is driven by the physical ocean model of Menemenlis et al 2008 (ECCO2, http: http://ecco2.jpl.nasas.gov). The grid is a cubed sphere with nominal resolution of 18km such that it is “eddy-permitting” in that it captures eddies and fronts at the mesoscale (order 100km), but not at the sub-mesoscale (order 10kms). Results here have been interpolated to a ½ degree grid. The ECCO2 synthesis covers the period 1992– 2015. The physical solution has been obtained using a data constrained Green's Function approach to estimate initial temperature and salinity conditions, surface boundary conditions, and several empirical ocean and sea ice model parameters. The control parameters include initial temperature and salinity conditions, atmospheric surface boundary conditions, background vertical diffusivity, critical Richardson numbers for the KPP scheme, air-ocean, ice-ocean, air-ice drag coefficients, ice/ocean/snow albedo coefficients, bottom drag, and vertical viscosity. Data constraints include sea level anomaly from altimeter data, time- mean sea level, sea surface temperature, temperature and salinity profiles from WOCE, TAO, ARGO, XBT, etc., sea ice concentration from passive microwave data, sea ice motion from radiometers, QuikSCAT, and RGPS, and sea ice thickness from ULS. Full depth biogeochemical solutions at native eddying resolutions are available via OpenDAP.