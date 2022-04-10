---
title: "Dealing with Imbalance Data in Classification Problem"
categories:
    - Blog
tags:
    - Data Science
---

---
**1. Choose Proper Evaluation Metrics**
   - F1 score
  
  ![image](https://latex.codecogs.com/gif.latex?%5Cdpi%7B150%7D%20%5Cbg_white%20%5Clarge%20F_%7B1%7D%20%3D%202%5B%5Cfrac%7B%28precision%29%28recall%29%7D%7B%28precision%29&plus;recall%7D%5D)
  
**2. Resampling (Oversampling or Undersampling)**
   - sklearn.utils.resample
  
```python
from sklearn.utils import resample
#create two different dataframe of majority and minority class 
df_majority = df_train[(df_train['Is_Lead']==0)] 
df_minority = df_train[(df_train['Is_Lead']==1)] 
# upsample minority class
df_minority_upsampled = resample(df_minority, 
                                 replace=True,    # sample with replacement
                                 n_samples= 131177, # to match majority class
                                 random_state=42)  # reproducible results
# Combine majority class with upsampled minority class
df_upsampled = pd.concat([df_minority_upsampled, df_majority])
```

**3. Synthetic Minority Oversampling Technique (SMOTE)**
    - SMOTE perform k-nearest neighbour on minority class instances to obtain random synthetic instances
    - Better than oversampling using same data/entries
```python
from imblearn.over_sampling import SMOTE
# Resampling the minority class. The strategy can be changed as required.
sm = SMOTE(sampling_strategy='minority', random_state=42)
# Fit the model to generate the data.
oversampled_X, oversampled_Y = sm.fit_sample(df_train.drop('Is_Lead', axis=1), df_train['Is_Lead'])
oversampled = pd.concat([pd.DataFrame(oversampled_Y), pd.DataFrame(oversampled_X)], axis=1)
```

**4. Balanced Bagging Classifier**
    - takes 2 parameters (i.e.: **sampling_strategy** & **replacement**)
    - *sampling_strategy:* decides on the resampling required (e.g. ‘majority’ – resample only the majority class, ‘all’ – resample all classes, etc)
    - *replacement* decides whether it is going to be a sample with replacement or not.

```python
from imblearn.ensemble import BalancedBaggingClassifier
from sklearn.tree import DecisionTreeClassifier
#Create an instance
classifier = BalancedBaggingClassifier(base_estimator=DecisionTreeClassifier(),
                                sampling_strategy='not majority',
                                replacement=False,
                                random_state=42)
classifier.fit(X_train, y_train)
preds = classifier.predict(X_test)
```

**5. Threshold Moving**
    - changing the threshold for separating 2 classes using **ROC curves** and **Precision-Recall Curves**
```python
# searching optimal value in a grid
from sklearn.ensemble import RandomForestClassifier
rf_model = RandomForestClassifier()
rf_model.fit(X_train,y_train)   
rf_model.predict_proba(X_test) #probability of the class label

# check the optimal value from the predicted class label probability
step_factor = 0.05 
threshold_value = 0.2 
roc_score=0
predicted_proba = rf_model.predict_proba(X_test) #probability of prediction
while threshold_value <=0.8: #continue to check best threshold upto probability 0.8
    temp_thresh = threshold_value
    predicted = (predicted_proba [:,1] >= temp_thresh).astype('int') #change the class boundary for prediction
    print('Threshold',temp_thresh,'--',roc_auc_score(y_test, predicted))
    if roc_score<roc_auc_score(y_test, predicted): #store the threshold for best classification
        roc_score = roc_auc_score(y_test, predicted)
        thrsh_score = threshold_value
    threshold_value = threshold_value + step_factor
print('---Optimum Threshold ---',thrsh_score,'--ROC--',roc_score)
```


---
References
1. [5 Techniques to Handle Imbalanced Data For a Classification Problem](https://www.analyticsvidhya.com/blog/2021/06/5-techniques-to-handle-imbalanced-data-for-a-classification-problem/)
2. [BalancedBaggingClassifier](https://imbalanced-learn.org/stable/references/generated/imblearn.ensemble.BalancedBaggingClassifier.html)
