# Fake-insurance-claims

## The goal of this project is to build a model that can detect auto mobile insurance fraud. Several models are tested to produce best results.

Dataset source: https://www.kaggle.com/buntyshah/auto-insurance-claims-data

The data set consist of 1000 auto incidents and auto insurance claims from Ohio, Illinois and Indiana from 01 January 2015 to 01 March 2015. Before any cleaning or feature engineering, the data set has a total of 40 variables with 1000 samples.

The dataset is highly imbalanced with 247 frauds and 753 non-frauds claimes.24.7% of the data were frauds while 75.3% were non-fraudulent claims.

![in1](https://user-images.githubusercontent.com/62187533/121945310-42c2e700-cd71-11eb-8212-8ff5506e092c.png)

The dataset is balanced using 'SMOTE'. Synthetic Minority Oversampling Technique, or SMOTE is a technique used for balancing the imbalanced dataset by oversampling the minority class. After smote the dataset is balanced with both classes have 526 samples each

## Exploratory data analysis:

### Exploring categorical variables

![in4](https://user-images.githubusercontent.com/62187533/121946222-54f15500-cd72-11eb-9f89-1d2986cd13df.png)

### Exploring numerical variables

![in3](https://user-images.githubusercontent.com/62187533/121945962-0348ca80-cd72-11eb-8dd3-b0e1b7bec2aa.png)

#### Outliers in numerical features

![in5](https://user-images.githubusercontent.com/62187533/121946373-7ce0b880-cd72-11eb-89a9-3e0ceec41ac3.png)

IFrom the above plots it can be seen that property_claim, policy_annual_premium, and age has some outliers.

### Correlation between features

![in6](https://user-images.githubusercontent.com/62187533/121946382-7f431280-cd72-11eb-826e-3e3c0c682a78.png)

Here we can see that there is some correlation between age and months as customer apart from that there is no major correlation between features.


## Performance of different models:

### Logistic regression

Results on training data:

- Accuracy = 0.7956273764258555
- Precision = 0.7961936939383735
- Recall = 0.7956273764258555

Results on testing data:

- Accuracy = 0.7866666666666666
- Precision = 0.8178682345846525
- Recall = 0.7866666666666666

![im7](https://user-images.githubusercontent.com/62187533/121947042-39d31500-cd73-11eb-9b20-cc2c16c06bea.png)

### Random forest classifier

Results on training data:

- Accuracy = 1.0
- Precision = 1.0
- Recall = 1.0

Results on testing data:

- Accuracy = 0.8266666666666667
- Precision = 0.823645147123408
- Recall = 0.8266666666666667

![im8](https://user-images.githubusercontent.com/62187533/121947048-3b044200-cd73-11eb-9799-b19bad778761.png)

### Support vector machine(degree =2, kernel = rbf, C = 3)

Results on training data:

- Accuracy = 0.8336501901140685
- Precision = 0.8349686305957829
- Recall = 0.8336501901140685

Results on testing data:

- Accuracy = 0.7633333333333333
- Precision = 0.7890935068512016
- Recall = 0.7633333333333333

![im9](https://user-images.githubusercontent.com/62187533/121947049-3b044200-cd73-11eb-84c2-7e9511fab350.png)

### Decision tree classifier

Results on training data:

- Accuracy = 1.0
- Precision = 1.0
- Recall = 1.0

Results on testing data:

- Accuracy = 0.78
- Precision = 0.7779851159357895
- Recall = 0.78

![im10](https://user-images.githubusercontent.com/62187533/121947053-3c356f00-cd73-11eb-8cfe-972d9835cff4.png)

### XGBoost classifier

- Accuracy = 1.0
- Precision = 1.0
- Recall = 1.0

Results on testing data:

- Accuracy = 0.8266666666666667
- Precision = 0.8222902654111418
- Recall = 0.8266666666666667

![im11](https://user-images.githubusercontent.com/62187533/121947056-3d669c00-cd73-11eb-8ca5-33dcf2e4cafc.png)

### CatBoost classifier

Results on training data:

- Accuracy = 1.0
- Precision = 1.0
- Recall = 1.0

Results on testing data:

- Accuracy = 0.8433333333333334
- Precision = 0.8440751813760663
- Recall = 0.8433333333333334
- 
![im12](https://user-images.githubusercontent.com/62187533/121947059-3dff3280-cd73-11eb-92a5-7a8347a0c14e.png)

  Out of all the models 'CatBoost classifier' gives best results with 100% accuracy on training data and 84% accuracy on test data.


