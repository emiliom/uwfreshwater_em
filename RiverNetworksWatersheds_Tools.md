# Compilation of open-source tools that perform river network extraction, network analysis, and watershed generation
**Python-centric or web-service based tools or access to important datasets.** 

## Digital Terrain Analysis, river network extraction and watershed delineation
- [TauDEM](http://hydrology.usu.edu/taudem/taudem5/index.html)
  - http://hydrology.usu.edu/taudem/taudem5/
  - https://github.com/dtarb/TauDEM
  - https://github.com/alexbruy/processing-taudem
  - https://github.com/WikiWatershed/docker-taudem
- Rapid Watershed Delineation
  - https://github.com/nazmussazib/RapidWatersheDelineation/
  - https://github.com/WikiWatershed/rapid-watershed-delineation/
  - MMW RWD web service
  - Sazib, Nazmus S. 2016. “Physically Based Modeling of the Impacts of Climate Change on Streamflow Regime.” PhD, Civil and Environmental Engineering, Utah State University. http://digitalcommons.usu.edu/etd/5067/.
  - Tarboton, David G., Nazmus Sazib, and Anthony K. Aufdenkampe. 2018. “The Model My Watershed Rapid Watershed Delineation Tool | CUAHSI HydroShare.” 2018. https://www.hydroshare.org/resource/d752efeae812478898fb78327f25c87c/
  - My ModelMyWatershed web service [API notebook demoing watershed extraction](http://nbviewer.jupyter.org/github/WikiWatershed/model-my-watershed/blob/develop/doc/MMW_API_watershed_demo.ipynb). The notebook and related documents are [hosted here](https://github.com/WikiWatershed/model-my-watershed/tree/develop/doc)
- [pysheds](https://github.com/mdbartos/pysheds). "Simple and fast watershed delineation in python". https://www.esipfed.org/student-fellow-blog/pysheds-a-fast-open-source-digital-elevation-model-processing-library
  - See my WaterHackWeek2019 notebook, `andeanamaz_pysheds.ipynb`
  - Some helpful links/docs I found:
    - https://github.com/mdbartos/pysheds/blob/master/examples/shapefiles.ipynb
    - https://github.com/mdbartos/pysheds/blob/master/examples/snap_to_mask.ipynb
    - [accept raster / array of pour points as input to catchment, issue #64](https://github.com/mdbartos/pysheds/issues/64#issuecomment-462951248)
    - https://github.com/cfandel/gottesacker/blob/master/subwatersheds.ipynb
- [watershed](https://github.com/phobson/watershed)
- https://github.com/selimnairb/EcohydroLib/tree/master/ecohydrolib. These are old, last maintained in May 2013
  - https://github.com/selimnairb/EcohydroLib/tree/master/ecohydrolib/nhdplus2
  - https://github.com/selimnairb/EcohydroLib/tree/master/ecohydrolib/hydro1k
  - https://github.com/selimnairb/RHESSysWorkflows
- [Landlab](http://landlab.github.io)
  - [Flow Routing](https://landlab.readthedocs.io/en/release/#flow-routing) component. See also the related notebooks, including [flow_direction_and_accumulation/the_FlowDirectors.ipynb](https://nbviewer.jupyter.org/github/landlab/tutorials/blob/release/flow_direction_and_accumulation/the_FlowDirectors.ipynb) and [flow_direction_and_accumulation/the_FlowAccumulator.ipynb](https://nbviewer.jupyter.org/github/landlab/tutorials/blob/release/flow_direction_and_accumulation/the_FlowAccumulator.ipynb)
  - [Terrain Analysis](https://landlab.readthedocs.io/en/latest/#terrain-analysis) component
  - https://github.com/landlab/landlab/wiki/Tutorials
- [`bopen/elevation`, SRTM DEM access](https://github.com/bopen/elevation). Python script to download global terrain digital elevation models, SRTM 30m DEM and SRTM 90m DEM.
- [A table I created listing important or promising geospatial datasets of surface waters and their properties](https://docs.google.com/document/d/1Q1gWXpgUrOPKo1lhtciZN5hn0bYvKI9jLjvh9hQfEE4/edit?usp=sharing)

## Network analysis
- Papers. Demir et al (2017) in particular seems really valuable
  - Cui, Zhengtao, Victor Koren, Neftali Cajina, Andreas Voellmy, and Fekadu Moreda. 2011. “Hydroinformatics Advances for Operational River Forecasting: Using Graphs for Drainage Network Descriptions.” Journal of Hydroinformatics 13 (2): 181–97. https://doi.org/10.2166/hydro.2010.023.
  - de Jager, A. L., and J. V. Vogt. 2010. “Development and Demonstration of a Structured Hydrological Feature Coding System for Europe.” Hydrological Sciences Journal 55 (5): 661–75. https://doi.org/10.1080/02626667.2010.490786
  - **Demir, Ibrahim, and Robert Szczepanek. 2017.** “Optimization of River Network Representation Data Models for Web-Based Systems.” Earth and Space Science 4 (6): 336–47. https://doi.org/10.1002/2016EA000224
  - Riedl, Doris. 2014. “Algorithms for Surface Water Networks and Their Catchments.” Phd, wien: uniwien. http://othes.univie.ac.at/33600/.
- [USGS CIDA - NLDI: The Hydro Network-Linked Data Index](https://owi.usgs.gov/blog/nldi-intro/)
  - https://my.usgs.gov/confluence/display/qwdp/Networked+Linked+Data+Index
  - [OGC ELFIE](http://www.opengeospatial.org/projects/initiatives/elfie)
- [Watershed / hydrological coding systems](https://en.wikipedia.org/wiki/Hydrological_code)
- [Pfastteter topological coding system](https://en.wikipedia.org/wiki/Pfafstetter_Coding_System). Querying for network relationships based on these codes. HydroBASINS, HydroSHEDS. See my [GeoHackWeek vector example](https://geohackweek.github.io/vector/06-geopandas-advanced/)
- US
  - HUC codes, NHDPlus. Horizon Systems Corporation. 2016. “NHD Plus Version 2: Users Guide.” http://www.horizon-systems.com/nhdplus/.
  - https://www.usgs.gov/core-science-systems/ngp/national-hydrography/about-national-hydrography-products, https://www.usgs.gov/core-science-systems/ngp/national-hydrography and https://www.usgs.gov/core-science-systems/ngp/national-hydrography/watershed-boundary-dataset
	- https://nhd.usgs.gov/userGuide/Robohelpfiles/NHD_User_Guide/Feature_Catalog/Watershed_Boundary_Dataset/Watershed_Boundary_Dataset.htm
	- https://water.usgs.gov/GIS/huc.html (mainly describes old, coarser-scale "HUC" dataset supersed by WBD)
	- https://hydro.nationalmap.gov/arcgis/rest/services/nhd/MapServer
	- https://hydro.nationalmap.gov/arcgis/rest/services/wbd/MapServer
- Querying and traversing river networks on a relational database system (discussions focused no PostgreSQL/PostGIS). [here](https://lists.osgeo.org/pipermail/postgis-users/2009-February/022748.html) and [here](https://lists.osgeo.org/pipermail/postgis-users/2009-February/022757.html)
- Tree / network path analysis
  - https://stackoverflow.com/questions/2358045/how-can-i-implement-a-tree-in-python-are-there-any-built-in-data-structures-in
  - https://stackoverflow.com/questions/3009935/looking-for-a-good-python-tree-data-structure
  - [anytree](https://github.com/c0fec0de/anytree). My anytree network querying code, via my examples from Costa Rica HydroSheds watersheds
  - [treelib](https://github.com/caesar0301/treelib), "An efficient implementation of tree data structure in python". 
  - Graph-theory approaches
  - [NetworkX](https://networkx.github.io/). https://en.wikipedia.org/wiki/NetworkX. NetworkX is a Python package for the creation, manipulation, and study of the structure, dynamics, and functions of complex networks.
    - https://pygraphviz.github.io/
    - https://www.python-course.eu/graphs_python.php
    - https://www.python-course.eu/networkx.php
    - https://gis.stackexchange.com/questions/227909/from-shapefile-to-python-networkx
    - https://towardsdatascience.com/getting-started-with-graph-analysis-in-python-with-pandas-and-networkx-5e2d2f82f18e
    - https://www.esipfed.org/uncategorized/natural-resources-nutrient-loading-and-networkx-watershed-network-analysis-part-i

## R tools
- [Watersheds:](https://cran.r-project.org/web/packages/Watersheds/index.html) Spatial Watershed Aggregation and Spatial Drainage Network Analysis
- [hydrolinks:](https://cran.r-project.org/web/packages/hydrolinks/index.html) Tools to link geographic data with hydrologic network, including lakes, streams and rivers. Includes automated download of U.S. National Hydrography Network and other hydrolayers. See this vignette: [WQP Lake Linking Example - Linking Water Quality Portal](https://cran.r-project.org/web/packages/hydrolinks/vignettes/wqp_lake_linking_example.html)
- [CRAN Task View: Hydrological Data and Modeling](https://cran.r-project.org/web/views/Hydrology.html). Curated listing of relevant packages
