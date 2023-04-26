[![Language](https://img.shields.io/badge/python-3.6%2B-blue?style=flat-square)](https://www.python.org/)
[![License](https://img.shields.io/badge/license-Apache--2.0-blue?style=flat-square)](https://github.com/yunjunz/2021-Maduo-EQ/blob/main/LICENSE)
[![Citation](https://img.shields.io/badge/DOI-10.1029%2F2022JB025936-blue?style=flat-square)](https://doi.org/10.1029/2022JB025936)

## 2021-Maduo-EQ

This repo contains notebooks for the 3D co-seismic deformation of the 2021 Mw 7.4 Maduo earthquake in Qinghai, China ([USGS](https://earthquake.usgs.gov/earthquakes/eventpage/us7000e54r/executive)) from Sentinel-1 SAR data. It's used in the following paper:

+ Xu, L., Yunjun, Z., Ji, C., Meng, L., Fielding, E. J., Zinke, R., & Bao, H. (2023). Understanding the rupture kinematics and slip model of the 2021 Mw 7.4 Maduo earthquake: A bilateral event on bifurcating faults. _Journal of Geophysical Research: Solid Earth, 128_(4), e2022JB025936, doi:[10.1029/2022JB025936](https://doi.org/10.1029/2022JB025936).

### Data ([Zenodo](https://zenodo.org/record/7170329))

Two pairs of Sentinel-1 SLCs (from ascending track 99 and descending track 106; both acquired at 20 - 26 May 2021) are used to derive the deformation in range and azimuth directions, using both InSAR and SAR speckle tracking techniques.

+ S1_A099_20210520_20210526_IFG
+ S1_A099_20210520_20210526_OFF_RG
+ S1_A099_20210520_20210526_OFF_AZ
+ S1_D106_20210520_20210526_IFG
+ S1_D106_20210520_20210526_OFF_RG
+ S1_D106_20210520_20210526_OFF_AZ
+ S1_20210520_20210526_ENU

### Notebooks

+ [1. Prepare azimuth offsets](./1_prep_az_off.ipynb)
+ [2. Prepare range offsets](./2_prep_rg_off.ipynb)
+ [3. Prepare interferograms](./3_prep_ifgram.ipynb)
+ [4. Decompose asc & desc azimuth offsets & interferograms into east/north/up](./4_defo3d.ipynb)
+ [Fig. 3](./5_Fig_3.ipynb) - Ground static displacement in (a) 3D and (b) near-field for surface traces
+ [Fig. S1](./6_Fig_S1.ipynb) - Ground statid displacement in east, north and up directions
