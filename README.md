
# cpp-593-treeproject-site
Website for CPP 593 Applied Project at Arizona State University: [https://castower.github.io/cpp-593-treeproject-site](https://castower.github.io/cpp-593-treeproject-site/#top)

An online step-by-step resource guide for conducting remote tree censuses using LiDAR data with R and other open-source software tools.

The following packages are needed:

```
# Install Packages

install.packages( "here" )
install.packages( "lidR" )
install.packages( "rLiDAR" )
install.pacakges( "raster" )
install.packages( "sp" )
install.packages( "ggmap" )
install.packages( "measurements" )
install.packages( "kableExtra" )
install.packages( "tidyverse" )
```

```
# Library

library( "here" )         # Used to create relative file paths so that code is reproducible
library( "lidR" )         # Used for LiDAR file processing
library( "rLiDAR" )       # Used for LiDAR file processing
library( "raster" )       # Used for raster file processing
library( "sp" )           # Used for mapping and spatial data processing
library( "ggmap" )        # Used for mapping and spatial data processing
library( "measurements" ) # Used to convert measurement units
library( "kableExtra" )   # Used to format tables
library( "tidyverse" )    # Used for manipulating data and packages
```

The LiDAR data set was accessed from Arizona State University Library’s [Map and Geospatial Hub](https://lib.asu.edu/geo). Tiles 2333.tif and 2433.tif from the Phoenix, Arizona USGS data set are used in the code-through. You can view details [here](https://lib.asu.edu/geo/news/robust-usgs-lidar-data-now-available).
