# END-TO-END-DATA-SCIENCE-PROJECT


*COMPANY*: CODTECH IT SOLUTIONS PVT LTD

*NAME*: Pooja Charpe

*INTERN ID*: CT12WU77

*DOMAIN*:  Data Science

*DURATION*: 12 Weeks

*MENTOR*: Neela Santosh

**This project presents a complete data science workflow, starting from data acquisition and preprocessing, moving through model development and evaluation, and culminating in deployment as a RESTful API. The objective was to predict the quality of red wine samples using their physicochemical properties, leveraging machine learning techniques and making predictions accessible via a web service.

The dataset utilized is the widely recognized "Wine Quality" dataset from the UCI Machine Learning Repository. It comprises over 1,500 red wine samples, each characterized by 11 chemical attributes such as acidity, residual sugar, pH, sulphates, and alcohol content. The target variable is the quality rating, an integer score between 0 and 10, representing expert assessments of wine quality.

The first phase of the project involved data preprocessing. The dataset was loaded into a Pandas DataFrame, and the features were separated from the target quality scores. A train-test split was performed to allocate 80% of the data for training the model and 20% for evaluating its performance on unseen data. This step ensures that the model’s generalization ability is properly assessed and guards against overfitting.

For the predictive modeling, a Random Forest Regressor was employed due to its robustness and ability to capture complex nonlinear relationships without extensive feature engineering or parameter tuning. The model was trained on the training set, and predictions were made on the test set. Performance was evaluated using Root Mean Squared Error (RMSE), which measures the average prediction error magnitude, and the coefficient of determination (R²), which indicates the proportion of variance explained by the model. The results showed reasonable accuracy, validating the model’s effectiveness for this task.

After training, the model was serialized using the joblib library. This allows the trained model to be saved as a file and loaded later for making predictions without repeating the training process, facilitating deployment and reuse.

The deployment was implemented using the Flask framework, a lightweight Python web framework suitable for quickly building APIs. A Flask application was created with two endpoints: a root route returning a simple status message to confirm the service is running, and a /predict route accepting POST requests with input features in JSON format. The API processes the input, feeds it to the preloaded model, and returns the predicted wine quality as a JSON response. This design makes the prediction model easily accessible to external clients such as web applications, mobile apps, or other backend services.

Development and experimentation took place primarily on Google Colab, an interactive cloud-based coding environment that offers free computational resources and seamless integration with Python data science libraries. Google Colab facilitated model training and evaluation efficiently. The Flask API was run locally on the developer’s machine for testing purposes, ensuring the endpoints functioned correctly and returned expected results.

This project exemplifies the full lifecycle of a data science solution—from raw data through preprocessing, model training, evaluation, and finally to deployment as a service. The combination of tools used—Python, pandas, scikit-learn, joblib, Flask, and Google Colab—highlights accessible, widely adopted technologies that make such end-to-end workflows feasible and reproducible.

The applications of this solution are broad. While specifically trained on wine quality data, the same architecture can be adapted for predictive modeling in various domains such as agriculture (crop yield predictions), healthcare (disease risk scoring), finance (credit risk evaluation), and e-commerce (demand forecasting). Deploying machine learning models as REST APIs ensures that predictive insights can be delivered in real time to diverse client applications, enabling scalable and efficient integration into business processes.**


**Where It’s Applicable**


This wine quality prediction project can be applied in many fields where predicting product quality or outcomes from data is important. Key areas include:

Food & Beverage: Predict quality of products like coffee, olive oil, and dairy to ensure consistency.

Agriculture: Forecast crop yields or soil health based on environmental data.

Healthcare: Support diagnostics by predicting patient risks or treatment outcomes.

Manufacturing: Monitor product quality during production to reduce defects.

Environmental Monitoring: Predict pollution or water quality levels for timely interventions.

Retail: Estimate demand and manage inventory of perishable goods.
