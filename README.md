# ADMN 5016 Machine Learning Project
ADMN 5016 Project  
Business Analytics  
School of Business  
St. Lawrence College

## Field-Bounded Crop Type Classification
Crop type classification is an established application of satellite remote sensing, able to map continental scales of agriculture with a vast pool of satellite data and relatively few ground reference points required for a reasonably accurate product. Decision Trees and Support Vector Machines are commonly deployed as ML methods for the classifications.

Most 'classic' methods approach classification pixel-by-pixel. Smoothing and filtering windows may be applied *post-hoc* to map more homogeneous fields. While these methods are often satisfactory for large-area classifications, accuracy expectations typically top-out at 80-85%.

This project seeks to test an enhancement these methods by considering the crop field geometry prior to classification through feature engineering. Reflectance averages, vegetation indices, and aggregate measures of spread of pixel values are calculated for each field, and these values used to classify crop type for each of these discrete spatial features.

The CSV file included with this notebook contains extracted LANDSAT 8 features for each field. Preprocessing and feature extraction from satellite imagery is resource-intensive and handled upstream of this CSV.
