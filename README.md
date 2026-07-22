# SMART POER PLANT POWER GENERATION FORECASTER

# OVERVIEW

This project uses an Artificial Neural Network (ANN) built with PyTorch to predict the electrical energy output of a combined cycle power plant. The model learns the relationship between environmental conditions and the generated power, helping improve energy forecasting and plant efficiency.

# FEATURES

Data preprocessing using Pandas and NumPy
Train-test split with Scikit-learn
Feature scaling using StandardScaler
ANN implemented using PyTorch
Two hidden layers with ReLU activation
Optimized using the Adam optimizer
Mean Squared Error (MSE) as the loss function
Saves the best-performing model during training
Performance evaluation using MSE and R² Score
Dataset

The dataset contains operational parameters collected from a combined cycle power plant.

# FEATURE DESCRIPTION

AT -  Ambient Temperature
V - Exhaust Vacuum
AP - Ambient Pressure
RH - Relative Humidity
PE - Electrical Energy Output (Target Variable)

# TECH STACK
Python
PyTorch
Pandas
NumPy
Scikit-learn

# MODEL ARCHITECTURE

Input Layer (4 Features)

⬇

Hidden Layer 1

6 Neurons
ReLU Activation

⬇

Hidden Layer 2

6 Neurons
ReLU Activation

⬇

Output Layer

1 Neuron (Power Output Prediction)

# Workflow

1) Load the dataset.

2) Separate input features and target variable.

3) Split the dataset into training and testing sets.

4) Standardize the input features.

5) Convert data into PyTorch tensors.

6) Create DataLoaders for batch training.

7) Build the ANN model.

8) Train the network using backpropagation and Adam optimizer.

9) Save the best-performing model.

10) Evaluate the model using MSE and R² Score.

11) Training Configuration

Parameter	Value
Epochs	100
Batch Size	32
Optimizer	Adam
Loss Function	Mean Squared Error (MSE)
Hidden Layers	2
Activation	ReLU
Evaluation Metrics

The model is evaluated using:

Mean Squared Error (MSE)
R² Score

These metrics measure prediction accuracy and how well the ANN explains the variance in power output.

# PROJECT STRUCTURE

Smart-Power-Generation-Forecasting/
│
├── powerplant_data.csv
├── best_model.pt
├── power_prediction.py
├── README.md
└── requirements.txt

Installation

git clone https://github.com/yourusername/Smart-Power-Generation-Forecasting.git

cd Smart-Power-Generation-Forecasting

pip install -r requirements.txt

Run the Project

python power_prediction.py

Future Improvements

Hyperparameter tuning

Dropout for regularization

Early stopping

Model deployment using Flask/FastAPI

Interactive dashboard with Streamlit

Compare ANN with XGBoost, Random Forest, and LSTM

Author

Arav Kumar

Deep Learning • Machine Learning • Artificial Intelligence