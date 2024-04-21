## Swire_CocaCola_Capstone

Swire Coca-Cola is a prominent beverage distribution company operating globally, specializing in delivering a wide range of refreshing beverages to consumers. With a focus on accessibility and inclusivity, Swire Coca-Cola aims to provide beverages to diverse communities, including those in remote or underserved areas. Renowned for its innovative distribution strategies, Swire Coca-Cola leverages advanced logistical systems and market insights to ensure timely and efficient delivery to customers. Their customer-centric approach prioritizes satisfaction, aiming to enhance the beverage experience for consumers of all backgrounds. Swire Coca-Cola manages distribution risks effectively through strategic planning and operational excellence, ensuring consistent availability and quality of products. Ultimately, Swire Coca-Cola is dedicated to promoting enjoyment and refreshment while contributing positively to the communities it serves.

### **Business Problem:** ###

- Swire Coca-Cola aims to optimize production planning and inventory management for its innovation products, necessitating accurate demand forecasting to prevent both out-of-stocks and overproduction.
- The challenge lies in predicting the demand for these new products at a weekly level, considering factors such as evolving consumer preferences, technological advancements, and regulatory changes.
- Accurate demand forecasting is essential for maximizing revenue and customer satisfaction while minimizing costs associated with inventory management and production.

### **Project Goal/Objective:** ###

The objective of the Swire Coca-Cola demand forecasting project is to develop a robust predictive model that accurately predicts the demand for innovation products at a weekly level. This involves leveraging historical data and incorporating relevant census data to derive actionable insights for optimal production planning and inventory management. Ultimately, the project aims to minimize costs, prevent stockouts, and maximize customer satisfaction, thereby driving revenue growth and sustaining long-term success in the dynamic beverage market.

### **Group's solution to the business problem:** ###

Initially, before the modeling process, data was cleaned, and joined, missing values were replaced, and additional variables were feature-engineered. We have then implemented 4 different machine-learning models namely - Logistic regression, Random forest, XGBoost, ARIMA time series forecasting and then chose XGBoost to make the demand predictions since XGBoost model performed well with the highest R-squared value, low RMSE , low MAE and low model run time.

The model was trained using a comprehensive set of variables extracted from the provided dataset.The categorical features such as caloric segment, category, manufacturer, brand, package size, and item description were incorporated to understand consumer preferences, product characteristics, and market segmentation. The market key identifier facilitated geographical analysis, enabling insights into regional variations in demand. Moreover, numerical data on unit sales and dollar sales provided essential metrics for evaluating sales performance and revenue generation. By considering these diverse variables, the model aimed to optimize demand forecasting accuracy by accounting for various factors influencing product sales across different markets and time periods.

XGBoost is preferred over other models due to its significantly higher R-squared value, indicating more accurate and reliable predictions with a better fit to the data. Its advantages include efficiency in handling large datasets, built-in regularization to reduce overfitting, flexibility across various predictive modeling problems, capability to handle missing data, and scalability for distributed computing. These features make XGBoost a versatile and powerful tool for predictive modeling, offering superior performance and computational efficiency, which is crucial for achieving high accuracy in our modeling task. We also performed cross-validation to assess the model's performance and ensure its generalization to new data.
XGBoost provides a highly efficient implementation of the gradient boosting algorithm, making it suitable for large datasets.

### **Results:** ###

The XGBoost model demonstrates outstanding predictive accuracy with an R-squared value of 0.96, implying it explains a vast majority of the variance in the dataset. The RMSE of 169.29 and MAE of 24.03 suggest the model's predictions are reasonably close to the actual values. These metrics, combined with a moderate execution time of 141 seconds, signify a robust performance that likely surpasses baseline predictive models.

### **Business Value to the solution:** ###
The application of XGBoost model for product demand forecasting offers substantial business value across various facets of a company's operations. Here's how the solutions provided above translate into business value:

1. **Strategic Product Launch Timing**: The model's ability to pinpoint peak demand weeks for specific products enables Swire-CC to strategically time their product launches, capitalizing on periods of high consumer interest, thereby maximizing sales and market penetration.
2. **Optimized Inventory Management**: By forecasting weekly demand with precision, the company can optimize its inventory levels, reducing the costs associated with overstocking or stockouts, and ensuring product availability aligns with consumer demand.
3. **Targeted Regional Marketing**: The model identifies the regions where specific products are predicted to perform best. This information can guide targeted marketing campaigns and resource allocation, increasing the effectiveness of promotional activities and boosting regional sales.
4. **Seasonal Trend Analysis**: Understanding seasonal trends and their impact on product performance allows for more efficient planning of production cycles, marketing efforts, and resource allocation throughout the year.
5. **Improved Supply Chain Coordination**: With demand forecasts in hand, Swire-CC can coordinate more effectively with suppliers and distributors, ensuring a smooth supply chain that can handle the predicted fluctuations in demand without disruption.

### **My contribution to the project:** ###
I was involved in the heavy-lifting part of the project. I have done the data preprocessing, missing data calculation, imputation, feature Engineering, different datasets(Fact market demand,Zipcode to Market key, Consumer demographics) aggregation for predictions, and Modeled using XGBoosting multiple times using different parameters and datasets.

### **Difficulties encountered during the project implementation:** ###
1. **Managing Product Variability**: One of the complexities we faced was the wide range of products, each with different demand patterns. To address this, we adopted a granular approach, customizing models for individual product categories to improve accuracy.
2. **In-depth Data Analysis**: The extensive dataset required a thorough Exploratory Data Analysis (EDA) to understand underlying trends and anomalies. This step was crucial in preparing the data for effective model training.
3. **Model Generalization**: Preventing overfitting was essential to ensure that our models could generalize well to unseen data. We employed techniques such as cross-validation and regularized learning to maintain a balance between bias and variance.
4. **Hyperparameter Tuning**: Identifying the best settings for the XGBoost model parameters was both resource-intensive and critical for performance. We leveraged automated hyperparameter optimization tools to expedite this process.

### **Learnings from the project implementation:** ###
For Swire, the implementation of predictive demand forecasting using XGBoost has been a journey of learning and refinement. Here are some key takeaways:
- **Customized Modeling**: An approach tailored to individual product lines led to more precise demand forecasts, acknowledging the distinct behavior of different market segments.
- **Deep Diving into Data**: Detailed data analysis not only prepared the data for modeling but also provided valuable business insights into consumption patterns.
- **Balanced Model Complexity**: Through cross-validation and regularization, we achieved models that are complex enough to capture underlying trends but simple enough to avoid overfitting.
- **Efficient Hyperparameter Optimization**: With a systematic search for the best hyperparameters, we could maximize model performance without incurring unnecessary computational costs.

For Swire, the implementation of predictive demand forecasting using XGBoost has been a journey of learning and refinement. Here are some key takeaways:




