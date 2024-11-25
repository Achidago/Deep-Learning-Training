# Module 1 - Artificial Neural Network 
> **Instructor**: Emmanuel Asare (<ins>emmanuelasare@<i></i>ufl.edu</ins>) <br>
> **Co-author**: Silas Achidago (<ins>s.achidago@<i></i>ufl.edu</ins>)

# Neural Networks Overview
## Artificial Neural Networks (ANN)
**What is a neural network?**: **An Artificial Neural Network (ANN)** is a computational model inspired by the way biological neural networks in the brain process information. ANNs consist of layers of interconnected nodes (neurons) that transform input data into output predictions. <br>



## Structure
  - **Input Layer**: The input layer receives the raw data (e.g., satellite images or geographical data). Each neuron in this layer corresponds to one feature or variable in the data.
  - **Hidden Layers**: These are intermediate layers between input and output. They apply transformations to the data using weights and biases. The number of hidden layers and neurons per layer defines the complexity of the model. In simple ANNs, these layers are **fully connected** (dense), meaning each neuron in a layer is connected to every neuron in the next layer.
  - **Output Layer**: This layer produces the final prediction, which could be a class label (in classification tasks) or a continuous value (in regression tasks).

<p align="center">
<img src="https://accra-training.s3.us-east-2.amazonaws.com/ann.png">
</p>

- **Neuron**: A neuron (or node) is a fundamental unit in artificial neural networks (ANNs) that processes input data and produces output.

- **Activation Functions**: Activation functions play a crucial role in deep learning by introducing non-linearity into the neural network.


- **Forward and backward propagation**: The **forward** pass produces predictions based on the current weights and biases of the network. These predictions are then compared to the actual labels using a loss function, which calculates the error. **Backpropagation** is the process of calculating gradients for each weight and bias in the network and then updating them to minimize the error.

- **Loss Functions**: <br>
    a. **Mean Squared Error (MSE)**: MSE calculates the average squared difference between predicted values (​ŷi) and actual values (yi).

    b. **Mean Absolute Error (MAE)**: MAE calculates the average absolute difference between predicted and actual values.

    c. **Binary Cross-Entropy (BCE)**: BCE measures the difference between actual and predicted probabilities in binary classification.
<p align="center">
<img src="https://accra-training.s3.us-east-2.amazonaws.com/bce-function.png">
</p>
    d. **Categorical Cross-Entropy**: This is an extension of binary cross-entropy for multi-class classification.

**Common Applications of Time Series Analysis:**
- Identifying urban expansion,
- Mapping deforestation,
- Monitoring flood or fire-related damage,
- Indentifying regions experiencing changes in temperature or precipitation.

<p align="center">
<img src="https://www.mdpi.com/urbansci/urbansci-03-00026/article_deploy/html/images/urbansci-03-00026-g006.png">
</p>
<sub> Landcover changes for Greater Accra Metropolitan Area (GAMA) from the year 1991 to 2015.</sub>

