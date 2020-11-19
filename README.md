# 3D House project 
### Deadline 20/11/2020


## Personal Work method

### Step 1

  Study the request ( What & Why)
   - What are shapefiles & how to read and use them ?
   - What are geoTIFFs & how to read and use them ?
   - What is LIDAR and what is the link with the assesment ?
   - What is DSM and DTM + differences

	Action points: Learing about the topic and watching tutorials

### Step 2 
 Analysing and plotting all the relevant data ( DSM 5, 12 & 13 and the mapshifs)

In  the analysis of the map shifts, the coordinates of Bruges show that this city is located in the
 dsm file 13. For the course of the assignment I will continue to work with the data series 13 to further locate the points of Bruges center.


 ### Next step

 Reading the geotiff of DSM 13 
 Proccessing the Data of DSM 13 and try to zoom more in on the city of Bruges

## after all the technical issues with the packages 
 resuming my work on the project
### 1st step
Issues with plotting the geotiff file ( 13) due to the size. the kernel kept on running for very long, 10 - 20 minutes and got nothing as output. Also my computer screen became black for a 10_15 seconds and mad a kind of beep sound 3 times.I have tried solution with rasterio “ widowed reading and writing”
But still trying to figure out how use this methode as it didn't run wel , I went looking for other soulutions to save time and have managed to reduces the size by cropping the tiff file in the Qgis tool the size went from 9, 43 MB to 11, 4 KB but still issues with plotting the image. So I think that the content of the file may have changed in the wrong way so I went back to the widowed option of rasterio and will try to figure out how to make this work.

### 2th step 

Trying to select an area around a selected coordinate point, slice that into a new geodataframe and plot that new gdf.

### 3th step 
Overlaying a shapefile on the geotiff to narrow down the location ( bruges)

### 4th step
Trying to reproject my geotiff dataset from the current coordinate reference system to the EPSG 4326. The method to use is Reprojecting and Raserio has utilities to make this easier ( transform_bounds(),calculate_default_transfor())
 