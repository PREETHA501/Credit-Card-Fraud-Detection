# Credit Card Fraud Detection

Credit card fraud is a major problem that involves payment cards like credit cards as an illegal source of funds in transactions. Fraud is an illegal way to get goods and funds. The goal of such an illegal transaction might be to get products without paying or gain an unauthorized fund from an account. 

#### Dataset Description :

Dataset taken from Kaggle.com. The creditcard.csv file represents a data set which contains only numerical input variables which are the result of a PCA transformation. Unfortunately, due to confidentiality issues, they cannot provide the original features and more background information about the data.

### IMPLEMENTATION

#### 1)DATA PRE-PROCESSING :

A. Cleaning: The dataset may contain record which may be duplicate, incomplete or may have null values. Such records need to remove/handle by certain cleaning methods. 

B. Sampling: As number of frauds in dataset is less than overall transaction, class distribution is unbalanced in credit card transaction. Hence sampling method is used to solve this issue. 

![image](https://user-images.githubusercontent.com/72308343/146036073-dc63b864-de59-475a-b68c-90f0b411e92f.png)
![image](https://user-images.githubusercontent.com/72308343/146036149-402a4aa6-a6f0-4086-9e9d-04f532c4ec73.png)

C. Scaling : By using RobustScaler(), we can remove the outliers and then use either StandardScaler or MinMaxScaler for preprocessing the dataset. It scales features using statistics that are robust to outliers. This method removes the median and scales the data in the range between the 1st quartile and the 3rd quartile.

#### 2)DATA ANALYSIS :

The data set contains 284,807 transactions. Most transactions are non-fraudulent. In fact, 99.83% of the transactions in this data set were not fraudulent while only 0.17% were fraudulent. We are visualizing the data using graphs for better understanding on effect of sampling in dataset for prediction.

#### 3)DATA PREDICTIVE MODEL :

Building the model using Logistic Regression, SVM and Decision Tree.

#### 4)MODEL EVALUATION :

Model evaluation aims to estimate the generalization accuracy of a model on future (unseen/out-of-sample) data.
Performance of these(Logistic Regression, SVM, Decision Tree) learning algorithms used for fraud detection in credit card transactions is compared in the below table. The comparison is based on their accuracy, precision, and recall.

![image](https://user-images.githubusercontent.com/72308343/146036478-632188a7-cc92-4ecc-b5cf-aa1ef154ef23.png)
![image](https://user-images.githubusercontent.com/72308343/146036513-dcc0c1d7-640c-4708-8373-666c7c711fde.png)




