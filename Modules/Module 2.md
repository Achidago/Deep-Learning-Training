### 2. Remote sensing systems and sensors
**2.1 Sensors:** 

• **Active sensors** consist of a transmitter and a receiver that may (monostatic system) or may not be (bistatic system) co-located. It transmits a known signal at a particular wavelength and receives some portion of the signal in the direction of a receiver. In case of a monostatic system, the received signal is called “backscatter”. Examples include a camera with the flash, Light Detection and Ranging (LIDAR), Synthetic aperture radar (SAR). 

• **Passive Sensors** consist of receiver that receives naturally occurring EM energy from a target at a particular wavelength and direction. Examples include a camera without the flash and radiometers.

<br/>

<!--- 
**Types of Detectors:** 

**Thermal detectors**

• absorb incident flux and undergo temperature changes

• the power in absorbed radiation is typically small, and so the detector itself should be small to have a low heat capacity

• Ex: Bolometer 

![image](https://user-images.githubusercontent.com/87503837/133616355-0ff8f5fd-2d57-4e97-b781-786353fa934e.png)

**External Photo-effect detectors**

• has photocathode where incident light is partially absorbed and generates photoelectrons

• Ex: Photomultiplier Tube (PMT)


<img src="https://user-images.githubusercontent.com/87503837/133625438-5593a350-5cd9-414a-bd1e-24f23e051fc4.png" width="500" height="320">

**Internal Photo-effect detectors**

• semiconductors in which the electons undergo internal energy level transitions when they absorb an electron

• consists of **photoconductive detectors** and **photovoltaic detectors**

• Ex: 

<img align="center" src="https://user-images.githubusercontent.com/87503837/133616643-ba9e4e28-2811-4d02-bc5a-987a549af606.png" width="350" height="320">

-->

**2.2 Resolution:**

• **Spatial resolution** describes how far apart two targets have to be so that they are detected as separate signals. If the detectable distance is small, the resolution is called **high** or **fine** and if the detectable distance is large, the resolution is **low** or **coarse**. 

• **Temporal resolution** describes how often a sensor observes the same target. If the revisit time is small, i.e. the target is observed more frequently, the temporal resolution is considered high (e.g. SMAP at about 2-3 days). On the other hand if the revisit time is longer or infrequent, e.g. LandSat at about 16 days, the temporal resolution is low/coarse. Typically, finer spatial resolution is associated with infrequent coverage because it covers less area during each overpass. 

• **Radiometric resolution** describes the number of wavelengths observed. For example, multispectral sensors observe about 10s of bands (or wavelength regions) in the VI/NIR spectrum, providing discrete observations. In contrast, hyperspectral sensors or imaging spectrometers observe 100s of wavelengths in the VI/NIR spectrum and provide continuous observations.

Spectral sampling: Multispectral sensors

<img src="https://user-images.githubusercontent.com/87503837/133636464-24493df3-1c5d-405f-b7ec-10fe64cec5e7.png" width="500" height="320">

Spectral sampling: Hyperspectral sensors

<img src="https://user-images.githubusercontent.com/87503837/133636485-93336e1a-214b-4897-b1ca-c1206879b4e1.png" width="500" height="320">


<br/>

**2.3 Satellite Systems**

•	**Geo-stationary/geo stationary/geo-synchronous** : continuous coverage of synchronous : continuous coverage of one region one region only (meteorological applications, high Earth (meteorological applications, high Earth orbit of ~36000 km; low/coarser spatial resolution; ~36000 km; low/coarser spatial resolution; e.g GOES, Japanese GOES, Japanese GMS, European GMS, European Metosat Metosat)

•	**Polar orbiting** : 100s km, low Earth orbit, high/fine spatial resolution; repeat global resolution; repeat global coverage; e.g. coverage; e.g. Landsat Landsat, Landsat Landsat TM, NOAA AVHRR, SSM/I TM, NOAA AVHRR, SSM/I) 

•	**Neither** - Tropical Rainfall Mapping Mission (TRMM), Tropical Rainfall Mapping Mission (TRMM), +/- 35deg

<br/>

**2.4 Graphics:**


**2.5 Applications of Remote Sensing**
1. Land use/land cover mapping
2. Geological and soil mapping
3. Agriculture
4. Forestry
5. Rangeland
6. Water resource
7. Snow and ice
8. Urban and regional planning 
9. Wetland mapping
10. Wildlife ecology 
11. Archeological 
12. Environmental assesment and protection
13. Natural disaster assesement 

**Data Sources**
| Data type                                     | Source      |
|-----------------------------------------------|-------------|
| Albedo                                        | MODIS       |
| Evapotranspiration   (ET)                     | MODIS       |
| Land cover                                    | LANDSAT     |
| Land surface   temperature                    | MODIS       |
| NDVI                                          | MODIS       |
| Normalized difference vegetation index (NDVI) | LANDSAT     |
| Soil   properties - moisture                  | NASA-SMAP   |
| Soil   properties                             | AfSoilGrids |
| Topography                                    | USGS        |
| Ts                                            | MODIS       |
| NDVI                                          | MODIS       |
| Ts                                            | MODIS       |
| Albedo                                        | MODIS       |

A table of the bands from the Landsat satellite program are given below, with the differences between Landsat 5, 7, and 8 outlined. General uses for these bands are supplied, such as Land Use/Land Cover (LULC) and Land Surface Temperature (LST).

<p align="center">
<img src="https://user-images.githubusercontent.com/84922404/134026792-d1f488cd-3630-4266-ad2f-ed7062e52982.png" width="500" height="600">
</p>
(M.U. Liaqat (February, 2016))