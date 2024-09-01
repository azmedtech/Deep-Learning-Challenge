# Deep Learning Challenge

## Overview

The goal of this project is to develop a predictive model for Alphabet Soup, a nonprofit foundation, to identify which funding applicants are most likely to succeed with the financial support they receive. Using historical data on funded organizations, a neural network model has been created to predict the success of future applicants. This model aims to enhance the efficiency and effectiveness of Alphabet Soup funding decisions by accurately predicting successful outcomes.

## Project Instructions

### Prerequisites

Ensure you have the following libraries installed:

- pandas
- numpy
- scikit-learn
- tensorflow
- keras

### Data Preprocessing

1. **Load the Data**: Read `charity_data.csv` into a Pandas DataFrame.
2. **Identify Target and Features**:
   - **Target Variable**: `IS_SUCCESSFUL` (1 for successful, 0 for unsuccessful).
   - **Feature Variables**: All columns except `IS_SUCCESSFUL`, `EIN`, and `NAME`.
3. **Preprocessing Steps**:
   - Drop `EIN` and `NAME` columns.
   - Handle categorical variables by encoding them using `pd.get_dummies()`.
   - Scale the feature data using `StandardScaler`.
   - Split the data into training and testing datasets.

### Model Training

1. **Build the Model**:
   - Create a neural network with two hidden layers.
   - Initial layer configuration: 30 neurons in the first hidden layer, 10 neurons in the second hidden layer.
   - Activation function: ReLU.
2. **Compile and Train**:
   - Compile the model with an appropriate optimizer and loss function.
   - Train the model using the training dataset.
   - Evaluate the model on the test dataset.
3. **Save the Model**:
   - The trained model is saved as `AlphabetSoupCharity.h5`.

### Model Optimization

1. **Optimization Attempts**:
   - Experiment with different configurations (number of layers, neurons, activation functions).
   - Document each attempt and its performance.
2. **Save the Optimized Model**:
   - The optimized model is saved as `AlphabetSoupCharity_Optimization.h5`.

### Running the Code

To run the Jupyter notebooks:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/deep-learning-challenge.git
   cd deep-learning-challenge
   ```
2. **Open Jupyter Notebook**:
   ```bash
   jupyter notebook
   ```
3. **Open and Execute**:
   - Start with `Data_Preprocessing_Code.ipynb` to preprocess the data in your local code editor.
   - Open the `Data_Preprocessing_Code.ipynb` in Google CoLaboratory and proceed to build and evaluate the initial model.
   - Use `AlphabetSoupCharity_Optimization.ipynb` for optimization attempts and saving the final model.

## Report

- **Neural Network Report.md**: This file provides a detailed analysis of the deep learning model, including the purpose, results, optimization attempts, and recommendations.
- **Images/**: This folder contains screenshots and images referenced in the `Neural Network Report.md`.

## Summary

The project involves preprocessing historical funding data, developing a neural network model, and optimizing it to predict the success of future applicants. If the neural network model does not achieve the target accuracy, consider exploring alternative models such as ensemble methods for potentially better performance.

## Collaboration
- Colleagues collaboration - model optimization discussions with J Bourbon.
- Debugging assistance - ASU Xpert Learning Assistant and Tutors