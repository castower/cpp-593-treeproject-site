---
title: " "
layout: single
classes: wide
header:
  overlay_filter: "0.5"
  overlay_image: /assets/images/tree-image-1.jpg #/assets/images/unsplash-image-1.jpg
  # image: /assets/images/tree-image-1.jpg #/assets/images/unsplash-image-1.jpg
  caption: "Photo credit: [Pascal Meier, **Unsplash**](https://unsplash.com/photos/sLnRjI0B4_w)" # "Photo credit: [**Unsplash**](https://unsplash.com)"
intro: 
  - excerpt: '<i markdown="1"> “Trees are right at the heart of all the necessary debates: ecological, social, economic, political, moral, religious.”
    ― [Colin Tudge](http://www.colintudge.com/) </i>'
sidebar:
  nav: "nav"
---

{% include feature_row id="intro" type="center" %}

<style type="text/css">
  
#masthead a:link {
  color: #fff;
  background-color: transparent;
  text-decoration: none;
}

</style>

<center> 
  <h1 id = "Introduction">Introduction</h1>
</center>

  <p> As the previous quote by Colin Tudge, author of <i>The Tree </i> espouses, trees play an essential role in the daily lives of humans, animals, and plants. Recent research on the widespread benefits of trees in a myriad of areas from environmental to physical to socioeconomic well-being has led policymakers to become advocates for eliminating “concrete jungles” in their cities and expanding tree canopy coverage through the planting of urban forests and other green spaces (“Benefits of trees”, 2019; Endreny, 2018; Kabisch et al., 2017).</p>
  
  <p> Early studies on these initiatives by environmental experts have found that urban forests reduce carbon emissions and mitigate global warming (Johnson et al., 2013; Malmsheimer et al., 2011; McPherson & Simpson, 1999; Russo et al., 2015; Zhao et al., 2010; Zheng et al., 2013). For example, a 2011 study conducted by the U.S. Forest Service iterated that that reducing greenhouse gases in the environment requires the creation of new forests (Malmsheimer et al., 2011), while an earlier study by McPherson & Simpson (1999) specifically focused on providing a guide for conservationists and business/industry executives to increase tree canopy coverage in communities and offset carbon dioxide emissions. Other studies such as those conducted by Johnson et al. (2013) and Russo et al. (2015) suggested urban forests as a way to reduce the effects of transportation on climate change and research by Zhao et al. (2010) and Zheng et al. (2013) provided overarching summaries of the benefits of urban forests. </p>

   <p> Similarly, investigations performed by socioeconomic and public health researchers have simultaneously espoused that trees and urban green spaces have a positive correlation with health and well-being in human living environments (Daams & Veneri, 2016; Dadvand et al., 2014; Dadvand et al., 2018; De Vries et al., 2007; Donovan, 2017; Faber Taylor & Kuo, 2011; King et al., 2015; Reid et al., 2017; Taylor et al., 1998; Turner‐Skoff & Cavender, 2019; U.S. Department of Agriculture, Forest Service, 2018; Ulmer et al., 2016). Studies by Dadvand et al (2014), Dadvand et al. (2018), Faber Taylor & Kuo (2011), Kabisch et al. (2017), Reid et al. (2017), the U.S. Department of Agriculture, Forest Service (2018), and Ulmer et al. (2016) all found that urban green spaces have significant benefits on the physical and mental health and well-being of individuals, particularly those who suffer from chronic illnesses and developmental difficulties such as obesity, asthma, allergies, diabetes, and ADHD. Other research by De Vries et al. (2007) and King et al. (2015) explore urban forests as outlets for safe play in inner-city areas while Turner et al. (2019) highlighted that trees are important for creating sustainable living environments. </p>
  
  <p> Following these scientific findings, cities have begun the task of creating databases to identify where trees are currently located in their communities and identify where new urban forests are needed (Poon, 2018).  However, the financial and human capital required to create these databases, known as tree censuses, are substantial (Poon, 2018).</p>
  
  <p> The city-wide TreesCount! census that was conducted in New York City, required 12,000 volunteer hours from 2,200 citizen mappers who were trained to utilize “high tech mapping tools with survey wheels, tape measures, and tree identification keys” according to a method developed by a non-profit organization, TreeKIT (“TreesCount!”, 2017). This volunteer work saved the city over $100,000 in survey costs, however even with such a large amount of volunteer hours, it took almost a year and a half to complete the census (“TreesCount!”, 2017). Although this was an intuitive way to save money and help “citizen mappers” and “citizen scientists” discover the importance of trees, many organizations do not have access to such a large pool of volunteers and/or are unable to wait years for results (Butt et al., 2013; Poon, 2018, “TreesCount!”, 2017). Therefore, cities and nonprofit groups are in dire need of a secondary assessment method that is quicker, less labor-intensive, and more affordable. </p>
  
  <p> In recent years, remote spatial data analysis tools have emerged as a viable option (Li et al., 2019; Lin et al., 2015; Ren et al., 2015; Tigges & Lakes, 2017). Remote spatial data analysis is a broad field that relies on unmanned aerial vehicles (UAV) and remote sensing (RS) techniques to combine high-quality optical images and LiDAR data into a "fast, replicable, objective, efficient, scalable, and cost-effective way to assess and quantify urban forest dynamics at varying spatiotemporal scales” (Li et al., 2019, p. 2; Lin et al., 2015; Poon, 2018; Tigges & Lakes, 2017). Research conducted by Li et al. (2019) and Poon (2018) explored the importance of improving methods to quantify urban forests while other analyses such as those conducted by Lin et al. (2015), Ren et al. (2015) and Tigges & Lakes (2017), have examined the strengths and limitations of available software. </p>
  
  <p> One area of consensus, though, is that the relatively cost-effective nature of these technologies make them into an important area of future research and an invaluable tool that is particularly attractive to advocates for open-data initiatives (Silva et al, 2018). Subsequently, these researchers have designed several software packages for the open-source data analysis language R (Silva et al., 2018).  It is the goal of this project to examine these software packages and produce a guide that determines the current feasibility of conducting remote tree censuses in an open-source format when the appropriate LiDAR data is available. </p>

<hr>

<br>

<center> 
  <h1 id = "Tools">Remote Tree Census Tools</h1>
