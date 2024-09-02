# Digit Recognizer with TensorFlow

This project implements a Convolutional Neural Network (CNN) model using TensorFlow to identify handwritten digits. The model is trained and validated on the MNIST dataset, a widely used collection of handwritten digits for training and testing in machine learning.

## Project Structure

The project is organized as follows:

1. **Data Loading and Preprocessing:** The training and testing data are loaded and preprocessed. Images are normalized and reshaped to the required dimensions for the CNN. Labels are converted to one-hot encoding.

2. **Data Augmentation:** The training dataset is augmented to enhance the variety of data available for model training without the need for new data collection. This involves applying rotations, shifts, and zooms.

3. **Model Building:** The CNN model is constructed using Keras' Sequential API. It consists of multiple convolutional layers, max pooling layers, dense layers, and dropout layers.

4. **Model Training:** The model is trained for 20 epochs using the Adam optimizer and categorical cross-entropy as the loss function. Callbacks for reducing the learning rate and saving model checkpoints are implemented.

5. **Model Evaluation:** The accuracy and loss of the model are plotted for both training and validation sets to evaluate its performance.

## Running the Model

To execute the model, simply run the Python script. The script will train the model and save the predictions for the test dataset in a file named `submission.csv`. This file contains two columns: `ImageId` and `Label`, representing the image ID from the test dataset and the predicted digit, respectively.

## Dependencies

This project requires the following libraries:

- TensorFlow
- Keras
- NumPy
- Pandas
- Matplotlib

## Setup

This application requires Python 3.6 or higher. You can install all necessary libraries using the following command:

```shell
pip install -r requirements.txt
