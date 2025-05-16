Seoul Bike Sharing Demand Prediction
Overview
This project aims to predict the number of rented bikes in Seoul using regression models based on the Seoul Bike Sharing Demand dataset. By leveraging environmental and temporal features, the project employs Linear Regression and Random Forest Regressor to achieve accurate predictions, with model performance evaluated using R², MAE, and RMSE 4-class brain tumor classification. The project includes exploratory data analysis, model comparison, and feature importance visualization to understand key factors influencing bike rentals.
Features

Data Preprocessing: Removed irrelevant columns (Date, Seasons, Functioning Day) and applied one-hot encoding for categorical variables (Holiday).
Exploratory Data Analysis: Visualized feature correlations using a heatmap to identify relationships between variables like temperature and bike rentals.
Model Development: Implemented and compared Linear Regression and Random Forest Regressor models to predict bike rental counts.
Evaluation: Assessed models using R² Score, Mean Absolute Error (MAE), and Root Mean Squared Error (RMSE).
Visualization: Generated a correlation matrix and feature importance plots to highlight influential factors such as hour and temperature.

Technologies Used

Python: Core programming language.
Pandas & NumPy: For data manipulation and preprocessing.
Scikit-learn: For regression models and evaluation metrics.
Seaborn & Matplotlib: For data visualization (correlation matrix and feature importance).

Dataset

Seoul Bike Sharing Demand (sourced from Kaggle or UCI).
Features: Hour, Temperature, Humidity, Wind Speed, Visibility, Dew Point Temperature, Solar Radiation, Rainfall, Snowfall, Holiday (one-hot encoded).
Target: Rented Bike Count (number of bikes rented per hour).
Size: Approximately 8,760 records (hourly data for one year).
Accessible via Kaggle.

Installation

Clone the repository:git clone https://github.com/Aerglo/seoul-bike-sharing-prediction.git


Install dependencies:pip install pandas numpy scikit-learn seaborn matplotlib


Download the Seoul Bike Sharing Demand dataset and place it in the data/ folder.
Run the Jupyter notebook:jupyter notebook bike_data_sharing.ipynb



Usage

Open the bike_data_sharing.ipynb notebook.
Execute cells to preprocess data, train models, evaluate performance, and visualize results.
Outputs include:
R², MAE, and RMSE for Linear Regression and Random Forest models.
Correlation matrix heatmap.
Feature importance plot for Random Forest.



Results

Model Performance: Random Forest outperformed Linear Regression, with higher R² and lower MAE/RMSE (exact values depend on train-test split).
Key Insights: Hour and Temperature were the most influential features for predicting bike rentals, as shown by feature importance analysis.
Visualizations: Correlation matrix revealed strong relationships between temperature and bike rentals, while feature importance highlighted temporal and environmental factors.

Future Improvements

Incorporate additional features like day of the week or public events to improve model accuracy.
Experiment with advanced models like XGBoost or neural networks.
Add cross-validation to ensure robust performance.
Develop a web interface for real-time bike rental predictions.

Contact
For questions or feedback, reach out at imnima82@gmail.com or via GitHub.
