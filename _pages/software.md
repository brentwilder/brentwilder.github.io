---
layout: single
permalink: /software/
title: "Software"
excerpt: "Software"
author_profile: false
---

## Global Optical Snow properties via High-speed Algorithm With K-means clustering ([goshawk](https://github.com/cryogars/goshawk))
This repository can be used to take in spaceborne imaging spectroscopy data to output snow surface properties. Our algorithm solves for these properties simultaneously using numerical optimization of a linear mixture and a coupled snow & atmospheric radiative transfer model. We leverage k-means spectral clustering and message passing interface to greatly speed up computation. We also solved optimally for terrain, thereby reducing errors associated with global DEM incidence angles. 



## Coregistration workflow for helicopter lidar data ([ice-road-copters](https://github.com/cryogars/ice-road-copters))

The ice-road-copter suite is designed to post-process point cloud data and enable differencing to resolve change in repeat collections. Our focus is snow depth maps. DEM differencing for snow depths requires detailed knowledge of Coordinate Reference Systems (CRS) for the reference product (snow-free) and other products (snow-on). Alignment issues often persist even when both products are tied to the same CRS and needs to be addressed with a co-registration process. This software relies on the Point Data Abstraction Library for point cloud filtering and segmentation and  NASA's Ames Stereo Pipeline to perform the co-registration component of the workflow. The software is designed to use plowed roadways through the survey domain as co-registration objects, as the snow-covered domain often lacks stable features. We use ASP's pc_align function to apply ICP method to align to these fixed surfaces and then apply translational/rotational matrix to the rest of the dataset.