([Source](https://www.mdpi.com/2413-8851/3/1/26#))<br>


## 2. Basics of Time Series Analysis
- **Spatial/geospatial data** is information on the location, shape, and extent of objects in a geographic space represented as points, paths, areas, or surfaces. <br>
- **Temporal data** are data that represent the state of a particular object at a given point of time. Temporal data collected over several intervals create time-series data.<br>
- **Spatio-temporal data** are data that describe the state of objects or processes across both space and time. 

<p align="center">
<img src="https://user-images.githubusercontent.com/87503837/151854688-12a69e04-c870-4273-88e6-4c30e7b9d7d5.png">
</p>

([Source](https://doi.org/10.1186/s40965-017-0038-z))<br>
MODIS NDVI and EVI

**Using Remote Sensing to Conduct Time Series Analyses:**
- In the context of remote sensing, time series analyses allow us to measure and quantify changes in spatio-temporal processes from space,
- For effective monitoring to occur, data need to: 1) have suitable spatial and spectral resolution to detect the phenomena, and 2) have a frequent-enough repeat interval to detect change.
- Assuming the object is detectable using a specific sensor, the timing of acquisition needs to be tuned to the rate of the process being studied. For example, discrete event detections (such as floods or fires) can be conducted by collecting images before and after that event has occurred. Images need to be spaced close in time for assessing rapidly changing phenomena, such as vegetation greenup after rain. For monitoring long-term changes, data can be aggregated over the time domain of interest, and then assessed on annual or monthly bases (urban expansion, temperature rise). 
- The availability of satellite data over different spatio-temporal resolutions therefore limits the kinds of proceses that can be studied.
- Some trends may need to be decomposed into their underlying components for generating insights into the dynamics. For example, temperature usually has a strong seasonal component in addition to potentially annual components in some regions.

**Types of Time Series Analysis**
- **Land cover trends:**
At the simplest, the relative change in the proportion of land cover types across time. When land cover maps are available, the user can calculate the proportions of landcover, and potentially aggregate them over administrative regions to generate a picture of differing trends in urbanization, agricultural expansion, or deforestation etc. Estimates of trends of land cover change are generally important for administrative and management applications.

<p align="center">
<img src="https://www.mdpi.com/land/land-09-00300/article_deploy/html/images/land-09-00300-g003.png">
</p>
<sub> Maps showing land cover change (LCC) characteristics in Kumasi (1986–2018)a. </sub>

([Source](https://www.mdpi.com/2073-445X/9/9/300/htm#))<br>

- **Seasonal/Annual Trends:**
Whereas land cover change can be considered a 'discrete' change in the state of a pixel or parcel of land, many processes vary continuously across both time and space. Temperature is a good example. Time series of temperature measurements can be analyzed for both seasonal variation (i.e. minimum/maximum annual temperature) or when strung together across many years, as annual trends (i.e. climate change).

<p align="center">
<img src="https://media.springernature.com/full/springer-static/image/art%3A10.1007%2Fs12665-022-10481-y/MediaObjects/12665_2022_10481_Fig9_HTML.png?as=webp">
</p>
<sub> Temperature analysis over the study period (1970–2020) in Southwestern Ghana </sub>

([Source](https://link.springer.com/article/10.1007/s12665-022-10481-y/figures/9))<br>

## 3. Methods for Change Mapping and Time Series Analysis
Several approaches can followed depending on the application context, for example:
- **Linear Models** - 
Linear time series analysis techniques are predicated on the assumption that the underlying process changes at a constant rate. For example, assessing the annual rate of change in land surface temperature across a city. In general, this involves fitting a straight line through time series of the observations of interest and evaluating the magnitude and direction of the slope of the fit.
- **Nonlinear Models** - 
Nonlinear time series models are employed when the time series cannot be adequately described by a straight line. For example, indicators of vegetation greenness usually have a strong seasonal component. Fitting a straight line through the data ignores intra-annual variations that might be important.
**Harmonic models**, also termed spectral analysis or Fourier analysis, allow the decomposition of the periodic signal into a series of sinusoidal functions, each defined by unique amplitude and phase values. See [this paper](https://www.isprs.org/proceedings/xxxiii/congress/part4/384_xxxiii-part4.pdf) for an excellent example.<br>
**Breakpoint Models** - Allow the automatic detection of breaks in time series data, and potentially the fitting of different linear and nonlinear models on either side of the break. 

## 4. Time Series Analysis in GEE

GEE has the functionality to derive both linear and harmonic trends from satellite imagery and environmental data. The techniques can be mixed and matched to model both simple trends, and to decompose complex trends into seasonal and annual components, and to detect and fit breakpoint models.
For the purposes of this training, we will focus on developing estimates of simple linear trends across regions. The user is directed to documentation on [**CCDC**](https://gee-ccdc-tools.readthedocs.io/en/latest/) for a more complex treatment of harmonic time series components for land cover mapping, and to [**LandTrendr**](https://emapr.github.io/LT-GEE/) for utilizing breakpoints for detection landcover change.
We will follow the following steps:
- Identify and collect a time series of interest,
- Find a location of interest, extract a time series and plot a chart,
- Export the chart in excel, and fit a linear trend to it,
- Fit linear trends to all pixels in the area of interest to assess rates of change.
<p align="center">
<img src="https://developers.google.com/static/earth-engine/images/Charts_image_collection_05.svg">
</p>
<sub> Example chart of time series NDVI data from MODIS plotted in GEE from 2010 to 2019. </sub>

([Source](https://developers.google.com/earth-engine/guides/charts_image_collection))<br>

## 5. Excercises<br>
**5.1 Extracting and exploring time series**<br>
- In this example, we will use GEE to extract a single time series from an ImageCollection and will open it in Microsoft Excel (or software of your choice).  We will manually fit a linear trendline to this time series and extract the slope. 
- If needed, use [this script](https://github.com/ecodynlab/GALUP/wiki/Scripts#02_image_indices_environmental_data) to refresh your skills in finding, filtering, and clipping images, 
- Copy the script [Time Series Analysis Example](https://github.com/ecodynlab/GALUP/wiki/Scripts#03_time_series_analysis_example) and paste into GEE editor,
- Variables **ST_DATE** and **EN_DATE** specify the start and end dates,
- Variable **MOD13Q1** is the MODIS 16-day 500m Global NDVI/EVI product
- Variable **imgNDV** filters all MODIS Data to get NDVI images and clip them to the region of interest.
- Variable **imgPET** similarly filters all MOD16A2 Data to get PET images and clip them to the region of interest.
- The print statements let you inspect the contents of these image collecetions in the console.
- On the charts generated in the console, click on the upper right corner to open the chart in a new window.
- Download the chart as an CSV sheet by clicking on the button in the upper right corner.
- Open this CSV in Microsoft Excel and fit a trendline to it.
- Please complete [Exercise 1](https://github.com/ecodynlab/GALUP/blob/main/ExercisesM2/Exercise1.md)

**5.2 Conducting linear time series analyses across large regions**<br>
- In this example, we will fit linear trends to all pixels across a large region and will assess how trends vary geographically for different parameters.
- Copy the script [Linear Time Series Fitting](https://github.com/ecodynlab/GALUP/wiki/Scripts#04_time_series_linear_fit) and paste into GEE editor,
- Variables **ST_DATE** and **EN_DATE** specify the start and end dates,
- Function **createTimeBand** adds a 'time band' to any image. Think of this as adding the date column to your excel sheet. This will form the X-axis.
- Variables **ERA5_temp** and **ERA5_rain** collect ERA5 reanalysis climatological data, filter dates set above, clip them to the region of interest, and add the time band.
- Variable **linearFitTemp** fits the linear fitting 'reducer' to the stack of images. A 'reducer' is a function that takes information from all bands and computes a certain metric from it. Common reducers include mean, median, min, and max. The **linearFit** reducer fits a linear regression model for every stack of pixels against the time band, and outputs the scale (slope), and the offset (intercept) of the fitting line.
- Inspect the respective histograms to find the best visualization parameters for the map displayed.
- Please complete [Exercise 2](https://github.com/ecodynlab/GALUP/blob/main/ExercisesM2/Exercise2.md)

## 6. What's Next?
Module 2 - [Change Detection](module2.md)

## 7. Other Useful Resources
 1. [Cloud-Based Remote Sensing with Google Earth Engine](https://www.eefabook.org/go-to-the-book.html)<br>
 2. [NASA ARSET: Time Series Analysis](https://www.youtube.com/watch?v=RqVselZ5hKM&t=3695s)<br>
