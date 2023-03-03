<img src="https://simplemap.io/wp-content/uploads/2022/08/Color-logo-no-background-1-2048x522.png" alt="SimpleMap Logo" width="236" height="60">

### UAV Thermography Procedures

# GEOREGISTRATION OF THERMAL IMAGES

## 1. Convert .RJPG thermal images to .TIFF
### 1.1 Use Case of UAV Matrice 300 RTK + Camera DJI H20T
In this step, we will convert our RJPG thermal images using a dockerized version of the Official DJI Thermal SDK, which can be found in this [Github repository](https://github.com/RentadroneCL/DJI-Thermal-SDK-Docker-image-Output-TIFF-Version).

Steps:
1. Fork and clone the github repository
2. Follow the instructions provided in the repository to install, build, and use the tool.

* Input: dataset of RJPG thermal images taken with DJI Martrice 300 RTK & DJI H20T camera (Format .JPG)
* Output: dataset of TIFF thermal images (Format:.TIF, EP)

### 1.2 Use Case for FLIR Cameras
*(In progress, waiting for data samples contributions)*


### 2 Georegistration of TIFF thermal images
In this step, we will use the Georeferencer tool in QGIS to convert each .tiff file into a GeoTIFF. Note that at least four (4) GCPs (Ground Control Points) are required per image for the conversion to take place. These GCPs can correspond to the corners of the images.

Steps:
1. Open Georeferencer tool in QGIS
2. Add .tiff images as raster data and GPC data as input and follow the workflow of the tool (*detailed information in next commits*).

* Input: dataset of TIFF thermal images (Format:.tif)
* Output: dataset of GeoTIFF thermal images (Format:.tif)







|*Content Maintainer*|
|-|
|*Hector Jose Bastidas Gonzalez*<br>*hector.bastidas@simplemap.io*|