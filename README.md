# Simulating Dispersal Across Cost Surfaces

There has been a rapid increase is the application of resistance-based landscape models, such as those produced through Circuitscape (1), in the fields of animal movement ecology, landscape genetics/genomics, conservation biology and landscape ecology. Often these cost surfaces are parameterized through expert opinion or genetics but very rarely, animal location data. The goal of this repository is provide a tool to test scenarios of dispersal across a parameterized cost surface through simulation  and use animal location data to validate the parameterization of the cost surface values. 

The completed end product will be a Python library that can be imported and used by others with Jupyter notebooks detailing its use. Users will be able to upload their Circuitscape map and enter in the starting locations to run animal dispersal simulations.

This library is still in development, however Jupyter notebooks will detail the steps to begin exploring the cost surface layers and the notebooks will be actively updated.


**Data and Tools**
The data that can be used for this are raster files (.tif, .asc files) of the cost surface of interest. Currently the raster file can be different numbers of rows and columns when itsimported but will either be trimmed or expanded so that the final file is the same number of rows and columns. 

The animal GPS location data can also be uploaded for visualization. These files can be in .kml format.

The tools that are used now or will be in the future are the following:

1.) Circuitscape to produce current density maps.
2.) GDAL to load and access the raster files and Matplotlib to visualize the map.
3.) NumPy to manipulate the raster files as arrays.
4.) JSAnimation to display the Matplotlib animations of dispersal.

**Usage** 

To load your Circuitscape .asc file, please follow the 1_Upload_Filter_Circuitscape notebook.


**Author:** Meredith VanAcker<br/>**Affiliation:** Dept. of Ecology, Evolution & Environmental Biology, Columbia University<br/>**Contact:**  mv2640@columbia.edu

**Reference:**  <br/>(1) McRae, B. H., Dickson, B. G., Keitt, T. & Shah, V. B. Using Circuit Theory To Model Connectivity in Ecology, Evolution, and Conservation. Ecology 89, 2712–2724 (2008).


