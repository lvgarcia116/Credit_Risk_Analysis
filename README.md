# Credit_Risk_Analysis
## Overview of the analysis
The purpose of this analysis is to employe different techniques to train and evaluate models with unbalanced classes. This analysis uses imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.


## Results
The results of Naive Random Oversampling are below. The accuracy of this model is 64%, precision for the high risk group is 1%, and the sensitivity/recall is 66%.

<img width="641" alt="naive" src="https://user-images.githubusercontent.com/86024512/137638908-80fb61d1-29e7-41a0-b66d-ff9b8b80de61.png">

The results of SMOTE Oversample are below. The accuracy of this model is 65%, precision for the high risk group is 1%, and the sensitivity/recall is 69% overall.

<img width="694" alt="SMOTE" src="https://user-images.githubusercontent.com/86024512/137639065-35161606-632e-4492-9a97-46e4efb80dde.png">

The results of Undersampling are below. The accuracy of this model is 65%, precision for the high risk group is 1%, and the sensitivity/recall is 40% overall.

<img width="719" alt="Screen Shot 2021-10-17 at 1 55 29 PM" src="https://user-images.githubusercontent.com/86024512/137639150-d4a421ec-ebb1-48d7-83d4-e73654262f46.png">


The results of Combination (over and under) are below. The accuracy of this model is 54%, precision for the high risk group is 1%, and the sensitivity/recall is 57% overall.

<img width="678" alt="combination" src="https://user-images.githubusercontent.com/86024512/137639276-0f725407-3796-4033-95a8-d93635a7c331.png">

The results of Balanced Random Forest Classifier results are below. The accuracy of this model is 79%, precision for the high risk group is 4%, and the sensitivity/recall is 88% overall.

<img width="703" alt="Balanced Random" src="https://user-images.githubusercontent.com/86024512/137639378-1c22320b-b6dc-4e94-8f0d-6707d276db25.png">

The results of Easy Ensemble AdaBoost Classifier results are below. The accuracy of this model is 92%, precision for the high risk group is 9%, and the sensitivity/recall is 94% overall.

<img width="689" alt="AdaBoost" src="https://user-images.githubusercontent.com/86024512/137639467-afde8761-a46d-458d-9c3b-6b6ebed47994.png">


## Summary
This analysis used different types of sampling to determine which model is the best at predicting high risk loans. The first four models do not have a good accuracy score as the last two models 

In the first four models we undersampled, oversampled and did a combination of both to try and determine which model is best at predicting which loans are the highest risk. The next two models we resampled the data using ensemble classifiers to try and predict which which loans are high or low risk. In our first four models our accuracy score is not as high as the ensemble classifiers and the recall in the oversampling/undersampling/mixed models is low as well. Typically in your models you want a good balance of recall and precision which is why I recommend the ensemble classifiers over the first four models. It appears that the Easy Ensemble had the best balance of all the models because of it's high accuracy score and good balance of precision and recall scores.
