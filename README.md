# Credit Card Fraud Detection

![screenshot1](https://raw.githubusercontent.com/Rushikesh2209/Credit-Card-Fraud-Detection/main/Credit-card-fraud.webp)
  

## Context :
   Credit card companies must be able to recognize fraudulent credit card transactions so that customers are not charged for items that they did not purchase.
              
## Description:
  In this analysis, we focused on detecting fraudulent transactions in a credit card dataset. The dataset contains 284,807 transactions with 31 features, including time, transaction amount, and variables V1 to V28. The target variable is 'Class,' where 0 indicates a non-fraudulent transaction and 1 indicates a fraudulent transaction.

   The first step is to Import the required Libraries.

![screenshot1](https://github.com/Rushikesh2209/Credit-Card-Fraud-Detection/blob/main/Importing%20the%20required%20Libraries..png)

Upload the CSV file named (credir.csv) in the Python folder saved on Jupyter Notebook. Load the Dataset from the CSV file name (credit.csv) using the pandas function.


![screenshot1](https://github.com/Rushikesh2209/Credit-Card-Fraud-Detection/blob/main/Load%20the%20dataset.png)


Now, we loaded the dataset and examined its basic information using info(). The dataset has no missing values, and all features are numerical. 


![screenshot1](https://github.com/Rushikesh2209/Credit-Card-Fraud-Detection/blob/main/basic%20information.png)


Descriptive statistics revealed that the mean of the 'Class' variable is close to 0, indicating a class imbalance.

![screenshot1](https://github.com/Rushikesh2209/Credit-Card-Fraud-Detection/blob/main/%23Calculate%20summary%20statistics.png)


  Now, we created histograms to visualize the distribution of transaction time and amount. The histograms revealed that transaction time has a relatively uniform distribution, while transaction amounts are right-skewed, with a few extremely high transactions.

![screenshot1](https://github.com/Rushikesh2209/Credit-Card-Fraud-Detection/blob/main/subplots.png)
![screenshot1](https://github.com/Rushikesh2209/Credit-Card-Fraud-Detection/blob/main/Histo.png)


Next, we used a bar plot to show the class distribution, highlighting the significant class imbalance. There are 284,315 non-fraudulent transactions ‘Class 0’ and only 492 fraudulent transactions ‘Class 1’.


![screenshot1](https://github.com/Rushikesh2209/Credit-Card-Fraud-Detection/blob/main/Bar%20plot%20for%20'Class.png)


  Created a pie chart to visualize the percentage distribution of normal and fraudulent transactions.


![screenshot1](https://github.com/Rushikesh2209/Credit-Card-Fraud-Detection/blob/main/class%20distribution.png)

   We created box plots to compare the distribution of transaction amounts and times between non-fraudulent and fraudulent transactions. The log scale is applied to the amount axis due to the wide range of transaction amounts. 

The plots suggest that fraudulent transactions tend to have higher amounts and occur more evenly across different times.
    

![screenshot1](https://github.com/Rushikesh2209/Credit-Card-Fraud-Detection/blob/main/Screenshot%202023-12-23%20090328.png)


We calculated the correlation matrix and visualized it using a heatmap.
Most features show low correlation, indicating that the variables (V1 to V28) are relatively independent of each other.



 ![screenshot1](https://github.com/Rushikesh2209/Credit-Card-Fraud-Detection/blob/main/correlations.png)

# Conclusion
"The analysis demonstrates an effective method for detecting credit card fraud, and our findings indicate that the dataset is highly imbalanced, with fraudulent transactions amounting to a higher value than non-fraudulent transactions."

# Future Work
- Investigate advanced anomaly detection techniques.
- Implement real-time fraud detection systems.
- Explore the impact of additional features on model performance.
