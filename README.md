# -Predicting-UHIs-with-ML
# Project Overview
Remote Sensing Correlations Between Income and Land Cover to Analyze Urban Heat Islands in Austin, Texas is a research project intended to answer the following questions:  
1. What are the primary factors contributing to increased risk of urban heat islands (UHIs) in socioeconomically disadvantaged areas of Austin, Texas?
2. To what extent do these primary variables correlate with each other?  
3. Which areas in Austin are most likely to be affected by urban heat islands based on these correlations?
  
Our team investigated four variables that affect the formation of urban heat islands: percentage of vegetation (greenness), percentage of impervious surfaces (concrete and asphalt), median household income, and land surface temperature. These variables were analyzed across 444 coordinates scattered around the city of Austin, Texas. After gathering data on these four factors, our team analyzed the extent at which they correlated with each other using unsupervised machine learning algorithms and aims to use these correlation results to inspire future enviornmental justice initiatives.  

View our full research paper here: (insert relative link later)  
View our final presentation here: https://drive.google.com/file/d/1bxMNVqxsKrOWAQOOjjTbuoS7zNeVFGpI/view?usp=drivesdk  
  
# Description of Files  
  
There are eight dataset files in the repository.  
1. [Census_Incomes.csv](datasets/Census_Incomes.csv)  - a .csv file of all of the median income data extracted from the United States Census Bureau encompassing all of our coordinates of study. These data were collected over a 5-year period from 2011-2015.
2. [Austin_CoordsOnly_CSV.csv](datasets/Austin_CoordsOnly_CSV.csv) - a .csv file of all of our coordinates of study. Note that there are 518 coordinates listed in this file, but there were only 444 used in the final version of our research due to a portion of the points containing unreliable data.
3. [Austin_TX_ALLAOIDATA.csv](datasets/Austin_TX_ALLAOIDATA.csv) - a .csv file containing the same 518 coordinates of study combined with all collection data from the GLOBE Observer app. Note that there are 518 coordinates listed in this file, but there were only 444 used in the final version of our research due to a portion of the points containing unreliable data.  
4. [Final-AOI_Points_with_Average_Income.csv](datasets/Final-AOI_Points_with_Average_Income.csv) - a .csv file containing the same 518 coordinates of study combined with all collection data from the GLOBE Observer app AND their corresponding average median incomes. Note that there are 518 coordinates listed in this file, but there were only 444 used in the final version of our research due to a portion of the points containing unreliable data.
5. [FINALUHIDATA.csv](datasets/FINALUHIDATA.csv) - a .csv file containing the FINAL 444 coordinates of study combined with all collection data from the GLOBE Observer app AND their corresponding average median incomes. This data has been filtered from the previous AOI datasets to only include high quality data points. IMPORTANT: This is the data file that our Google Colab notebooks draw upon in order to run!  
6. [Austin_LST_Data_ECOSTRESS_UNFILTERED.json](datasets/Austin_LST_Data_ECOSTRESS_UNFILTERED.json) - a .json file of the original land surface temperature request from the NASA AppEEARS application. It is derived from the ECOSTRESS instrument aboard the International Space Station and encompasses daily land surface temperature measurements in Kelvin from January 1, 2022 to July 18, 2024.  
7. [Austin_LST_Data_ECOSTRESS_FILTERED.csv](datasets/Austin_LST_Data_ECOSTRESS_FILTERED.csv) - a .csv file of the original land surface temperature request from NASA AppEEARS filtered to only the high-quality data points using the original request's included quality checking fields.  
8. [datasets/Austin-LST-Points-ECO-L2T-LSTE-002-metadata.xml](datasets/Austin-LST-Points-ECO-L2T-LSTE-002-metadata.xml) - a document that contains all necessary metadata for the ECOSTRESS land surface temperature request from NASA AppEEARS.  
   
There are also two Jupyter Colab notebooks in the repository that contain all of our created code.  
1. (add in relative link to main colab later) - a notebook containing all of the code used to run correlation analysis using three different unsupervised learning algorithms: K-means, Hierarchal, and DBSCAN. This notebook also contains the graphs we generated from this correlation analysis and our steps for processing and pre-processing of the datasets. 
2. (add in relative link to results colab later) - a notebook containing our final heatmap created for the correlations between the four variables as well as the code used to generate it.  
  
# Steps to Reproduce Results

  add in code block here!  
# Citations and Acknowledgements  
Global Learning and Observations to Benefit the Environment (GLOBE) Program, 2024-07-29, https://www.globe.gov/globe-data.  
Collect Earth Online - Satellite Image Viewing & Interpretation System​. (2023, August 30). https://www.collect.earth/.  
AρρEEARS. (n.d.). Appeears.earthdatacloud.nasa.gov. https://appeears.earthdatacloud.nasa.gov/.  
United States Census Bureau. (2022). Explore Census Data. United States Census Bureau. https://data.census.gov/.  
  
These data were optained from NASA, the United States Census Bureau, and the GLOBE Program and are freely available for use in research, publications and commercial applications.  
