# ADMN 5016 Machine Learning Project
ADMN 5016 Project  
Business Analytics  
School of Business  
St. Lawrence College

## Field-Bounded Crop Type Classification
Crop type classification is an established application of satellite remote sensing, able to map continental scales of agriculture with a vast pool of satellite data and relatively few ground reference points required for a reasonably accurate product. Decision Trees and Support Vector Machines are commonly deployed as ML methods for the classifications.

Most 'classic' methods approach classification pixel-by-pixel. Smoothing and filtering windows may be applied *post-hoc* to map contiguous fields. While these methods are often satisfactory for large-area classifications, accuracy expectations typically top-out at 80-85%.

This project seeks to test an enhancement these methods by considering the crop field geometry prior to classification through feature engineering. Reflectance averages, vegetation indices, and aggregate measures of spread of pixel values are calculated for each field, and these values used to classify crop type for each of these discrete spatial features.

Decision-Tree and Support Vector Machine classifiers will be tested on this dataset and compared to benchmarks of pixel-by-pixel methods.

The CSV file included with this notebook contains LANDSAT 8 features extracted for each field. Three dominant crops (corn, soybeans, and winter wheat) are mapped to fields greater than 15 hectares (*n* = 928) in a small subset of West Perth County, Ontario. The satellite image is from 24 September 2013 when there is strong spectral discrimination between the crops of interest. Preprocessing and feature extraction from satellite imagery is resource-intensive and handled upstream of this CSV.

LANDSAT 8 data is retrieved from the United States Geological Survey (USGS) [EarthExplorer portal](https://earthexplorer.usgs.gov/). Field boundaries and crop data are retrieved from the author's previous work (*Bangs et al., 2014. Exploring Field-Bounded Remote Sensing and Agriculture: Spatial Discretization of Ontario Farmland. Poster. Presented to Canadian Association of Geographers Conference 2014)*. 

*N.B.:* Model Codes are adapted from ADMN 5016 course material provided by Joseph Santarcangelo
