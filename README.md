# Implementation-of-SVM-For-Spam-Mail-Detection

## AIM:
To write a program to implement the SVM For Spam Mail Detection.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import the necessary libraries.
2. Read the dataset and separate the independent and dependent variables.
3. Split the dataset into training and testing.
4. Do preprocessing if needed, in this case vectorization is needed which is done using CountVectorizer()
5. Train the model using SVC() algorithm and .fit()
6. Predict the model on x_test.
7. Measure its accuracy

## Program:
```
/*
Program to implement the SVM For Spam Mail Detection..
Developed by    : Shivaram M.
Register Number : 212223040195
    import pandas as pd
    data=pd.read_csv("/content/spam.csv",encoding="mac_roman")
    data.info()
    
    x=data['v2'].values
    y=data['v1'].values
    x.shape
    y.shape
    
    from sklearn.model_selection import train_test_split
    x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=2)
    
    from sklearn.feature_extraction.text import CountVectorizer
    cv=CountVectorizer()
    x_train=cv.fit_transform(x_train)
    x_test=cv.transform(x_test)
    x_train
    
    from sklearn.svm import SVC
    svc=SVC()
    svc.fit(x_train,y_train)
    y_pred=svc.predict(x_test)
    y_pred
    
    from sklearn.metrics import accuracy_score
    acc=accuracy_score(y_test,y_pred)
    acc
*/
```

## Output:

<img width="1680" alt="Screenshot 2025-05-22 at 8 02 01 PM" src="https://github.com/user-attachments/assets/8c3fc44c-5f4d-4b9b-994c-439d65be0d3d" />
<img width="1680" alt="Screenshot 2025-05-22 at 8 02 07 PM" src="https://github.com/user-attachments/assets/7134f427-ead2-4bc5-96cf-e9d360534594" />

## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.
