# Credit_Risk_Analysis

**Overview of the analysis:**

The purpose if this analysis is to determine whether resampling models, SMOTEENN Algorithm and Ensemble Classifiers should be used to predict credit risk. This analysis uses imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling. Also, using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, this analysis oversamples the data using the RandomOverSampler and SMOTE algorithms, and undersamples the data using the ClusterCentroids algorithm. Additionally, a combinatorial approach of over- and undersampling using the SMOTEENN algorithm is used. This analysis also compares two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. The performance of these models is evaluated, and a written recommendation is included, on whether they should be used to predict credit risk.

**Results:**

Below are the balanced accuracy scores and the precision and recall scores of all six machine learning models

_- Smote Model:_

From the analysis performed using the Smote model (and shown in the image below), we observe a balanced accuracy score of approximately 66%. Also, the high risk precision is at 1% with 63% sensitivity which makes a F1 of 2% only. Lastly, as a result of the majority low risk population, we can observe a precision of about 100% with a sensitivity of 66%.

<img width="300" alt="Smote" src="https://user-images.githubusercontent.com/79670933/123569338-23c24d00-d794-11eb-9548-6337a48aa5e7.png">

_- Smoteenn Model:_

Based on the Smoteenn model analysis, we can observe a balanced accuracy score of approximately 65%. Also, high risk precision is at 1% with 69% sensitivity which makes a F1 of 2%. We can also observe a low risk sensitivity of 60%, which is attributable to the large number of  false positives. Below is a snapshot of the result using this model.
 
<img width="300" alt="Smoteenn" src="https://user-images.githubusercontent.com/79670933/123569339-245ae380-d794-11eb-887b-4e91cc29318b.png">

_- BalancedRandomForestClassifier Model:_

Based on the BalanceRandomForestClassifier analysis, we can observe a balanced accuracy score of approximately 94%. Also, high risk precision is at 4% with 64% sensitivity which makes a F1 of 7%. We can also observe a low risk sensitivity of 90% with 100% precision. Below is a snapshot of the result.

<img width="300" alt="balancedrandomforestclassifier" src="https://user-images.githubusercontent.com/79670933/123569340-245ae380-d794-11eb-9a8a-d7f78e3eda68.png">

_- ClusterCentroids Model:_

The result of the ClusterCentroids analysis shows a balanced accuracy score of approximately 51.5%. Also, high risk precision is at 1% with 61% sensitivity which makes a F1 of 1%. We can also observe a low risk sensitivity of 42% with 100% precision. Below is a snapshot of the result.

<img width="300" alt="ClusterCentroids" src="https://user-images.githubusercontent.com/79670933/123569341-245ae380-d794-11eb-8779-6cc557d0237d.png">

_- EasyEnsembleClassifier Model:_

The result of the EasyEnsembleClassifier analysis shows a balanced accuracy score of approximately 94%. Also, high risk precision is at 9% with 92% sensitivity which makes a F1 of 16%. We can also observe a low risk sensitivity of 94% with 100% precision. Below is a snapshot of the result.

<img width="300" alt="Easyensembleclassifier" src="https://user-images.githubusercontent.com/79670933/123569342-24f37a00-d794-11eb-8dfb-cc33932ef22a.png">

_- RandomOverSample Model:_

The result of the RandomOverSample model analysis shows a balanced accuracy score of approximately 66%. Also, high risk precision is at 1% with 63% sensitivity which makes a F1 of only 2%. We can also observe a low risk sensitivity of 66% with 100% precision. Below is a snapshot of the result.

<img width="300" alt="Randomoversample" src="https://user-images.githubusercontent.com/79670933/123569343-24f37a00-d794-11eb-8091-73b2cd7fe94e.png">


**Summary:**

The 6 models used for the credit risk prediction analysis show a low or weak precision in determining if a credit risk is high. 

However, the EasyEnsembleClassifier model appears to be most effective in showing the sensitivity for the high risk credits as it shows a recall of 92%. The precision rate for this model is however low at 9%, which means many low risk credits are still falsely detected. This could impact the credibility of the information provided by LendingClub. In the absence of better or reliable models, I would recommend using the EasyEnsembleClassifier model.
