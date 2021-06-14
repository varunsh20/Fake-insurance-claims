# Fake-insurance-claims

## The goal of this project is to build a model that can detect auto mobile insurance fraud.

Dataset source: https://www.kaggle.com/buntyshah/auto-insurance-claims-data

The data set consist of 1000 auto incidents and auto insurance claims from Ohio, Illinois and Indiana from 01 January 2015 to 01 March 2015. Before any cleaning or feature engineering, the data set has a total of 40 variables with 1000 samples.

The dataset is highly imbalanced with 247 frauds and 753 non-frauds claimes.24.7% of the data were frauds while 75.3% were non-fraudulent claims.

![in1](https://user-images.githubusercontent.com/62187533/121945310-42c2e700-cd71-11eb-8212-8ff5506e092c.png)

The dataset is balanced using 'SMOTE'. Synthetic Minority Oversampling Technique, or SMOTE is a technique used for balancing the imbalanced dataset by oversampling the minority class. After smote the dataset is balanced with both classes have 526 samples each

![in2](https://user-images.githubusercontent.com/62187533/121945958-02b03400-cd72-11eb-8ab0-2072065b1d5c.png)

![in3](https://user-images.githubusercontent.com/62187533/121945962-0348ca80-cd72-11eb-8dd3-b0e1b7bec2aa.png)
