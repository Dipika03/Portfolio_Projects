# Credit Card Fraud Detection

### Description
The world we are living in, is undeniably digital. Since covid 19 there is a tremendous increase in the number of users who prefer online shopping as it is convenient and easy. Most of the people use credit cards for online purchase. Credit Card offers lot of the benefits to users and one of the advantages of credit card is - it allows users to buy something even if they do not have money at that time. This feature has also increased the financial fraud. Although cybersecurity is there and plays an important role in providing digital security, but it is not easy to track down the unusual activity.

### Tools/Technologies Used
Pyplot, series, dataframe, gridspec, download_plotlyjs, init_notebook_mode, plot, iplot, train_test_split, confusion_matrix, ConfusionMatrixDisplay, LogisticRegression, TfidfVectorizer, ROCAUC, LinearRegression, RandomForestClassifier

### Methodology
Logistic Regression Model: Using Logistic Regression Model, we can predict whether the transaction is fraud or
not.
Random Forest Model: One of the popular algorithms in machine learning is Random Forest. It is a collection of decision tree called “forest” which trained by combining different improved models. Random Forest classifier give more precise and reliable result as it is created using several decision trees.

### Exploratory Analysis:
- The dataset has 284807 rows and 31 columns.
- Using the describe function I have noticed that there is no missing values or Null values in the dataset.
- Using the heatmap below we can clearly say that v7 and v20 features are positively correlated to Amount. Class and Amount is negatively correlated to v3. Also, we can see that V2 and V5 are negatively correlated to Amount. The features V1, V2, ... and V28 are weakly correlated to each other. Class is negatively correlated to v14, v17 and v12. The features V1, V2, ... and V28 are weakly correlated to each other, and they do not have much dependency on others. But we do find that Class and Amount variable are positively and negatively correlated to some of the features like V2, V3, V5, V7, V14, V17 and V12.

### Results:
- The Logistic Regression model 98% accuracy and Random Forest classifier model shows 99.9% accuracy.
- Both models performed really well but the F1 score of Logistic regression model is very less as .12 whereas for Random Forest model the F1 score is .86.
- The trained Random Forest model performed much better on the test data set compared to Logistic Regression model.
- Random Forest model shows 96% of the Area Under the ROC curve value with 99.9% accuracy and .86 F1 score meaning the model build above can correctly classify Non-Fraudulent and Fraudulent Transactions.
