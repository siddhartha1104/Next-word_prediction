# Next Word Prediction using LSTM

## Project Overview

This project aims to develop a deep learning model for predicting the next word in a given sequence of words. The model is built using Long Short-Term Memory (LSTM) networks, which are well-suited for sequence prediction tasks. The project includes the following steps:

1. **Data Collection**: We use the text of Shakespeare's _Hamlet_ as our dataset. This rich, complex text provides a good challenge for our model.

2. **Data Preprocessing**: The text data is tokenized, converted into sequences, and padded to ensure uniform input lengths. The sequences are then split into training and testing sets.

3. **Model Building**: An LSTM model is constructed with an embedding layer, two LSTM layers, and a dense output layer with a softmax activation function to predict the probability of the next word.

4. **Model Training**: The model is trained using the prepared sequences, with early stopping implemented to prevent overfitting. Early stopping monitors the validation loss and stops training when the loss stops improving.

5. **Model Evaluation**: The model is evaluated using a set of example sentences to test its ability to predict the next word accurately.

6. **Deployment**: A Streamlit web application is developed to allow users to input a sequence of words and get the predicted next word in real-time.

## Prerequisites

- Python 3.11
- Conda (Optional but recommended)

## Setup and Installation

Follow these steps to run the project on your machine:

1. **Clone the repository**

   ```bash
   git clone <repository_url>
   cd <repository_folder>
   ```

2. **Create a virtual environment**

   ```bash
   conda create -p venv python=3.11 -y
   ```

3. **Activate the virtual environment and install dependencies**

   ```bash
   conda activate venv
   pip install -r requirements.txt
   ```

4. **Run the Streamlit application**
   ```bash
   streamlit run app.py
   ```

## Usage

- Open the provided Streamlit web interface.
- Enter a sequence of words in the input field.
- The model predicts and displays the most probable next word.

## Technologies Used

- Python 3.11
- TensorFlow/Keras (for deep learning)
- Streamlit (for web deployment)
- Natural Language Processing (NLP) techniques
