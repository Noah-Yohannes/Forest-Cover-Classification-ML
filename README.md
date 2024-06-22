# Forest Cover Type Classification

This project aims to predict the appropriate forest cover type of an area from cartographic variables (no remotely sensed data). The variables define several features of an environment and are based on historical data the best-suited forest to grow in the area is forecasted. 

The dataset was obtained from the [UC Irvine Machine Learning Repository ](https://archive.ics.uci.edu/dataset/31/covertype), presented in the Dataset folder in this repo. It contains: 
* Cartographic variables collected from _Roosevelt National Forest of northern Colorado._
*  581,000 samples of data, 54 feature columns and encoded target columns.
*  The target column has 7 labels, forest cover types, encoded in numbers.
*  Dataset contains no missing values.


![image](https://github.com/Noah-Yohannes/Covertype_Forest-Classification/assets/112534387/fcf064d7-0d23-42f4-8945-b536173d2ec2)


## Preprocessing and Exploratory Data Analysis

* First, quantitative numerical columns are identified and operated. Then the Z-score Normalization is applied and the IQR measures are used to detect outliers.
* The features of the dataset are inspected for correlation to drop either of the highly correlated columns.
* The PCA transformation was applied to the dependent(y) and independent (x) variables, and the contribution of each component to the overall variation was observed in the figure below.
  ![image](https://github.com/Noah-Yohannes/Covertype_Forest-Classification/assets/112534387/6c9168e4-a7b0-4120-b2f2-6400ec274d79)

As can be seen, only the top 39 components were able to capture 99.5% of the variation in the dataset. Therefore, the resulting reduced dataset was used to train the models and evaluate their performance. 
  
*  The dimensionality of the dataset was reduced to account for only 95% of the variation in the original dataset. 

Features correlation

PCA analysis

All columns checked for linearity (feature->target)
![image](https://github.com/Noah-Yohannes/Covertype_Forest-Classification/assets/112534387/fd3a04f9-f6fc-48bf-bdae-a7b4f025dec2)





Predicting forest cover type from cartographic variables only (no remotely sensed data).  The actual forest cover type for a given observation (30 x 30 meter cell) was determined from US Forest Service (USFS) Region 2 Resource Information System (RIS) data.  Independent variables were derived from data originally obtained from US Geological Survey (USGS) and USFS data.  Data is in raw form (not scaled) and contains binary (0 or 1) columns of data for qualitative independent variables (wilderness areas and soil types).

Classification of pixels into 7 forest cover types based on attributes such as elevation, 
aspect, slope, hillshade, soil-type, and more.
Task Type: Classification
Dataset/Details Link: Covertype


## Outline

* The problem statement and uses
- Approaches followed
- ML modelling
- Performance Evaluation




