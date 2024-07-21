# Determining-Customer-Satisfaction-Predictive-Features---Using-XGB-Model-with-tunned-hyperparameters
XGBoost model

# Introduction
Using the same dataset used for the decision tree model, the data is already cleaned and prepared for the modeling. Though `XGBClassifier` is capable of handing missing values in a datset. When it encounters a missing value at a node, it tries both left and right splits and learns the path leading to a higher loss for each node. This process is repeated when working on the testing data.
However, still use the final data prepared during the Decision Tree model process. 

# Import packages

![image](https://github.com/user-attachments/assets/63608905-5d80-4868-be41-0351fd9c73e4)

For the data preparation details, [please click here](https://github.com/OTQUEEN/Constructing-and-Evaluating-a-Model-to-Predict-Customer-Satisfaction-?tab=readme-ov-file#data-exploration-data-cleaning-and-model-preparation)

![image](https://github.com/user-attachments/assets/2b2741c1-1037-4fd4-a43d-837aab795380)
![image](https://github.com/user-attachments/assets/369299c3-d2c2-4a66-8ea4-475f86c76b6c)

### Gain clarity with the confusion matrix
Creating a confusion matrix based on the predicted values for the test set.

![image](https://github.com/user-attachments/assets/939750eb-2a42-42c6-806a-a907599841dd)
* The top left to bottom right diagonal in the confusion matrix represents the correct predictions, and the ratio of these squares showcases the accuracy.

* Additionally, the concentration of true positives and true negatives stands out relative to false positives and false negatives, respectively. This ratio is why the precision score is so high (0.930).

### Visualize most important features
![image](https://github.com/user-attachments/assets/bdbd6300-abe3-4ed0-a033-3b2986164337)

* By a little margin, "seat comfort" rated as most important in the model.The type of seating is very different between first class and coach seating.
  However, the privileges of being in first class also go beyond the seating type, so perhaps that is an underlying explanation of this feature's importance.
* Surprisingly, delays (both arrival and departure) did not score as highly important.

### Comparing xgb model to the other models
[Click here for other models scores](https://github.com/OTQUEEN/Using-A-Random-Forest-Model--Evaluate-and-Determining-Predictive-Variables-In-Customer-Satisfaction?tab=readme-ov-file#comparing-the-tuned-decision-tree-model-to-the-tuned-random-forest-model-for-the-best-performing-model)
![image](https://github.com/user-attachments/assets/5d526929-afc0-497f-b052-189274dc16ac)

# Conclusion and Recommendation

**In a summary:**
* The models created is highly effective at predicting passenger satisfaction.
* Based on the results shown in the table above, the F1, precision, recall, and accuracy scores of the XGBoost model are similar to the corresponding scores of the decision tree and random forest models.
  The random forest model seemed to outperform the decision tree model as well as the XGBoost model. 

**Recommendation:**
* The feature importance of seat comfort warrants additional investigation. It will be important to ask domain experts why they believe this feature scores so highly in this model.


**Thank you for reading !!!**

To read more on Random Forest model, [please click here](https://github.com/OTQUEEN/Using-A-Random-Forest-Model--Evaluate-and-Determining-Predictive-Variables-In-Customer-Satisfaction)

To read more on Decision Tree model, [please click here](https://github.com/OTQUEEN/Constructing-and-Evaluating-a-Model-to-Predict-Customer-Satisfaction-)








