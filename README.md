# Grabow et al. 2022 *Frontiers in Ecology and Evolution*
## Data-integration of opportunistic species observations into hierarchical modelling frameworks improves spatial predictions for urban red squirrels 

> **M. Grabow**, **J. Louvrier**, **A. Planillo**, **S. Kiefer**, **S. Drenske**. **K. Börner**, **M. Stillfried**, **R. Hagen**, **S. Kimmig**, **T. Straka** & **S. Kramer-Schadt** (2022). Data-integration of opportunistic species observations into hierarchical modelling frameworks improves spatial predictions for urban red squirrels. *Frontiers in Ecology and Evolution*. DOI: [10.3389/fevo.2022.881247](https://dx.doi.org/10.3389/fevo.2022.881247)
---
## Abstract

The prevailing trend of increasing urbanisation and habitat fragmentation makes knowledge of species’ habitat requirements and distribution a crucial factor in conservation and urban planning. Species distribution models (SDMs) offer powerful toolboxes for discriminating the underlying environmental factors driving habitat suitability. Nevertheless, challenges in SDMs emerge if multiple data sets - often sampled with different intention and therefore sampling scheme – can complement each other and increase predictive accuracy. Here, we investigate the potential of using recent data integration techniques to model potential habitat and movement corridors for Eurasian red squirrels (Sciurus vulgaris) in an urban area. We constructed hierarchical models integrating data sets of different quality stemming from unstructured on one side and semi-structured wildlife observation campaigns on the other side in a combined likelihood approach and compared the results to modelling techniques based on only one data source. Our study highlights the increasing importance of considering multiple data sets for SDMs to enhance their predictive performance. We finally used Circuitscape (version 4.0.5) on the most robust model to delineate suitable movement corridors for red squirrels as a basis for planning road mortality mitigation measures. Our results indicate that even though red squirrels are common, urban habitats are rather small and partially lack connectivity along natural connectivity corridors in Berlin. Thus, additional fragmentation could bring the species closer to its limit to persist in urban environments.

---
## Data

This Repository includes two data sets of red squirrel observations:

1.) The **unstructured** data set of red squirrel observations was collected opportunistically by non-scientists

2.) The **semi-structured** data set of red squirrel observations was collected by camera-traps set up in private or allotment gardens. Given the sensitive nature of this data set, coordinates refer to the centroid of the 2 x 2 km grid cell the garden is located in.


---
## Scripts

The R scripts are located in the `R` subfolder:

`02_occupancy`: single season occupancy models fit to the **semi-structured** camera-trap data set (M3)

`03_maxent`: MaxEnt models fit with the **unstructured** opportunistically collected data set only (M1) & incorporating the **semi-structured** data-set (M2)

`04_data_integration`: Inhomogeneous Poisson point process model (IPPPM): Data-integration approach combining the **structured** and **unstructured** data sets (M4)

`05_data_integration_area_interaction`: Area interaction model (AIM): Data-integration approach combining the **structured** and **unstructured** data sets (M5)

The Circuitscape configuration & input files are located in the `Circuitscape` subfolder
