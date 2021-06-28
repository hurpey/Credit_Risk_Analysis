# Credit_Risk_Analysis

**Overview of the analysis:**

The purpose if this analysis is to determine resampling models, SMOTEENN Algorithm and Ensemble Classifiers should be used to predict credit risk. This analysis uses imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling. Also, using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, this analysis oversamples the data using the RandomOverSampler and SMOTE algorithms, and undersamples the data using the ClusterCentroids algorithm. Additionally, a combinatorial approach of over- and undersampling using the SMOTEENN algorithm is used. This analysis also compares two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. The performance of these models is evaluated, and a written recommendation is included, on whether they should be used to predict credit risk.

**Results:**

The images below show the balanced accuracy scores and the precision and recall scores of all six machine learning models

- Smote:

<img width="242" alt="Smote" src="https://user-images.githubusercontent.com/79670933/123569338-23c24d00-d794-11eb-9548-6337a48aa5e7.png">

- Smoteenn:
- 
<img width="235" alt="Smoteenn" src="https://user-images.githubusercontent.com/79670933/123569339-245ae380-d794-11eb-887b-4e91cc29318b.png">

- BalancedRandomForestClassifier:
- 
<img width="238" alt="balancedrandomforestclassifier" src="https://user-images.githubusercontent.com/79670933/123569340-245ae380-d794-11eb-9a8a-d7f78e3eda68.png">

- ClusterCentroids:

<img width="238" alt="ClusterCentroids" src="https://user-images.githubusercontent.com/79670933/123569341-245ae380-d794-11eb-8779-6cc557d0237d.png">

- EasyEnsembleClassifier:
 
<img width="236" alt="Easyensembleclassifier" src="https://user-images.githubusercontent.com/79670933/123569342-24f37a00-d794-11eb-8dfb-cc33932ef22a.png">

- RandomOverSample:

<img width="235" alt="Randomoversample" src="https://user-images.githubusercontent.com/79670933/123569343-24f37a00-d794-11eb-8091-73b2cd7fe94e.png">

Summary: Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.