</center>

  <p markdown= "1"> Although the field of remote tree identification is relatively new (the first R package for LiDAR data analysis was developed in [2014](https://www.researchgate.net/publication/324437694_LiDAR_Analysis_in_R_and_rLiDAR_for_Forestry_Applications)), the number of open-source tools available has expanded quickly. In this tutorial, we will be examining the tools available to conduct tree censuses with LiDAR data in R/RStudio. </p>

<center>
  <h2 id = "LIDAR">LiDAR</h2>
</center>

  <h3 markdown= "1"> **What is LiDAR data?** </h3>
  
  <p markdown= "1"> LiDAR is an acronym for _**Light Detection And Ranging**_. </p>
  
  <p markdown= "1"> The National Ocean Service of the [National Oceanic and Atmospheric Administration (NOAA)](https://oceanservice.noaa.gov/facts/lidar.html) describes it as "a remote sensing method that uses light in the form of a pulsed laser to measure ranges (variable distances) to the Earth. These light pulses—combined with other data recorded by the airborne system — generate precise, three-dimensional information about the shape of the Earth and its surface characteristics...[t]opographic lidar typically uses a near-infrared laser to map the land." </p> 
  
  <p markdown= "1"> Further, the NOAA explains the process of collecting LiDAR data in the following way: </p>

  <blockquote markdown= "1">
  When an airborne laser is pointed at a targeted area on the ground, the beam of 
  light is reflected by the surface it encounters. A sensor records this reflected light
  to measure a range. When laser ranges are combined with position and orientation data
  generated from integrated GPS and Inertial Measurement Unit systems, scan angles, and
  calibration data, the result is a dense, detail-rich group of elevation points, called
  a "point cloud."

  Each point in the point cloud has three-dimensional spatial coordinates (latitude,
  longitude, and height) that correspond to a particular point on the Earth's surface
  from which a laser pulse was reflected. The point clouds are used to generate other
  geospatial products, such as digital elevation models, canopy models, building models,
  and contours.
  </blockquote>

  <p markdown= "1"> You can read more on the NOAA website [here](https://oceanservice.noaa.gov/facts/lidar.html). </p>
  
  <p> The following websites provide access to free, publicly available LiDAR data sets: </p>
  
  <p>
  <ul>
  <li> <a href="https://www.geoplatform.gov/">GeoPlatform.gov</a></li> 
  <li> <a href="https://catalog.data.gov/dataset/lidar-point-cloud-usgs-national-map">Data.gov</a> </li>
  <li> <a href="https://www.usgs.gov/faqs/what-lidar-data-and-where-can-i-download-it?qt-news_science_products=0#qt-news_science_products">USGS.gov</a> </li>
  </ul>
  </p>
  
  
<br>

<center> 
  <h2 id = "R_RStudio">R and RStudio</h2> 
</center>

  <h3 markdown= "1">**What is R?**</h3>
  
<center>  
  <img src="data/website/tree-project_files/Rlogo.png" width="150" height="150">
</center>

<br>
  
  <p markdown="1"> **R** is an open-source programming environment that was developed for statistical and graphical analysis. The functionality of the environment is easily extended through the installation of software packages that can perform a wide variety of analyses. </p>
  
  <p markdown= "1"> You can read more about R and download the software from the Comprehensive R Archive Network **(CRAN)** for installation on a Linux, Mac OS X, or Windows device by clicking [here](https://www.r-project.org/about.html). </p>
  
  
<br>

  <h3 markdown= "1"> **What is RStudio?** </h3>
  
<center>  

  <img src="data/website/tree-project_files/RStudio-Logo-Flat.png" width="300" height="150">

</center>

<br>
  
  <p markdown= "1"> **RStudio Desktop** is an open-source software that provides a graphical user interface to run R code and create a variety of document types (such as .html, markdown, .pdf, .docx) that include R code and output. </p>
  
  <p markdown = "1"> You can learn more about the software and install it on your device by clicking [here](https://rstudio.com/index2/). </p>
  
  
<br>

<center>  
  <h1 id= "Remote_Tree_Census">Remote Tree Census Code-Through</h1>
</center>

  <p> The following steps will guide you through the process of setting up RStudio and conducting the tree census. </p> 

  <h2 id="SetUp">Set-Up</h2>
  <p> Once you have R and RStudio installed, open RStudio and create a new file of your choice. You may find it easiest to create an RMarkdown file as displayed below: </p>
  
  <center>
  <img src="data/website/tree-project_files/screenshot-01.png">
  </center>
  
  <br>
  
  <p> If you select the RMarkdown option, you will get the following dialog box: </p>
  
  <center>
  <img src="data/website/tree-project_files/screenshot-02.png">
  </center>
  
  <br>
  
  <p markdown="1"> Select the option of your choice for document type. You can change this selection later using any of the multitude of RMarkdown output formats detailed [here](https://rmarkdown.rstudio.com/formats.html). This document was created using the Github document option: </p>
  
  <center>
 <img src="data/website/tree-project_files/screenshot-03.png">
 </center>
  
  
<br>

  <h2 id= "Packages">Packages</h2>
  
  <h3 markdown="1">**Installation**</h3>
  
  <p> Once RStudio is set up, copy and paste the following code into the Console to install the packages that we will need for the tree census: </p>
  
<center>  
  <img src="data/website/tree-project_files/screenshot-04.png">
</center>  

<br>

``` r
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

<br>

<p markdown="1"> Another option is to use the insert button to create an R Code chunk that you will copy and paste the code into and run once. After the packages are installed, add `eval=FALSE` to the top of the code chunk. </p>

<center>  
  <img src="data/website/tree-project_files/screenshot-05.png">
</center> 

<br>

<center>
<img src="data/website/tree-project_files/screenshot-06.png">
</center>

<br>

 <h3 markdown="1">**Library**</h3>
 
 <p markdown="1"> Once the packages are installed, add them to a code chunk in your RMarkdown file using the `library()` function: </p>
 
 ``` r
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

<p markdown="1"> Although there are a wide variety of packages available for processing geospatial and LiDAR data in R, these selected packages are user-friendly and capable of analyzing the data in its raw form. Some other packages such as `ForestTools` require some pre-processing of the data. We will be working with a raw data set in this tutorial and coding all height models directly in R. </p>

<p markdown="1"> The documentation and reference manuals for the packages are available on **CRAN**: </p>

- [here](https://CRAN.R-project.org/package=here)
- [lidR](https://CRAN.R-project.org/package=lidR)
- [rLiDAR](https://CRAN.R-project.org/package=rLiDAR)
- [raster](https://CRAN.R-project.org/package=raster)
- [sp](https://CRAN.R-project.org/package=sp)
- [ggmap](https://CRAN.R-project.org/package=ggmap)
- [measurements](https://CRAN.R-project.org/package=measurements)
- [kableExtra](https://CRAN.R-project.org/package=kableExtra)
- [tidyverse](https://CRAN.R-project.org/package=tidyverse)


<h2 id= "Data">Data</h2>
  
  <p> Now that we have RStudio set up and our needed packages installed, we need to load our LiDAR data set.</p>
  
  <p markdown="1"> For this tutorial we will be using a set of LiDAR point clouds from Phoenix, Arizona that was collected by the USGS. We retrieved this data set from the Arizona State University Library's [Map and Geospatial Hub](https://lib.asu.edu/geo). A filtered version of the file is available in the Github repository for this site [here](https://github.com/castower/cpp-593-treeproject-site). </p>

  <p markdown="1"> **Note:** LiDAR data sets can be relatively large. Ensure that you have the storage and processing capacity to run the required analysis. For this tutorial, the [ASU Research Computing Facilities' supercomputer](https://cores.research.asu.edu/research-computing/about-rc) was used to configure an RStudio session with **R version 3.6.2** and **6 CPU Cores**. In addition, a sufficient amount of RAM is needed. A minimum of 4GB RAM and fewer CPU cores may be used, but you will need to allot time for delayed processing. [Click here](https://info.vercator.com/blog/how-to-overcome-large-datasets-in-point-cloud-processing) and [here](https://www.fs.fed.us/pnw/pubs/pnw_gtr768.pdf) for articles that provide suggestions for appropriate computer configurations. </p>
  
  
 <h3 markdown="1">**Data Download**</h3>
 
 <p> First, you need to ensure that you have your data downloaded and stored in a clearly labeled file for easy reference during your coding process. </p>
 
 <p> Depending on where your data is stored, the code needed for download may vary. The data set used for this tutorial was stored in Dropbox and the following code was used: </p>
 
 ``` r
# Download LAS LiDAR data

# 2333 tile
download.file( "dropbox_link_here", 
              "./data/lidar/las-points/lidar_2333_usgs_2014.las" )



# 2433 tile
download.file( "dropbox_link_here", 
              "./data/lidar/las-points/lidar_2433_usgs_2014.las" )
```

 <p markdown="1"> Dropbox is an excellent tool for hosting larger data sets. You can find tips on importing data from Dropbox into R [here](https://github.com/lecy/Import-Data-Into-R/blob/master/import%20from%20dropbox.md). </p>
 
 <p markdown="1"> **Note:** Some operating systems and/or wifi speeds may have trouble with downloading the entire LAS files from Dropbox. Double check that file sizes match the original source. </p> 

  
 <h3 markdown="1">**Data Exploration**</h3>
  
 <p> To load the data we will use the following code: </p>
 
 ``` r
LASfile <-  here( "data/lidar/las-points/lidar_2333_usgs_2014.las" )
las <- lidR::readLAS( LASfile )

LASfile2 <- here( "data/lidar/las-points/lidar_2433_usgs_2014.las" )
las2 <- lidR::readLAS( LASfile2 )
```

<p markdown="1"> The `here()` function stores the LiDAR data into the `LASfile` variable. This variable is then used with the `lidR` package function `readLAS` to properly import the LiDAR point cloud data. </p>

<p> Next, we can use base R functions to explore the LiDAR data sets further. For the purposes of the tutorial, we will summarize our first data set: </p>

``` r
summary( las )  # 11.25 million points over 1.04 km^2
```

    ## class        : LAS (v1.2 format 1)
    ## memory       : 858.3 Mb 
    ## extent       : 397990, 399010, 3704990, 3706010 (xmin, xmax, ymin, ymax)
    ## coord. ref.  : +proj=utm +zone=12 +datum=NAD83 +units=m +no_defs +ellps=GRS80 +towgs84=0,0,0 
    ## area         : 1.04 km²
    ## points       : 11.25 million points
    ## density      : 10.81 points/m²
    ## File signature:           LASF 
    ## File source ID:           0 
    ## Global encoding:
    ##  - GPS Time Type: Standard GPS Time 
    ##  - Synthetic Return Numbers: no 
    ##  - Well Know Text: CRS is GeoTIFF 
    ##  - Aggregate Model: false 
    ## Project ID - GUID:        00000000-0000-0000-0000-000000000000 
    ## Version:                  1.2
    ## System identifier:         
    ## Generating software:      TerraScan 
    ## File creation d/y:        290/2014
    ## header size:              227 
    ## Offset to point data:     513 
    ## Num. var. length record:  3 
    ## Point data format:        1 
    ## Point data record length: 28 
    ## Num. of point records:    11250194 
    ## Num. of points by return: 10933801 303379 12794 220 0 
    ## Scale factor X Y Z:       0.001 0.001 1e-05 
    ## Offset X Y Z:             397990 3704990 329.04 
    ## min X Y Z:                397990 3704990 329.04 
    ## max X Y Z:                399010 3706010 363.8 
    ## Variable length records: 
    ##    Variable length record 1 of 3 
    ##        Description: GeoTiff GeoKeyDirectoryTag 
    ##        Tags:
    ##           Key 1024 value 1 
    ##           Key 1025 value 1 
    ##           Key 1026 value 0 
    ##           Key 2049 value 21 
    ##           Key 2054 value 9102 
    ##           Key 2062 value 0 
    ##           Key 3072 value 26912 
    ##           Key 3076 value 9001 
    ##    Variable length record 2 of 3 
    ##        Description: GeoTiff GeoDoubleParamsTag 
    ##        data:                 0 0 0 
    ##    Variable length record 3 of 3 
    ##        Description: GeoTiff GeoAsciiParamsTag 
    ##        data:                 NAD83 / UTM zone 12N|NAD83|


<p> The summary output indicates the size of each pixel in the LAS file and indicates that there are 11.25 million points spread over 1.04 km^2 </p>

``` r
# 1,000 meter by 1,000 meter area
sqrt( 11250000 ) # 11,250,000 points
```

    ## [1] 3354.102

``` r
# 3,354 pixels per side 
```

<p> The square root function further breaks down the analysis to indicate that in a 1,000 meter by 1,000 meter area there are 3,354 pixels per side. </p>

``` r
# pixel to area
# 1,000 meters / 3,354 pixels 
1000/3354
```

    ## [1] 0.2981515

``` r
# 0.30 meters per pixel ~ one foot per pixel 
```

<p> We can then divide the area by the pixels to find that there are approximately .30 meters per pixel in the data set. In the United States Customary System (USCS) of measurements, this is equivalent to approx. 1 foot per pixel. </p>

<h2 id="Identification">Tree Identification</h2>

<p> In order to conduct a tree census, we must first identify individual trees. To accomplish this, we need to normalize the heights of the LAS files, colorize the pixels, and create a Canopy Height Model. </p>

<p markdown="1"> The [Canopy Height Model (CHM)](https://www.earthdatascience.org/courses/earth-analytics/lidar-raster-data-r/lidar-chm-dem-dsm/) finds the distance of objects from the ground and will serve as a measurement tool for analysis. </p>

``` r
# Tree identification for 2433 tile

las2  <- normalize_height( las2, tin() )               # Normalize heights
col  <- height.colors( 50 )                            # Colorize pixels
chm2  <- lidR::grid_canopy( las2, res = 1, p2r() )     # Create Canopy Height Model
```

``` r
# Plot Canopy Height Model

plot( chm2, col = col )
```

<center>

<img src="data/website/tree-project_files/figure-gfm/unnamed-chunk-6-1.png">

</center>

<br>

<p> This plot displays the heights of the various items in the LiDAR data tile. Flat areas with a height of 0 meters are displayed in dark blue while tall areas with a height up to 30 meters are displayed in red. </p>

<p markdown="1"> The `lidR` package's `grid_canopy()` function provides several [graphing options](https://github.com/Jean-Romain/lidR/wiki/Rasterizing-perfect-canopy-height-models) that can change the appearance of the plot: </p>


``` r
chm2  <- lidR::grid_canopy( las2, res = 0.5, p2r() ) # alter the resolution to 0.5
plot( chm2, col = col )
```

<center>

<img src="data/website/tree-project_files/figure-gfm/unnamed-chunk-7-1.png">

</center>

<br>

<p> This reduction in the resolution worsens the plot </p>


``` r
chm2  <- lidR::grid_canopy( las2, res = 0.5, p2r(0.2) ) # adjust the points-to-raster algorithm's circle size
plot( chm2, col = col )
```

<center>

<img src="data/website/tree-project_files/figure-gfm/unnamed-chunk-8-1.png">

</center>

<br>

<p> Adjusting the points-to-raster algorithm's circle size slightly improves the graph, but keeps some holes in the plot. </p>

``` r
chm2  <- lidR::grid_canopy( las2, res = 2, p2r() ) # alter the resolution to 2
plot( chm2, col = col )
```

<center>

<img src="data/website/tree-project_files/figure-gfm/unnamed-chunk-9-1.png">

</center>

<br>

<p> This improves the resolution of the plot, but some holes still remain. </p>

``` r
chm2  <- lidR::grid_canopy( las2, res = 2, p2r(0.5) ) # alter the resolution and points-to-raster configurations
plot( chm2, col = col )
```

<center>

<img src="data/website/tree-project_files/figure-gfm/unnamed-chunk-10-1.png">

</center>

<br>

<p markdown="1"> This slightly increases the plot, but there are still some unclear plots. Therefore, we will try the package's `pitfree()` function: </p>

<p markdown="1"> **Note:** This function is more computationally demanding than the p2r and triangulation based methods that are available in the package's documentation. </p>

``` r
chm2  <- lidR::grid_canopy(las2, 0.25, pitfree(c(0,2,5,10,15), c(0,1), subcircle = 0.2))
```

``` r
# Pitfree plot

plot( chm2, col = col )
```

<center>

<img src="data/website/tree-project_files/figure-gfm/unnamed-chunk-12-1.png">

</center>

<br>

<p> This plot contains very few white spaces and provides a clear colorized analysis of the heights present in the tile. </p>

``` r
# Find heights of objects in tile that are at least 1.37 meters tall

trees2 <- FindTreesCHM( chm2 ) # function from rLiDAR package
head( trees2 ) %>% kable() %>% kable_styling() # Create table of data
```
<center>
<table class="table" style="margin-left: auto; margin-right: auto;">

<thead>

<tr>

<th style="text-align:right;"> x </th>

<th style="text-align:right;"> y </th>

<th style="text-align:right;"> height </th>

</tr>

</thead>

<tbody>

<tr>

<td style="text-align:right;"> 398400.6 </td>

<td style="text-align:right;"> 3705009 </td>

<td style="text-align:right;"> 3.565190 </td>

</tr>

<tr>

<td style="text-align:right;"> 398401.9 </td>

<td style="text-align:right;"> 3705009 </td>

<td style="text-align:right;"> 3.421995 </td>

</tr>

<tr>

<td style="text-align:right;"> 398523.9 </td>

<td style="text-align:right;"> 3705009 </td>

<td style="text-align:right;"> 2.164520 </td>

</tr>

<tr>

<td style="text-align:right;"> 398578.6 </td>

<td style="text-align:right;"> 3705009 </td>

<td style="text-align:right;"> 7.366430 </td>

</tr>

<tr>

<td style="text-align:right;"> 398705.1 </td>

<td style="text-align:right;"> 3705009 </td>

<td style="text-align:right;"> 4.276970 </td>

</tr>

<tr>

<td style="text-align:right;"> 398713.9 </td>

<td style="text-align:right;"> 3705009 </td>

<td style="text-align:right;"> 4.272560 </td>

</tr>

</tbody>

</table>

</center>


<p> After we find the heights of objects in meters, we can also find the measures in feet: </p>

``` r
# Create measures in feet and meters 

colnames( trees2 ) <- c( "x", "y", "height_meter" ) # rename column to designate meters

head( trees2 ) %>% kable() %>% kable_styling() # preview data set with new column titles
```
<center>

<table class="table" style="margin-left: auto; margin-right: auto;">

<thead>

<tr>

<th style="text-align:right;"> x </th>

<th style="text-align:right;"> y </th>

<th style="text-align:right;"> height_meter </th>

</tr>

</thead>

<tbody>

<tr>

<td style="text-align:right;"> 398400.6 </td>

<td style="text-align:right;"> 3705009 </td>

<td style="text-align:right;"> 3.565190 </td>

</tr>

<tr>

<td style="text-align:right;"> 398401.9 </td>

<td style="text-align:right;"> 3705009 </td>

<td style="text-align:right;"> 3.421995 </td>

</tr>

<tr>

<td style="text-align:right;"> 398523.9 </td>

<td style="text-align:right;"> 3705009 </td>

<td style="text-align:right;"> 2.164520 </td>

</tr>

<tr>

<td style="text-align:right;"> 398578.6 </td>

<td style="text-align:right;"> 3705009 </td>

<td style="text-align:right;"> 7.366430 </td>

</tr>

<tr>

<td style="text-align:right;"> 398705.1 </td>

<td style="text-align:right;"> 3705009 </td>

<td style="text-align:right;"> 4.276970 </td>

</tr>

<tr>

<td style="text-align:right;"> 398713.9 </td>

<td style="text-align:right;">

3705009

</td>

<td style="text-align:right;"> 4.272560 </td>

</tr>

</tbody>

</table>

</center>

``` r
trees2$height_ft <- conv_unit( trees2$height_meter, "m", "ft"  ) # create column with tree heights in feet

head( trees2 ) %>% kable() %>% kable_styling() # view new data set with measures in feet
```
<center>
<table class="table" style="margin-left: auto; margin-right: auto;">

<thead>

<tr>

<th style="text-align:right;"> x </th>

<th style="text-align:right;"> y </th>

<th style="text-align:right;"> height_meter </th>

<th style="text-align:right;"> height_ft </th>

</tr>

</thead>

<tbody>

<tr> 

<td style="text-align:right;"> 398400.6 </td>

<td style="text-align:right;"> 3705009 </td>

<td style="text-align:right;"> 3.565190 </td>

<td style="text-align:right;"> 11.696818 </td>

</tr>

<tr>

<td style="text-align:right;"> 398401.9 </td>

<td style="text-align:right;"> 3705009 </td>

<td style="text-align:right;"> 3.421995 </td>

<td style="text-align:right;"> 11.227019 </td>

</tr>

<tr>

<td style="text-align:right;"> 398523.9 </td>

<td style="text-align:right;"> 3705009 </td>

<td style="text-align:right;"> 2.164520 </td>

<td style="text-align:right;"> 7.101444 </td>

</tr>

<tr>

<td style="text-align:right;"> 398578.6 </td>

<td style="text-align:right;"> 3705009 </td>

<td style="text-align:right;"> 7.366430 </td>

<td style="text-align:right;"> 24.168077 </td>

</tr>

<tr>

<td style="text-align:right;"> 398705.1 </td>

<td style="text-align:right;"> 3705009 </td>

<td style="text-align:right;"> 4.276970 </td>

<td style="text-align:right;"> 14.032054 </td>

</tr>

<tr>

<td style="text-align:right;"> 398713.9 </td>

<td style="text-align:right;"> 3705009 </td>

<td style="text-align:right;"> 4.272560 </td>

<td style="text-align:right;"> 14.017585 </td>

</tr>

</tbody>

</table>

</center>


<p> Now we will repeat these steps for our 2333 tile: </p> 

``` r
# Tree identification for 2333 tile

# Normalize heights
las  <- normalize_height( las, tin() )

# Colorize pixels
col  <- height.colors( 50 )

# Create Canopy Height Model
chm  <- lidR::grid_canopy( las, 0.25, pitfree(c(0,2,5,10,15), c(0,1), subcircle = 0.2) )
```

``` r
# Plot 2333 tile

plot(chm, col = col)
```

<center>

<img src="data/website/tree-project_files/figure-gfm/unnamed-chunk-16-1.png">

</center>

<br>

``` r
# Find trees

trees <- FindTreesCHM( chm )

head( trees ) %>% kable() %>% kable_styling()
```

<center>
  
<table class="table" style="margin-left: auto; margin-right: auto;">

<thead>

<tr>

<th style="text-align:right;"> x </th>

<th style="text-align:right;"> y </th>

<th style="text-align:right;"> height </th>

</tr>

</thead>

<tbody>

<tr>

<td style="text-align:right;"> 398074.1 </td>

<td style="text-align:right;"> 3706009 </td>

<td style="text-align:right;"> 7.155665 </td>

</tr>

<tr>

<td style="text-align:right;"> 398102.9 </td>

<td style="text-align:right;"> 3706009 </td>

<td style="text-align:right;"> 5.658660 </td>

</tr>

<tr>

<td style="text-align:right;"> 398103.1 </td>

<td style="text-align:right;"> 3706009 </td>

<td style="text-align:right;"> 5.658660 </td>

</tr>

<tr>

<td style="text-align:right;"> 398108.4 </td>

<td style="text-align:right;"> 3706009 </td>

<td style="text-align:right;"> 5.650502 </td>

</tr>

<tr>

<td style="text-align:right;"> 398126.6 </td>

<td style="text-align:right;"> 3706009 </td>

<td style="text-align:right;"> 11.269140 </td>

</tr>

<tr>

<td style="text-align:right;"> 398130.9 </td>

<td style="text-align:right;"> 3706009 </td>

<td style="text-align:right;"> 8.827670 </td>

</tr>

</tbody>

</table>

</center>

``` r
# Create measures in feet and meters 

colnames( trees ) <- c( "x", "y", "height_meter" ) # rename column to designate meters

head( trees ) %>% kable() %>% kable_styling() # preview data set with new column titles
```

<center>

<table class="table" style="margin-left: auto; margin-right: auto;">

<thead>

<tr>

<th style="text-align:right;"> x </th>

<th style="text-align:right;"> y </th>

<th style="text-align:right;"> height_meter </th>

</tr>

</thead>

<tbody>

<tr>

<td style="text-align:right;"> 398074.1 </td>

<td style="text-align:right;"> 3706009 </td>

<td style="text-align:right;"> 7.155665 </td>

</tr>

<tr>

<td style="text-align:right;"> 398102.9 </td>

<td style="text-align:right;"> 3706009 </td>

<td style="text-align:right;"> 5.658660 </td>

</tr>

<tr>

<td style="text-align:right;"> 398103.1 </td>

<td style="text-align:right;"> 3706009 </td>

<td style="text-align:right;"> 5.658660 </td>

</tr>

<tr>

<td style="text-align:right;"> 398108.4 </td>

<td style="text-align:right;"> 3706009 </td>

<td style="text-align:right;"> 5.650502 </td>

</tr>

<tr>

<td style="text-align:right;"> 398126.6 </td>

<td style="text-align:right;"> 3706009 </td>

<td style="text-align:right;"> 11.269140 </td>

</tr>

<tr>

<td style="text-align:right;"> 398130.9 </td>

<td style="text-align:right;"> 3706009 </td>

<td style="text-align:right;"> 8.827670 </td>

</tr>

</tbody>

</table>

</center>

``` r
trees$height_ft <- conv_unit( trees$height_meter, "m", "ft"  ) # create column with tree heights in feet

head( trees ) %>% kable() %>% kable_styling() # view data set with measures in feet
```

<center>
<table class="table" style="margin-left: auto; margin-right: auto;">

<thead>

<tr>

<th style="text-align:right;"> x </th>

<th style="text-align:right;"> y </th>

<th style="text-align:right;"> height_meter </th>

<th style="text-align:right;"> height_ft </th>

</tr>

</thead>

<tbody>

<tr>

<td style="text-align:right;"> 398074.1 </td>

<td style="text-align:right;"> 3706009 </td>

<td style="text-align:right;"> 7.155665 </td>

<td style="text-align:right;"> 23.47659 </td>

</tr>

<tr>

<td style="text-align:right;"> 398102.9 </td>

<td style="text-align:right;"> 3706009 </td>

<td style="text-align:right;"> 5.658660 </td>

<td style="text-align:right;"> 18.56516 </td>

</tr>

<tr>

<td style="text-align:right;"> 398103.1 </td>

<td style="text-align:right;"> 3706009 </td>

<td style="text-align:right;"> 5.658660 </td>

<td style="text-align:right;"> 18.56516 </td>

</tr>

<tr>

<td style="text-align:right;"> 398108.4 </td>

<td style="text-align:right;"> 3706009 </td>

<td style="text-align:right;"> 5.650502 </td>

<td style="text-align:right;"> 18.53839 </td>

</tr>

<tr>

<td style="text-align:right;"> 398126.6 </td>

<td style="text-align:right;"> 3706009 </td>

<td style="text-align:right;"> 11.269140 </td>

<td style="text-align:right;"> 36.97224 </td>

</tr>

<tr>

<td style="text-align:right;"> 398130.9 </td>

<td style="text-align:right;"> 3706009 </td>

<td style="text-align:right;"> 8.827670 </td>

<td style="text-align:right;"> 28.96217 </td>

</tr>

</tbody>

</table>

</center>


<p> Once we have our data set created, we can then narrow the area of the plot to create a sample area to conduct our remote tree census: </p>

``` r
# Create fixed square window size of 5 for an area to conduct a sample tree census
trees <- FindTreesCHM( chm, fws=5 )

# Create measures in feet and meters 

colnames( trees ) <- c( "x", "y", "height_meter" ) # rename column to designate meters

head( trees ) %>% kable() %>% kable_styling() # preview data set with new column titles
```

<center>
  
<table class="table" style="margin-left: auto; margin-right: auto;">

<thead>

<tr>

<th style="text-align:right;"> x </th>

<th style="text-align:right;"> y </th>

<th style="text-align:right;"> height_meter </th>

</tr>

</thead>

<tbody>

<tr>

<td style="text-align:right;"> 398074.1 </td>

<td style="text-align:right;"> 3706009 </td>

<td style="text-align:right;"> 7.155665 </td>

</tr>

<tr>

<td style="text-align:right;"> 398102.9 </td>

<td style="text-align:right;"> 3706009 </td>

<td style="text-align:right;"> 5.658660 </td>

</tr>

<tr>

<td style="text-align:right;"> 398103.1 </td>

<td style="text-align:right;"> 3706009 </td>

<td style="text-align:right;"> 5.658660 </td>

</tr>

<tr>

<td style="text-align:right;"> 398108.4 </td>

<td style="text-align:right;"> 3706009 </td>

<td style="text-align:right;"> 5.650502 </td>

</tr>

<tr>

<td style="text-align:right;"> 398126.6 </td>

<td style="text-align:right;"> 3706009 </td>

<td style="text-align:right;"> 11.269140 </td>

</tr>

<tr>

<td style="text-align:right;"> 398130.9 </td>

<td style="text-align:right;"> 3706009 </td>

<td style="text-align:right;"> 8.827670 </td>

</tr>

</tbody>

</table>

</center>

``` r
trees$height_ft <- conv_unit( trees$height_meter, "m", "ft"  ) # create column with tree heights in feet

head( trees ) %>% kable() %>% kable_styling() # view data set with measures in feet
```
<center>

<table class="table" style="margin-left: auto; margin-right: auto;">

<thead>

<tr>

<th style="text-align:right;"> x </th>

<th style="text-align:right;"> y </th>

<th style="text-align:right;"> height_meter </th>

<th style="text-align:right;"> height_ft </th>

</tr>

</thead>

<tbody>

<tr>

<td style="text-align:right;"> 398074.1 </td>

<td style="text-align:right;"> 3706009 </td>

<td style="text-align:right;"> 7.155665 </td>

<td style="text-align:right;"> 23.47659 </td>

</tr>

<tr>

<td style="text-align:right;"> 398102.9 </td>

<td style="text-align:right;"> 3706009 </td>

<td style="text-align:right;"> 5.658660 </td>

<td style="text-align:right;"> 18.56516 </td>

</tr>

<tr>

<td style="text-align:right;"> 398103.1 </td>

<td style="text-align:right;"> 3706009 </td>

<td style="text-align:right;"> 5.658660 </td>

<td style="text-align:right;"> 18.56516 </td>

</tr>

<tr>

<td style="text-align:right;"> 398108.4 </td>

<td style="text-align:right;"> 3706009 </td>

<td style="text-align:right;"> 5.650502 </td>

<td style="text-align:right;"> 18.53839 </td>

</tr>

<tr>

<td style="text-align:right;"> 398126.6 </td>

<td style="text-align:right;"> 3706009 </td>

<td style="text-align:right;"> 11.269140 </td>

<td style="text-align:right;"> 36.97224 </td>

</tr>

<tr>

<td style="text-align:right;"> 398130.9 </td>

<td style="text-align:right;"> 3706009 </td>

<td style="text-align:right;"> 8.827670 </td>

<td style="text-align:right;"> 28.96217 </td>

</tr>

</tbody>

</table>

</center>

``` r
summary( trees ) %>% kable() %>% kable_styling()
```
<center>

<table class="table" style="margin-left: auto; margin-right: auto;">

<thead>

<tr>

<th style="text-align:left;"> x </th>

<th style="text-align:left;"> y </th>

<th style="text-align:left;"> height_meter </th>

<th style="text-align:left;"> height_ft </th>

</tr>

</thead>

<tbody>

<tr>

<td style="text-align:left;"> Min. :397991 </td>

<td style="text-align:left;"> Min. :3704991 </td>

<td style="text-align:left;"> Min. : 1.495 </td>

<td style="text-align:left;"> Min. : 4.905 </td>

</tr>

<tr>

<td style="text-align:left;"> 1st Qu.:398277 </td>

<td style="text-align:left;"> 1st Qu.:3705224 </td>

<td style="text-align:left;"> 1st Qu.: 3.973 </td>

<td style="text-align:left;"> 1st Qu.:13.033 </td>

</tr>

<tr>

<td style="text-align:left;"> Median :398527 </td>

<td style="text-align:left;"> Median :3705425 </td>

<td style="text-align:left;"> Median : 4.925 </td>

<td style="text-align:left;"> Median :16.157 </td>

</tr>

<tr>

<td style="text-align:left;"> Mean :398527 </td>

<td style="text-align:left;"> Mean :3705468 </td>

<td style="text-align:left;"> Mean : 6.190 </td>

<td style="text-align:left;"> Mean :20.307 </td>

</tr>

<tr>

<td style="text-align:left;"> 3rd Qu.:398812 </td>

<td style="text-align:left;"> 3rd Qu.:3705732 </td>

<td style="text-align:left;"> 3rd Qu.: 7.770 </td>

<td style="text-align:left;"> 3rd Qu.:25.493 </td>

</tr>

<tr>

<td style="text-align:left;"> Max. :399009 </td>

<td style="text-align:left;"> Max. :3706009 </td>

<td style="text-align:left;"> Max. :27.568 </td>

<td style="text-align:left;"> Max. :90.445 </td>

</tr>

</tbody>

</table>

</center>


<p> We can save the raster file of the plot and the CSV file of tree height data with the following functions: </p>

``` r
# Save tree heights to CSV file

write.csv( trees, here("data/csv/trees_2333.csv") )

# Save Canopy Height Model to raster file

writeRaster( chm, here("data/lidar/raster/2333.tif") )
```

<p> To view the saved CSV file, we can run the following code: </p>

``` r
# Preview CSV file

head ( read.csv( here("data/csv/trees_2333.csv"), col.names = c("id", "x", "y", "height_meter", "height_ft"), stringsAsFactors = FALSE ) ) %>% kable() %>% kable_styling()
```

<center>
  
<table class="table" style="margin-left: auto; margin-right: auto;">

<thead>

<tr>

<th style="text-align:right;"> id </th>

<th style="text-align:right;"> x </th>

<th style="text-align:right;"> y </th>

<th style="text-align:right;"> height_meter </th>

<th style="text-align:right;"> height_ft </th>

</tr>

</thead>

<tbody>

<tr>

<td style="text-align:right;"> 1 </td>

<td style="text-align:right;"> 398074.1 </td>

<td style="text-align:right;"> 3706009 </td>

<td style="text-align:right;"> 7.155665 </td>

<td style="text-align:right;"> 23.47659 </td>

</tr>

<tr>

<td style="text-align:right;"> 2 </td>

<td style="text-align:right;"> 398102.9 </td>

<td style="text-align:right;"> 3706009 </td>

<td style="text-align:right;"> 5.658660 </td>

<td style="text-align:right;"> 18.56516 </td>

</tr>

<tr>

<td style="text-align:right;"> 3 </td>

<td style="text-align:right;"> 398103.1 </td>

<td style="text-align:right;"> 3706009 </td>

<td style="text-align:right;"> 5.658660 </td>

<td style="text-align:right;"> 18.56516 </td>

</tr>

<tr>

<td style="text-align:right;"> 4 </td>

<td style="text-align:right;"> 398108.4 </td>

<td style="text-align:right;"> 3706009 </td>

<td style="text-align:right;"> 5.650502 </td>

<td style="text-align:right;"> 18.53839 </td>

</tr>

<tr>

<td style="text-align:right;"> 5 </td>

<td style="text-align:right;"> 398126.6 </td>

<td style="text-align:right;"> 3706009 </td>

<td style="text-align:right;"> 11.269140 </td>

<td style="text-align:right;"> 36.97224 </td>

</tr>

<tr>

<td style="text-align:right;"> 6 </td>

<td style="text-align:right;"> 398130.9 </td>

<td style="text-align:right;"> 3706009 </td>

<td style="text-align:right;"> 8.827670 </td>

<td style="text-align:right;"> 28.96217 </td>

</tr>

</tbody>

</table>

</center>

<h2 id= "Mapping">Mapping Trees</h2>

<h3>Automatic</h3>

<p markdown="1"> Now that we have a **Canopy Height Model** raster file created, we can map our trees using the `sp` and `ggmap` packages. </p>

<p markdown="1"> **Note:** For this tutorial, we will use Google Maps to conduct our automated vs manual remote tree census comparison. However, since Google Maps are proprietary, to access them you must request an API code from [Google's Cloud Services](https://cloud.google.com/maps-platform/) and keep a credit card on record with Google. If you would like a completely open-source mapping option, ggmap also supports OpenStreetMap and Stamen Maps. Details on these mapping options are available [here](https://cfss.uchicago.edu/notes/raster-maps-with-ggmap/#obtain-map-images). </p>

<p> If you decide to use Google Maps, you will need to run the following code to register your API key before following the rest of the tutorial: </p>

```r

register_google(key = "[your API key]") # for temporary use of key

register_google(key = "[your API key]", write = TRUE) # for registering key in .Renviron file

```

<p markdown="1"> More details on ggmap's Google API key requirements can be found on the package's [Github repo](https://github.com/dkahle/ggmap#attention). </p>

<p markdown="1"> To begin the mapping process, first we must use the `sp` package to convert our LiDAR 3D point cloud dimensions into traditional latitude and longitude measurements. We will store these in the `lat.lon` variable: </p>

```r
coords <- trees[ c("x","y") ]
names( trees ) <- c("id", "x.meters","y.meters","height")
crs <- sp::CRS( "+proj=utm +zone=12 +datum=NAD83 +units=m +no_defs" )
df <- sp::SpatialPointsDataFrame( coords, proj4string=crs, data=trees ) 

df2 <- spTransform( df, CRS("+proj=longlat +datum=WGS84") )

lat.lon <- coordinates( df2 ) %>% as.data.frame()
lat.lon$height <- trees$height
```

<p> Next, we will use ggmap to plot the locations of our trees on a map: </p>

<hr>

<center>
  <h1 id = "References">References</h1>
</center>

- Arizona State University Map and Geospatial Hub. (n.d.). New web map for accessing Phoenix LiDAR data. Retrieved July 5, 2020, from [https://lib.asu.edu/Geo/news/New-Web-Map-Accessing-Phoenix-LiDAR-Data](https://lib.asu.edu/Geo/news/New-Web-Map-Accessing-Phoenix-LiDAR-Data) 

- ASU Research Computing. (n.d.). Retrieved July 5, 2020, from [https://cores.research.asu.edu/research-computing/about](https://cores.research.asu.edu/research-computing/about)

- Benefits of trees. (2019). <i>Nature Climate Change, 9</i>(8), 569–569. [doi:10.1038/s41558-019-0556-z](https://www.nature.com/articles/s41558-019-0556-z)
    
- Birk, M. A. (2019, May 28). measurements: Tools for Units of Measurement. Retrieved July 6, 2020, from [https://CRAN.R-project.org/package=measurements](https://CRAN.R-project.org/package=measurements)

- Butt, N., Slade, E., Thompson, J., Malhi, Y., & Riutta, T. (2013). Quantifying the sampling error in tree census measurements by volunteers and its effect on carbon stock estimates. <i> Ecological Applications, 23</i>(4), 936–943. [doi:10.1890/11-2059.1](https://esajournals.onlinelibrary.wiley.com/doi/abs/10.1890/11-2059.1)
    
- Daams, M. N. & Veneri, P.  (2016). Living near to attractive nature? A well-being indicator for ranking Dutch, Danish, and German functional urban areas. <i> [Social Indicators Research](https://link.springer.com/article/10.1007/s11205-016-1375-5), 133</i>(2), 501–526.
    
- Dadvand, P., Villanueva, C. M., Font-Ribera, L., Martinez, D., Basagaña, X., Belmonte, J., Vrijheid, M., Gražulevičiene, R., Kogevinas, M., & Nieuwenhuijsen, M. J. (2014). Risks and benefits of green spaces for children: A cross-sectional study of associations with sedentary behavior, obesity, asthma, and allergy. <i>Environmental Health Perspectives, 122</i>(12), 1329–1335. [doi:10.1289/ehp.1308038](https://ehp.niehs.nih.gov/doi/10.1289/ehp.1308038)
    
- Dadvand, P., Poursafa, P., Heshmat, R., Motlagh, M., Qorbani, M., Basagaña, X., & Kelishadi, R. (2018). Use of green spaces and blood glucose in children; a population-based CASPIAN-V study. <i>Environmental Pollution, 243</i>(Pt B), 1134–1140. [https://doi.org/10.1016/j.envpol.2018.09.094](https://doi.org/10.1016/j.envpol.2018.09.094) 
    
- De Vries, S. I., Bakker, I., Van Mechelen, W., & Hopman-Rock, M. (2007). Determinants of activity-friendly neighborhoods for children: Results from the SPACE study. <i>[American Journal of Health Promotion: AJHP](https://journals.sagepub.com/doi/10.4278/0890-1171-21.4s.312), 21</i>(4), 312–316.
    
- Donovan, G. (2017). Including public-health benefits of trees in urban-forestry decision making. <i>Urban Forestry & Urban Greening, 22</i>, 120–123. [https://doi.org/10.1016/j.ufug.2017.02.010](https://doi.org/10.1016/j.ufug.2017.02.010) 
    
- Endreny, T. (2018, April 27). The multi-million-dollar benefits of urban trees. Retrieved May 25, 2020, from [https://www.citylab.com/environment/2018/04/heres-how-much-money-trees-save-in-megacities/559211/](https://www.citylab.com/environment/2018/04/heres-how-much-money-trees-save-in-megacities/559211/)
    
- Faber Taylor, A., & Kuo, F. (2011). Could exposure to everyday green spaces help treat ADHD? Evidence from children’s play settings. <i>Applied Psychology: Health and Well‐Being, 3</i>(3), 281–303. [https://doi.org/10.1111/j.1758-0854.2011.01052.x](https://doi.org/10.1111/j.1758-0854.2011.01052.x) 
      
- Gatziolis, D. & Andersen, H. (2008). A guide to LIDAR data acquisition and processing for the forests of the Pacific Northwest. <i>United States Department of Agriculture Forest Service</i>. Retrieved July 5, 2020, from [https://www.fs.fed.us/pnw/pubs/pnw_gtr768.pdf](https://www.fs.fed.us/pnw/pubs/pnw_gtr768.pdf)

- Google. (n.d.). Google Cloud Maps Platform. Retrieved July 7, 2020, from [https://cloud.google.com/maps-platform/](https://cloud.google.com/maps-platform/)

- Google. (n.d.). Google MyMaps Creator. Retrieved July 7, 2020, from [https://www.google.com/maps/about/mymaps/](https://www.google.com/maps/about/mymaps/)

- Hijmans, R. J. et al. (2020, June 27). raster: Geographic Data Analysis and Modeling. Retrieved July 6, 2020, from [https://CRAN.R-project.org/package=raster ](https://CRAN.R-project.org/package=raster)

- Johnson, M., Gonzalez, A., Kozak, B., & Sperlak, L. (2013). Carbon estimation and offsets for U.S. university aviation programs. <i>Collegiate Aviation Review, 31</i>(1), 40–56. [https://doi.org/10.22488/okstate.18.100437](https://doi.org/10.22488/okstate.18.100437) 
      
- Kabisch, N., van den Bosch, M., & Lafortezza, R. (2017). The health benefits of nature-based solutions to urbanization challenges for children and the elderly – A systematic review. <i>Environmental Research, 159</i>, 362–373. [doi:10.1016/j.envres.2017.08.004](https://www.sciencedirect.com/science/article/abs/pii/S0013935117315396?via%3Dihub)
      
 - Kahle, D. (2019, May 11). ggmap Github Repository. Retrieved July 7, 2020, from [https://github.com/dkahle/ggmap](https://github.com/dkahle/ggmap)
 
 - Kahle, D. et al. (2019, February 5). ggmap: Spatial Visualization with ggplot2. Retrieved July 6, 2020, from [https://CRAN.R-project.org/package=ggmap](https://CRAN.R-project.org/package=ggmap)
 
 - King, D. K., Litt, J., Hale, J., Burniece, K. M., & Ross, C. (2015). “The park a tree built”: Evaluating how a park development project impacted where people play. <i>Urban Forestry & Urban Greening, 14</i>(2), 293–299. [doi:10.1016/j.ufug.2015.02.011](https://www.sciencedirect.com/science/article/abs/pii/S1618866715000291?via%3Dihub) 
      
 - Lecy, J. (2016, April 2). Load data files from Dropbox. Retrieved July 5, 2020, from [https://github.com/lecy/Import-Data-Into-R/blob/master/import%20from%20dropbox.md](https://github.com/lecy/Import-Data-Into-R/blob/master/import%20from%20dropbox.md)
 
 - Li, X., Chen, W. Y., Sanesi, G., & Lafortezza, R. (2019). Remote sensing in urban forestry: Recent applications and future directions. <i>Remote Sensing, 11</i>(10) [doi:10.3390/rs11101144](https://www.mdpi.com/2072-4292/11/10/1144)
      
 - Lin, Y., Jiang, M., Yao, Y., Zhang, L., & Lin, J. (2015). Use of UAV oblique imaging for the detection of individual trees in residential environments. <i>Urban Forestry & Urban Greening, 14</i>(2), 404–412. [doi:10.1016/j.ufug.2015.03.003](https://www.sciencedirect.com/science/article/abs/pii/S1618866715000333?via%3Dihub)
      
 - Malmsheimer, R. W., Bowyer, J. L., Fried, J. S., Gee, E., Izlar, R., Miner, R. A., Munn, I. A., Oneil, E., & Stewart, W. C. (2011). Managing forests because carbon matters: Integrating energy, products, and land management policy. <i>Journal of Forestry, 109</i>(7), S7-S50. Retrieved May 31, 2020, from [https://www.fs.usda.gov/treesearch/pubs/40291](https://www.fs.usda.gov/treesearch/pubs/40291)

- McPherson, E., & Simpson, J. (1999). Carbon dioxide reduction through urban forestry: guidelines for professional and volunteer tree planters. Albany, Calif: U.S. Dept. of Agriculture, Forest Service, Pacific Southwest Research Station. Retrieved May 31, 2020, from [https://permanent.access.gpo.gov/lps94433/psw-gtr171.pdf](https://permanent.access.gpo.gov/lps94433/psw-gtr171.pdf)

- Muller, K. (2017, May 28). here: A Simpler Way to Find Your Files. Retrieved July 6, 2020, from [https://CRAN.R-project.org/package=here](https://CRAN.R-project.org/package=here)

- National Oceanic and Atmospheric Administration (NOAA) (2020, July 1). What is lidar?. <i>National Ocean Service website.</i> Retrieved July 3, 2020, from [https://oceanservice.noaa.gov/facts/lidar.html](https://oceanservice.noaa.gov/facts/lidar.html)
   
- Pebesma, E. et al. (2020, May 20). sp: Classes and Methods for Spatial Data. Retrieved July 6, 2020 from [https://CRAN.R-project.org/package=sp](https://CRAN.R-project.org/package=sp)

- Poon, L. (2018, December 28). Every tree in the city, mapped. Retrieved May 25, 2020, from [https://www.citylab.com/environment/2018/12/urban-tree-canopy-maps-artificial-intelligence-descartes-labs/578701/](https://www.citylab.com/environment/2018/12/urban-tree-canopy-maps-artificial-intelligence-descartes-labs/578701/)

- Roussel, J. et al. (2020, July 5). lidR: Airborne LiDAR Data Manipulation and Visualization for Forestry Applications. Retrieved July 6, 2020, from [https://CRAN.R-project.org/package=lidR](https://CRAN.R-project.org/package=lidR)

- Reid, C., Clougherty, J., Shmool, J., & Kubzansky, L. (2017). Is all urban green space the same? A comparison of the health benefits of trees and grass in New York City. <i>International Journal of Environmental Research and Public Health, 14</i>(11), 1411. [doi:10.3390/ijerph14111411](https://www.mdpi.com/1660-4601/14/11/1411)

- Ren, Z., Zheng, H., He, X., Zhang, D., Yu, X., & Shen, G. (2015). Spatial estimation of urban forest structures with Landsat TM data and field measurements. <i>Urban Forestry & Urban Greening, 14</i>(2), 336–344. [doi:10.1016/j.ufug.2015.03.008](https://www.sciencedirect.com/science/article/abs/pii/S1618866715000400?via%3Dihub)

- RStudio. (n.d.). RStudio Logo. Retrieved July 4, 2020, from [https://rstudio.com/about/logos/](https://rstudio.com/about/logos/)

- Russo, A., Escobedo, F. J., Timilsina, N., & Zerbe, S. (2015). Transportation carbon dioxide emission offsets by public urban trees: A case study in Bolzano, Italy. <i>Urban Forestry & Urban Greening, 14</i>(2), 398–403. [doi:10.1016/j.ufug.2015.04.002](https://linkinghub.elsevier.com/retrieve/pii/S1618866715000424)

- Silva, C.A. et al. (2017, July 12). rLiDAR: LiDAR Data Processing and Visualization. Retrieved July 6, 2020, from [https://CRAN.R-project.org/package=rLiDAR](https://CRAN.R-project.org/package=rLiDAR)

- Silva, C. A., Klauberg, C. M., Mohan, M. M., & Bright, B. C. (2018). LiDAR Analysis in R and rLiDAR for Forestry Applications. Retrieved from [https://www.researchgate.net/publication/324437694_LiDAR_Analysis_in_R_and_rLiDAR_for_Forestry_Applications](https://www.researchgate.net/publication/324437694_LiDAR_Analysis_in_R_and_rLiDAR_for_Forestry_Applications)

- Taylor, A. F., Wiley, A., Kuo, F. E., & Sullivan, W. C. (1998). Growing up in the inner city: Green spaces as places to grow. <i>Environment and Behavior, 30</i>(1), 3–27. [https://doi.org/10.1177/0013916598301001](https://doi.org/10.1177/0013916598301001)

- The R Foundation. (2016). The R logo. Retrieved July 4, 2020, from [https://www.r-project.org/logo/](https://www.r-project.org/logo/)

- Thomson, C. (2020). How to overcome large datasets in point cloud processing. <i>Vercator</i>. Retrieved July 5, 2020, from [https://info.vercator.com/blog/how-to-overcome-large-datasets-in-point-cloud-processing](https://info.vercator.com/blog/how-to-overcome-large-datasets-in-point-cloud-processing)

- Tigges, J., & Lakes, T. (2017). High resolution remote sensing for reducing uncertainties in urban forest carbon offset life cycle assessments. <i>Carbon Balance and Management, 12</i>(1), 1–18. [https://doi.org/10.1186/s13021-017-0085-x](https://doi.org/10.1186/s13021-017-0085-x)

- Toro, M. (2017). Robust USGS LiDAR data for Metro Phoenix now available. Retrieved June 29, 2020 from [https://lib.asu.edu/geo/news/trees](https://lib.asu.edu/geo/news/trees)

- TreesCount! (2017). Retrieved May 31, 2020, from [http://media.nycgovparks.org/images/web/TreesCount/Index.html](http://media.nycgovparks.org/images/web/TreesCount/Index.html)

- Turner‐Skoff, J. B., & Cavender, N. (2019). The benefits of trees for livable and sustainable communities. <i>Plants, People, Planet, 1</i>(4), 323–335. [doi:10.1002/ppp3.39](https://nph.onlinelibrary.wiley.com/doi/full/10.1002/ppp3.39)

- U.S. Department of Agriculture, Forest Service. (2018). Urban nature for human health and well-being: A research summary for communicating the health benefits of urban trees and green space. FS-1096. Washington, DC. Retrieved May 25, 2020, from [https://permanent.access.gpo.gov/gpo91156/urbannatureforhumanhealthandwellbeing_508_01_30_18.pdf](https://permanent.access.gpo.gov/gpo91156/urbannatureforhumanhealthandwellbeing_508_01_30_18.pdf)

- USGS. (2014). NGA LiDAR project - Phoenix, AZ. Retrieved July 4, 2020, from ASU Library Map and Geospatial Hub [https://lib.asu.edu/geo](https://lib.asu.edu/geo)

- Ulmer, J. M., Wolf, K. L., Backman, D. R., Tretheway, R. L., Blain, C. J., O’Neil-Dunne, J. P., & Frank, L. D. (2016). Multiple health benefits of urban tree canopy: The mounting evidence for a green prescription. <i>Health & Place, 42</i>, 54–62. [doi:10.1016/j.healthplace.2016.08.011](https://linkinghub.elsevier.com/retrieve/pii/S1353829216301332)

- University of Chicago Computing for the Social Sciences. (2020, February 18). Drawing raster maps with ggmap. Retrieved July 7, 2020, from [https://cfss.uchicago.edu/notes/raster-maps-with-ggmap/#obtain-map-images](https://cfss.uchicago.edu/notes/raster-maps-with-ggmap/#obtain-map-images)

- Wasser, L. (2020). Create a canopy height model with LiDAR data. Retrieved June 29, 2020 from [https://www.earthdatascience.org/courses/earth-analytics/lidar-raster-data-r/lidar-chm-dem-dsm/](https://www.earthdatascience.org/courses/earth-analytics/lidar-raster-data-r/lidar-chm-dem-dsm/)

- Wickham, H. & RStudio (2019, November 21). tidyverse: Easily Install and Load the 'Tidyverse'. Retrieved July 6, 2020, from [https://CRAN.R-project.org/package=tidyverse](https://CRAN.R-project.org/package=tidyverse)

- Zhao, M., Kong, Z.-H., Escobedo, F. J., & Gao, J. (2010). Impacts of urban forests on offsetting carbon emissions from industrial energy use in Hangzhou, China. <i>Journal of Environmental Management, 91</i>(4), 807–813. [doi:10.1016/j.jenvman.2009.10.010](https://www.sciencedirect.com/science/article/pii/S030147970900365X?via%3Dihub)
  
- Zheng, D., Ducey, M., & Heath, L. (2013). Assessing net carbon sequestration on urban and community forests of northern New England, USA. <i>Urban Forestry & Urban Greening, 12</i>(1), 61–68. [https://doi.org/10.1016/j.ufug.2012.10.003](https://doi.org/10.1016/j.ufug.2012.10.003)

- Zhu, H. et al. (2019, March 16). kableExtra: Construct Complex Table with 'kable' and Pipe Syntax. Retrieved July 6, 2020, from [https://CRAN.R-project.org/package=kableExtra](https://CRAN.R-project.org/package=kableExtra)

<br>

---

<center>
  <h1 id = "Author">Author</h1>
</center>
 
 <p> Courtney Stowers is a graduate student completing an M.S. in Program Evaluation and Data Analytics at the Watts College of Public Service and Community Solutions, Arizona State University. Her undergraduate degrees in Family and Human Development and Applied Quantitative Science and work experience as a teaching assistant in college-level family science, research methods, and social statistics courses lend to a special interest in social policy for families and children. She hopes to pursue a career that will allow her to use data science to effect change in the lives of communities throughout the United States and across the globe. </p>

<p> During her free time, she enjoys exploring new coding languages, playing board and card games, baking, solving sticker puzzles, reading (particularly current events news articles and historical, romance, and children's literature), listening to music (especially from 1980s-2010s boybands!), and falling asleep on television shows. </p>

<p markdown="1"> She can be contacted via email at courtney.stowers@asu.edu. You can also visit her Github Page [here](https://github.com/castower). </p>
  
---

<p> <i> Last updated: July 07, 2020 </i> </p>
