---
layout: single
permalink: /software/
title: "Software"
excerpt: "Software"
author_profile: false
---

## Coregistration workflow for helicopter lidar data
### [ice-road-copters](https://github.com/SnowEx/ice-road-copters)

The ice-road-copter suite is designed to post-process point cloud data and enable differencing to resolve change in repeat collections. Our focus is snow depth maps. DEM differencing for snow depths requires detailed knowledge of Coordinate Reference Systems (CRS) for the reference product (snow-free) and other products (snow-on). Alignment issues often persist even when both products are tied to the same CRS, and this needs to be addressed with a co-registration process.  The software relies on the Point Data Abstraction Library ([PDAL](www.pdal.io)) for point cloud filtering and segmentation.  NASA's Ames Stereo Pipeline  ([ASP](https://github.com/NeoGeographyToolkit/StereoPipeline)) performs the co-registration component of the workflow.  The software is designed to use plowed roadways through the survey domain as co-registration objects, as the snow-covered domain often lacks stable features.   

![roads](https://raw.githubusercontent.com/SnowEx/ice-road-copters/main/docs/roads.png)
![snow](https://raw.githubusercontent.com/SnowEx/ice-road-copters/main/docs/snow.jpeg)



## Snow Albedo Alg coming soon...

;)
