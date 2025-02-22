# phase-3-project
# Customer Churn Prediction 

## **Overview**
Customer churn is a critical issue for businesses, particularly in industries with high customer acquisition costs, such as telecommunications. This project aims to develop a machine learning model to predict customer churn using the **SyriaTel Customer Churn dataset**. By identifying at-risk customers, businesses can take proactive measures to retain them and reduce revenue loss.

## **Business and Data Understanding**
### **Business Problem**
Our key stakeholder is a **telecommunications company** seeking to minimize customer churn by leveraging machine learning. The goal is to predict which customers are likely to leave and provide insights into the factors influencing churn.

### **Dataset**
- The dataset contains various features such as **customer account details, usage patterns, call durations, and customer service interactions**.
- The target variable is **churn**, where 1 represents a churned customer, and 0 represents a retained customer.
- Key features include:
  - **Total day minutes, total night minutes, customer service calls** (indicating dissatisfaction), and **international plan** status.
  
## **Modeling**
### **Approach**
To ensure the best predictive performance, we took an **iterative approach**:
1. **Baseline Model:** Logistic Regression to establish a benchmark.
2. **Decision Tree Model:** A more flexible model to capture non-linear patterns.
3. **Hyperparameter Tuning:** Optimizing the Decision Tree using GridSearchCV.
4. **Ensemble Learning (Optional):** Testing a Random Forest model for improved accuracy.

### **Feature Engineering & Preprocessing**
- **Handled missing values**
- **Converted categorical variables** using one-hot encoding
- **Standardized numerical features** for better model performance

## **Evaluation**
The models were evaluated using:
- **Accuracy**: Measures the overall correctness of the model.
- **Precision & Recall**: Important for assessing false positives and false negatives.
- **F1-Score**: Balances precision and recall.
- **ROC-AUC Curve**: Evaluates classification performance across thresholds.
- **Confusion Matrix**: Provides insights into misclassifications.

### **Results**
- The **Logistic Regression model achieved 85% accuracy**, providing a simple and interpretable baseline.
- The **tuned Decision Tree model improved accuracy to 94%**, with better feature importance insights.
- **Feature Importance:** Customer tenure and service call frequency were strong churn predictors.

## **Conclusion**
### **Key Takeaways**
- **Customer tenure and frequent customer service calls** significantly influence churn.
- **Predictive modeling can help telecom companies proactively retain customers.**
- **Decision Trees outperform Logistic Regression** but require tuning to prevent overfitting.

### **Recommendations**
- **Proactive Retention Strategies:** Offer loyalty programs or discounts to high-risk customers.
- **Improved Customer Support:** Reduce negative interactions that lead to churn.
- **Further Model Enhancements:** Explore **ensemble methods (Random Forest, XGBoost)** to refine predictions.
- **Deploy Model in Production:** Integrate the model into business operations for real-time churn predictions.

---
### **Next Steps**
- Explore **deep learning models (Neural Networks)** for better pattern recognition.
- Incorporate **additional customer behavior data** (e.g., survey feedback).
- **Monitor Model Performance** and retrain with new data to maintain accuracy.



