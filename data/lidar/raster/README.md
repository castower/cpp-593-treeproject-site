- .tif files of LiDAR canopy height models. To load in R use the following code:

```

# install.packages( raster )

library( raster )

# Colorize pixels
col  <- height.colors( 50 )

# Read and plot 2333 tile raster CHM model
raster.2333 <- raster( here("data/lidar/raster/2333.tif") )
plot( raster.2333, col = col )

# Read and plot 2433 tile raster CHM model
raster.2433 <- raster( here("data/lidar/raster/2433.tif") )
plot( raster.2433, col = col )

```
