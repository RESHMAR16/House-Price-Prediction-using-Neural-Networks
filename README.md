# House-Price-Prediction-using-Neural-Networks
A simple neural network model built with TensorFlow to predict house prices based on area, bedrooms, and age of the house.

This project uses a simple Artificial Neural Network (ANN) built with TensorFlow and Keras to predict house prices based on features such as area (sq. ft), number of bedrooms, and age of the house.

# Overview
The goal of this project is to demonstrate how a basic deep learning model can predict house prices from a few numerical inputs. The model learns patterns from a small dataset and estimates the price of a new house.

# Tech Stack
1. Python 3
2. TensorFlow / Keras
3. NumPy

# Model Architecture

Input Layer: 3 features (Area, Bedrooms, Age of the house)

Hidden Layer 1: 10 neurons, ReLU activation

Hidden Layer 2: 5 neurons, ReLU activation

Output Layer: 1 neuron (Predicted price)

# Model Training

The model is compiled using:

optimizer='adam'
loss='mse'
metrics=['mse']

Trained for 100 epochs with a batch size of 1.

# Model Performance

As training progresses, the Mean Squared Error (MSE) gradually decreases, indicating the model’s learning improvement.

Final MSE after 100 epochs ≈ 60.0

# Prediction Example
new_house = np.array([[1400, 3, 8]])
price = model.predict(new_house)
print("Predicted Price:", price)

Output:

Predicted Price: [[84.43975]]

The model predicts a house with 1400 sq.ft, 3 bedrooms, and 8 years old, to cost around ₹84.4 Lakhs.
