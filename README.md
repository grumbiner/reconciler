# reconciler
Bathymetry + Coastline reconciliation on to target grid

This works from coastline bounding curves (via a now-old version of GSHHS) and a bathymetry data file (etopo2) to produce a land mask and a bathymetry on target grids. 

* docs contains the original publication and some notes on how to use the codes
* reference contains a couple of reference files (strait definitions and some points of interest)
* working has a working set of codes, makefile, and build script with which to build masks + bathymetries
* .gitmodules includes the reference to the MMABLIB, which is needed by the codes -- [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7387835.svg)](https://doi.org/10.5281/zenodo.7387835)

Also present, but only retained for historical reference:
* legacy1 -- source/make/scripts that are, more or less, older
* legacy2 -- source/make/scripts that are, more or less, newer and perhaps less stable

The original document is in docs, TN301 from the NOAA/NWS/NCEP Environmental Modeling Center, Marine Modeling and Analysis Branch

Robert Grumbine
