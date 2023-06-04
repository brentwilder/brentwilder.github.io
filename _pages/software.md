---
layout: single
permalink: /software/
title: "Software"
excerpt: "Software"
author_profile: false
---

## Global Optical Snow properties via High-speed Algorithm With K-means clustering (GOSHAWK)
This repository can be used to take in spaceborne imaging spectroscopy data to output snow surface properties. Our algorithm solves for these properties simultaneously using numerical optimization of a linear mixture / two-stream snow model ([TARTES](https://github.com/ghislainp/tartes)). We leverage k-means spectral clustering and message passing interface to greatly speed up computation.



## Coregistration workflow for helicopter lidar data ([ice-road-copters](https://github.com/SnowEx/ice-road-copters))

The ice-road-copter suite is designed to post-process point cloud data and enable differencing to resolve change in repeat collections. Our focus is snow depth maps. DEM differencing for snow depths requires detailed knowledge of Coordinate Reference Systems (CRS) for the reference product (snow-free) and other products (snow-on). Alignment issues often persist even when both products are tied to the same CRS and needs to be addressed with a co-registration process. This software relies on the Point Data Abstraction Library ([PDAL](www.pdal.io)) for point cloud filtering and segmentation and  NASA's Ames Stereo Pipeline  ([ASP](https://github.com/NeoGeographyToolkit/StereoPipeline)) to perform the co-registration component of the workflow. The software is designed to use plowed roadways through the survey domain as co-registration objects, as the snow-covered domain often lacks stable features. We use ASP's pc_align function to apply ICP method to align to these fixed surfaces and then apply translational/rotational matrix to the rest of the dataset.

![roads](https://raw.githubusercontent.com/SnowEx/ice-road-copters/main/docs/roads.png)
![snow](https://raw.githubusercontent.com/SnowEx/ice-road-copters/main/docs/snow.jpeg)




