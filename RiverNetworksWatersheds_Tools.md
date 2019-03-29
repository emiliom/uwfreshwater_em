# Compilation of open-source tools that perform river network extraction, network analysis, and watershed generation
**Python-centric or web-serviced based tools or access to important datasets.** 

- Go over my firefox bookmarks to find recent bookmarks

## Digital Terrain Analysis, river network extraction and watershed delineation
- [TauDEM](http://hydrology.usu.edu/taudem/taudem5/index.html)
  - https://github.com/dtarb/TauDEM
  - https://github.com/alexbruy/processing-taudem
- Rapid Watershed Delineation
  - https://github.com/nazmussazib/RapidWatersheDelineation/
  - https://github.com/WikiWatershed/rapid-watershed-delineation/
  - MMW RWD web service
  - Sazib, Nazmus S. 2016. “Physically Based Modeling of the Impacts of Climate Change on Streamflow Regime.” PhD, Civil and Environmental Engineering, Utah State University. http://digitalcommons.usu.edu/etd/5067/.
  - Tarboton, David G., Nazmus Sazib, and Anthony K. Aufdenkampe. 2018. “The Model My Watershed Rapid Watershed Delineation Tool | CUAHSI HydroShare.” 2018. https://www.hydroshare.org/resource/d752efeae812478898fb78327f25c87c/
- [pysheds](https://github.com/mdbartos/pysheds). "Simple and fast watershed delineation in python". https://www.esipfed.org/student-fellow-blog/pysheds-a-fast-open-source-digital-elevation-model-processing-library
- [watershed](https://github.com/phobson/watershed)
- https://github.com/selimnairb/EcohydroLib/tree/master/ecohydrolib. These are old, last maintained in May 2013
  - https://github.com/selimnairb/EcohydroLib/tree/master/ecohydrolib/nhdplus2
  - https://github.com/selimnairb/EcohydroLib/tree/master/ecohydrolib/hydro1k
- [Landlab](http://landlab.github.io)
  - [Flow Routing](https://landlab.readthedocs.io/en/release/#flow-routing) component. See also the related notebooks, including [flow_direction_and_accumulation/the_FlowDirectors.ipynb](https://nbviewer.jupyter.org/github/landlab/tutorials/blob/release/flow_direction_and_accumulation/the_FlowDirectors.ipynb)
  - [Terrain Analysis](https://landlab.readthedocs.io/en/latest/#terrain-analysis) component

## Network analysis
- Papers. Demir et al (2017) in particular seems really valuable
  - Cui, Zhengtao, Victor Koren, Neftali Cajina, Andreas Voellmy, and Fekadu Moreda. 2011. “Hydroinformatics Advances for Operational River Forecasting: Using Graphs for Drainage Network Descriptions.” Journal of Hydroinformatics 13 (2): 181–97. https://doi.org/10.2166/hydro.2010.023.
  - de Jager, A. L., and J. V. Vogt. 2010. “Development and Demonstration of a Structured Hydrological Feature Coding System for Europe.” Hydrological Sciences Journal 55 (5): 661–75. https://doi.org/10.1080/02626667.2010.490786
  - **Demir, Ibrahim, and Robert Szczepanek. 2017.** “Optimization of River Network Representation Data Models for Web-Based Systems.” Earth and Space Science 4 (6): 336–47. https://doi.org/10.1002/2016EA000224
  - Riedl, Doris. 2014. “Algorithms for Surface Water Networks and Their Catchments.” Phd, wien: uniwien. http://othes.univie.ac.at/33600/.
- [USGS CIDA - NLDI: The Hydro Network-Linked Data Index](https://owi.usgs.gov/blog/nldi-intro/)
  - https://my.usgs.gov/confluence/display/qwdp/Networked+Linked+Data+Index
  - [OGC ELFIE](http://www.opengeospatial.org/projects/initiatives/elfie)
- HUC codes, NHDPlus. Horizon Systems Corporation. 2016. “NHD Plus Version 2: Users Guide.” http://www.horizon-systems.com/nhdplus/.
- [Pfastteter topological coding system](https://en.wikipedia.org/wiki/Pfafstetter_Coding_System). Querying for network relationships based on these codes. HydroBASINS, HydroSHEDS. See my [GeoHackWeek vector example](https://geohackweek.github.io/vector/06-geopandas-advanced/)
- Tree / network path analysis
  - [anytree](https://github.com/c0fec0de/anytree). My anytree network querying code, via my examples from Costa Rica HydroSheds watersheds
  - [treelib](https://github.com/caesar0301/treelib), "An efficient implementation of tree data structure in python". 
  - Graph-theory approaches
