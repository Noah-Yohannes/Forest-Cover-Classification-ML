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

## Performance Evaluation

The following evaluation metrics were used to evaluate the models' performance:
* Accuracy
* Precision = High cost of false positives in this domain
* Mathew's Correlation Coefficient = Handles class imbalance.


## Model's Selection  

75% of the dataset was split into training and the rest for validation.

The following models are used in this project:  KNN (a baseline model), Naive-Bayes, Decision trees, Logistic Regression and MLP. 

## Resulsts
                   Models 
Evaluation Metrics 

|  Metrics      | KNN (5 N)     | Naive Bayees  | Decision T    | Logistic Regression  | MLP
| ------------- | ------------- | ------------- | ------------- | ------------- |-------------  
| Content Cell  | Content Cell  | Content Cell  | Content Cell  | Content Cell  | Content Cell  
| Content Cell  | Content Cell  | Content Cell  | Content Cell  | Content Cell  | Content Cell  







