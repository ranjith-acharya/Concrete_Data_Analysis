# Concrete_Data_Analysis
This repository contains code for a linear regression model on the Concrete Data. The following libraries were used:

<li>pandas
<li>numpy
<li>sklearn.model_selection.train_test_split
<li>sklearn.preprocessing.StandardScaler
<li>sklearn.linear_model.LinearRegression
<li>sklearn.metrics.mean_squared_error
<li>sklearn.metrics.mean_absolute_error
<li>sklearn.metrics.r2_score
<li>seaborn
<li>matplotlib.pyplot
# Dataset
The dataset used for this model is the Concrete Data, which can be found in the Dataset folder in the repository.<br>

# Preprocessing
Before training the model, the dataset was preprocessed in the following way:<br>

<li>Checked for null values in the dataset using the isnull().sum() method
<li>Checked for duplicated values in the dataset using the duplicated() method
<li>Removed duplicated values using the drop_duplicates() method
<li>Visualized the data using the pairplot() method from seaborn
<li>Checked for correlation in the dataset using the corr() method
<li>Visualized the correlation data using the heatmap() method from seaborn
<li>Visualized the boxplot for all the features using the boxplot() method from pandas

# Training and Testing
The data was split into training and testing sets using the train_test_split() method from sklearn. 
The testing set size was set to 30%.<br>

The StandardScaler() method from sklearn was used to standardize the data. The fit_transform() method was used for the training set, and the transform() method was used for the testing set.<br>

The linear regression model was then trained using the LinearRegression() method from sklearn.

# Model Evaluation
The model was evaluated using the following metrics:<br>

<li>Mean Squared Error (MSE)
<li>Square Root Mean Squared Error (RMSE)
<li>Mean Absolute Error (MAE)
<li>R2 Score
<li>Adjusted R2 Score

<br>
The performance metrics were calculated using the mean_squared_error(), sqrt() from numpy, mean_absolute_error(), r2_score(), and a custom formula for the adjusted R2 score.