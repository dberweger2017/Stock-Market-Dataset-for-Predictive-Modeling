# Stock Market Dataset for Predictive Modeling
This project involves a comprehensive analysis of a historical stock market dataset with the aim of building a predictive model using Long Short-Term Memory (LSTM), a type of Recurrent Neural Network (RNN).

## Dataset
The dataset utilized in this project was constructed to capture weekly stock market data across several sectors, from 1980 till present. The dataset features multiple data points including 'Open', 'High', 'Low', 'Close', 'Adjusted Close', 'Volume', 'Symbol', and 'Sector'. Further, data related to additional market indicators such as the 'Volatility Index (VIX)' and '10-year Bond Yield' were also added to the dataset for comprehensive analysis.

## Approach
The methodology adopted in this investigation is as follows:

1. Exploratory Data Analysis: All the unique stocks in the dataset were identified, distribution across different sectors checked, and missing values in the dataset dealt with.

2. Data Augmentation with VIX and Bond_Yield: To enhance the potential predictive validity of the predictive model, additional market indices: VIX and 10 year Bond_Yield were added to the dataset, thus improving distinguishing features in the dataset.

3. Correlation Analysis: Correlation among variables in the dataset were analyzed, providing insights on the relationship of different factors with each other.

4. Prediction Model with LSTM: After EDA and data augmentation, a predictive model was trained using LSTM methodology due to its competencies in handling sequential data. The LSTM model was utilized to predict the 'Adjusted Close' stock prices.

## Results
The Root Mean Square Error (RMSE) on the training set is approximately 9.21, indicating the model's predictions were close to the actual prices on the training data. However, the model's performance on the test data can be improved further (Test RMSE = 74.96), suggesting that the model could be overfitting to the training data. Several strategies including increasing the training data, reducing model complexity, regularization, and early stopping might help improvise the model predictions.

## Future Improvements
Given the results, future improvements to this project could include:

1. Testing more stocks or adding additional market indicators (such as commodities prices or foreign exchange rates) to provide a more diverse set of inputs for model training.
   
2. Exploring other types of machine learning models, such as transformers, for comparison and potentially improved performance.

3. Experimenting with different strategies to handle missing data in the VIX and Bond_Yield columns to check if that improves the model predictive quality.

4. Trying out different approaches for feature selection.
