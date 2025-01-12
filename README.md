This project aims to predict future temperatures using historical weather data and real-time weather forecasts obtained through the OpenWeatherMap API. 
The model leverages an Artificial Neural Network (ANN) to make accurate predictions based on several weather parameters.

Project Workflow:

Data Collection:
Retrieves real-time 5-day weather forecast data for a specified city using OpenWeatherMap API.
Loads historical weather data from a CSV file to train the ANN model.

Data Preparation:
Cleans the historical weather data by removing duplicates and handling missing values.
Normalizes the data using MinMaxScaler for improved ANN performance.
Splits the data into training and testing sets.

Model Building:
Constructs an ANN model using TensorFlow and Keras, consisting of multiple dense layers with ReLU activations and a linear output layer for regression tasks.
Compiles the model with adam optimizer and mean_squared_error loss function, aiming for high accuracy in temperature prediction.

Model Training:
Trains the ANN model on the prepared dataset with early stopping to prevent overfitting.
Evaluates the model's performance using metrics like Mean Squared Error (MSE), Mean Absolute Error (MAE), and R-squared (R²).

Prediction and Evaluation:
Uses the trained model to predict future temperatures based on the latest weather data.
Compares predicted temperatures with actual forecasted temperatures to evaluate the model's performance.

Output:
Displays the weather forecast alongside the ANN's predicted future temperatures for the next day.
Provides a comprehensive view of current weather conditions and predicted trends.

Key Features:
Real-Time Weather Forecasting: Incorporates live weather data from the OpenWeatherMap API.
ANN for Prediction: Utilizes a multi-layered ANN to predict future temperatures based on historical and current weather data.
Performance Metrics: Evaluates the model using industry-standard metrics like MSE, MAE, and R² to ensure accuracy and reliability.
Scalable: Designed to accommodate data from multiple cities and various weather parameters for broader applications.
