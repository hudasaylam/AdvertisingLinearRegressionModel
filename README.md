# AdvertisingLinearRegressionModel
machine learning model to predict sales based on the number of advertisements across different media types using a linear regression model.
# Regression Model Analysis Project

This project involves developing a regression model to analyze and predict a target variable based on given features. The analysis includes detecting and handling outliers, evaluating model performance using metrics like RMSE and R² score, and visualizing the data to gain insights.

## Table of Contents

- [Project Overview](#project-overview)
- [Technologies Used](#technologies-used)
- [Data Preparation](#data-preparation)
- [Outlier Detection](#outlier-detection)
- [Model Training and Evaluation](#model-training-and-evaluation)
- [Results](#results)
- [Visualizations](#visualizations)
- [Conclusion](#conclusion)


## Project Overview

This project focuses on creating a linear regression model to predict a target variable, "Sales," based on different features such as "Newspaper." The model's performance is evaluated using RMSE and R² scores. Additionally, outlier detection technique such as IQR are employed to clean the data and improve model accuracy.

## Technologies Used

- Python
- Jupyter Notebook
- Libraries: NumPy, Pandas, Scikit-Learn, Matplotlib, Seaborn

## Data Preparation

- The dataset is loaded into a Pandas DataFrame for analysis.
- The dataset contains multiple features, including "Newspaper" and "Sales," used for predicting sales.
- Initial data visualization and statistical summaries are conducted to understand data distribution.

## Outlier Detection

   IQR method is used to detect and handle outliers in the data:

 **Interquartile Range (IQR) Method**:
   - Calculated the IQR for the "Newspaper" column.
   - Used the IQR to identify and remove data points outside the acceptable range (1.5 times the IQR).

## Model Training and Evaluation

- A linear regression model is trained using the cleaned dataset.
- The model is evaluated using:
  - **Root Mean Squared Error (RMSE):** 1.6881844417270029, indicating the average prediction error in the same units as the target variable.
  - **R² Score:** 0.8989454779619589, indicating that 89% of the variance in the target variable is explained by the model.

## Results

- The regression model demonstrates a strong fit with an R² score of 0.898, suggesting that it effectively captures the relationship between the input features and the target variable.
- The RMSE of 1.688 indicates a relatively low average prediction error.

## Visualizations




### Box Plot Before And After deleting the outliers

The box plot displays the spread and detects outliers for different features. The dots outside the box represent outliers that were identified and handled.

![image](https://github.com/user-attachments/assets/0441a183-6f16-4e8c-ae19-7946905d7a0d)
)
![image](https://github.com/user-attachments/assets/72668b1b-b041-404e-bde5-6c3a9600da56)

### Scatter Plot

This plot shows the relationship between "Newspaper" and "Sales." It displays a general upward trend but with some randomness, indicating a moderate correlation.

![image](https://github.com/user-attachments/assets/e152e314-f031-4416-a816-a73206845805)



## Conclusion

The project successfully builds a linear regression model with good performance metrics (RMSE and R² score). Outlier detection and removal improved the model's accuracy. Data visualizations provided valuable insights into feature relationships and distributions, enhancing model interpretation and reliability.



