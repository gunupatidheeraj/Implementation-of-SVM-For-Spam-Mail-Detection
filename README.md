# Implementation-of-SVM-For-Spam-Mail-Detection

## AIM:
To write a program to implement the SVM For Spam Mail Detection.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import the required packages.
2. Import the dataset to operate on.
3. Split the dataset.
4. Predict the required output.
5. End the program. 

## Program:
```
/*
Program to implement the SVM For Spam Mail Detection..
Developed by: DEEPIKA.J
RegisterNumber:  212221230016

import pandas as pd
data=pd.read_csv("spam.csv",encoding='Windows-1252')

import chardet
file='spam.csv'
with open(file, 'rb') as rawdata:
    result = chardet.detect(rawdata.read(10000))
result

data.head()

data.info()

data.isnull().sum()

x=data["v1"].values

y=data["v2"].values

from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=0)

from sklearn.feature_extraction.text import CountVectorizer 
cv=CountVectorizer()

x_train=cv.fit_transform(x_train)
x_test=cv.transform(x_test)

from sklearn.svm import SVC
svc=SVC()
svc.fit(x_train,y_train)

y_pred=svc.predict(x_test)
y_pred

from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy
*/
```

## Output:

![p1](https://user-images.githubusercontent.com/94747031/203760640-cfad6efe-a694-45e4-acf6-35c2167dca43.png)

![p2](https://user-images.githubusercontent.com/94747031/203760987-ff9ea748-fd5c-41ca-98f0-4adfd963741c.png)


![p3](https://user-images.githubusercontent.com/94747031/203760751-0dfbe925-f505-480c-9bd1-9a4e1d0002b4.png)

![p4](https://user-images.githubusercontent.com/94747031/203760863-320a89cc-9e39-4249-82ad-875bd4bef18a.png)

![p5](https://user-images.githubusercontent.com/94747031/203760907-46b349c1-bedd-474f-a26d-b1d8956f8cb6.png)

![p6](https://user-images.githubusercontent.com/94747031/203760949-aee3c034-68cf-4be8-9978-636c3ea3d335.png)


## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.
