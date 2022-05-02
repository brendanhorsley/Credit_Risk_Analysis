# Credit Risk Analysis

The purpose of this analysis was to assist Jill in handling credit risk data. 
With a large number of clients having to manually evaluate each client for their credit risk becomes a lengthy process.
With supervised machine learning, we could have a machine sort individuals into low or high risk by feeding it examples of labelled data.
We trained our machine learning model to attempt to effectively predict the credit risk of individuals applying for loans and credit cards.

## Results

The model was created and then retrained using different support packages.
The accuracy scores of the model after each training are listed below:
* Original Resampling: 0.65
* Naive Random Oversampling: 0.58
* SMOTE Oversampling: 0.65
* Undersampling: 0.65
* Combination of Over and Undersampling: 0.67
* Balanced Random Forest: 0.79
* Easy Ensemble AdaBoost: 0.93

![resampled_against_over](https://user-images.githubusercontent.com/96553988/166177589-c0574e57-a022-4ebd-acce-0812c89c57a7.png)
![balanced_random_forest](https://user-images.githubusercontent.com/96553988/166177593-605b05fc-3004-4a62-97f4-708bed8aa2bb.png)
![easy_ensemble](https://user-images.githubusercontent.com/96553988/166177596-ac91fe9f-da2f-4359-b9ff-34fdebda55c0.png)

Below is the precision of the models with the three highest accuracy scores.

Combination of Over and Undersampling:
![overunder](https://user-images.githubusercontent.com/96553988/166178543-b1318e19-ab6f-4b19-9262-ade89121a7a6.png)

Balanced Random Forest:
![forest_precision](https://user-images.githubusercontent.com/96553988/166178561-b2467d55-77b6-48b1-a7b5-244ba6cec174.png)

Easy Ensemble AdaBoost:
![easy_ensemble_precision](https://user-images.githubusercontent.com/96553988/166178573-146cccd5-832a-4a7f-80f4-1a166d0a1193.png)


## Analysis
From our analysis the Combination of Over and Undersampling created a model slightly more accurate than the original data resampling model.
The Balanced Random Forest model was 14% more accurate and the Easy Ensemble AdaBoost model was 28% more accurate.
The overall precision of every model was 99%, however inspecting the high risk precision we can see the Easy Ensemble AdaBoost was much higher than every other model.
The precision of high risk prediction was 0.01 in the first random oversampling model.
However, the precision for the Easy Ensemble AdaBoost was 0.09 for high risk, it was also the only model to have 100% precision on low risk individuals.
From the 6 models the Easy Ensemble model was significantly better than the other 5.
The model which uses the Easy Ensemble AdaBoost had 93% accuracy, and an overall 99% precision rating.

