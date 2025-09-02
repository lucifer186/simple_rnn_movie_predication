# IMDB Movie Review  Simple RNN

## Overview
This project aims to build a sentiment analysis application using a Simple Recurrent Neural Network (RNN) trained on the IMDB movie review dataset. The goal is to classify movie reviews as either positive or negative based on the text content. The project involves training a Simple RNN model using TensorFlow, saving the trained model, and creating an interactive web application with Streamlit to allow users to input their own movie reviews and receive sentiment analysis results in real-time.

## Features
Data Preprocessing: The IMDB dataset is preprocessed to convert reviews into sequences of integers, which are then padded to ensure uniform input length.
Model Training: A Simple RNN model is trained on the preprocessed data, using an embedding layer and a recurrent layer with 128 units.
Early Stopping: The training process includes early stopping to prevent overfitting and to restore the best weights based on validation loss.
Model Saving: The trained model is saved as an H5 file for later use in the Streamlit application.
Interactive Web Application: A Streamlit-based web application is developed to allow users to input movie reviews and get real-time sentiment analysis results. The application visualizes the sentiment distribution using a pie chart.

## Getting Started
Prerequisites \
Ensure you have the following libraries installed:

TensorFlow \
Streamlit \
Plotly \
Numpy 

You can install these libraries using pip:
`pip install tensorflow streamlit plotly numpy`

## Project Structure
app.py: The main Streamlit application script that loads the model, processes user input, and displays sentiment analysis results.
simple_rnn_imdb.h5: The saved Simple RNN model trained on the IMDB dataset.
README.md: Project documentation and overview.
Running the Application
Clone the repository to your local machine.
Ensure that simple_rnn_imdb.h5 is in the same directory as app.py.
Run the Streamlit application using the following command:
`streamlit run app.py`
Open the provided local URL in your web browser to interact with the application.

## Usage
Open the Streamlit web application.
Enter a movie review in the text area provided.
Click the "Analyze" button.
View the sentiment analysis result, including the predicted sentiment (Positive/Negative) and the confidence level.
A pie chart will visualize the sentiment distribution.
