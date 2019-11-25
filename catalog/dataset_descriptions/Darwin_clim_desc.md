This version of the model is modified from Dutkiewicz et al. (2015) and Ward et al. (2012). It includes the biogeochemical cycling of carbon, nitrogen, phosphorus, silica, iron and oxygen, a complex marine ecosystem, incorporating both functional and size diversity of phytoplankton and zooplankton, as well as dissolved organic matter (including an explicit colored component, CDOM), and organic particulate matter. An explicit radiative transfer component and spectral treatment of irradiance provides output that is similar to data provided by ocean color satellite instruments (surface reflectance) and also subsurface optical characteristics such as absorption and scattering.
There are 35 phytoplankton types (2 pico-prokaryotes, 2 pico-eukaryotes, 5 coccolithophore, 5 diazotrophs, 11 diatoms, 10 mixotrophic dinoflagellates) and 16 zooplankton types ranging from 0.6µm to 2500 µm equivalent spherical diameter. Parameters influencing growth, grazing, and sinking are related to size (following Ward et al., 2012) with specific differences between functional groups. This simulation uses Monod kinetics, and C:N:P:Fe stoichiometry are constant over time (though do differ between different phytoplankton groups). The zooplankton preferentially graze on plankton 10 times smaller than themselves with a Holling III function. The distributions of the plankton in this model compare well with both observations based on functional types as well as size distributions. We have incorporated distinct absorption and scattering spectra for the different phytoplankton (as in Dutkiewicz et al., 2015) as well as flattening of the spectra with size for absorption and scattering.


In **Darwin_v0.1_llc90**, this ecosystem model is driven by the physical ocean model of Forget et al, 2015 (ECCO version 4, https://eccov4.readthedocs.io) which runs on a 1-degree, global grid called LLC90 (Forget et al, 2015). This physical ocean model benefits from optimized parameterizations (small- and meso-scale turbulence) and atmospheric boundary conditions (air-sea fluxes). As a result, it matches in-situ observations (T, S, MLD, etc.) and remote sensing data (SST, altimetry, etc.) better than earlier ECCO solutions do (Forget, Ferreira, Liang 2015, Forget and Ponte 2015). Another advantage of this model configuration is that it is easy and inexpensive to rerun in order to produce more output or to experiment with the ecosystem and physical model settings (Forget 2018, 2019, https://cbiomes.readthedocs.io). Results here have been interpolated to a ½ degree grid.