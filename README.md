# Models

To meet our prject goal of exploring music in terms of form of therapy to see if it could help improve mental health. We tried several different models from Random Forest Classifier, Easy Ensemble, Smote, Undersampling, and SMOTEEM.
<br><br>
From all of these the best performing model was the RandomForest with a 69.89% Accuracy and a F1 Score of 70%.

![randomforest_confusion](https://github.com/mbthompson14/final_project/blob/final_supervised_machine_learning/Images/randomforest_confusionmatrix.PNG?raw=true)

From more observation we also noted that the top 5 most important factors were the BPM, Age, Anxiety, Depression, and Hours Per Day.

![randomforest_importance](https://github.com/mbthompson14/final_project/blob/final_supervised_machine_learning/Images/randomforest_importance.PNG?raw=true)

Our data we believe has too much outlier data and is too skewed. Recommandations would be to get more data and hopefully more varied in terms of age to see more consistancy across all ages and not just for 20 year olds.
