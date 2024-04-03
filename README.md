# Cat and Dog image classifier - Machine Learning

This project is a Python-based implementation of a Convolutional Neural Network (CNN) for image classification. The model is trained and validated on a dataset of images, and then used to make predictions on a test set. The images are preprocessed and loaded using the ImageDataGenerator class from the tensorflow.keras.preprocessing.image module.

## Code Structure
The code is organized as follows:

* Data Preparation: The number of images in the training, validation, and test directories are calculated. These directories each contain subdirectories for each class of images.
* Preprocessing and Training Variables: Variables for preprocessing the images and training the model are defined. These include the batch size, number of epochs, and the dimensions to which all images will be resized.
* Image Data Generators: Image data generators for the training, validation, and test datasets are created using the ImageDataGenerator class. These generators read the images, decode them into floating point tensors, and rescale the tensors from values between 0 and 255 to values between 0 and 1.
* Model Construction: A CNN model is constructed using the Sequential class from the tensorflow.keras.models module. The model consists of several convolutional layers with increasing numbers of filters, followed by max pooling layers. After the convolutional base, the model includes a flatten layer and two dense layers.
* Model Compilation: The model is compiled with the Adam optimizer and binary cross entropy loss function, suitable for binary classification problems. The accuracy metric is used to evaluate the performance of the model.
* Model Training: The model is trained on the training data using the fit method. The validation data is used to validate the model during training.
* Model Evaluation: The trained model is used to make predictions on the test data. The predictions are then evaluated to determine the model's performance.

## Usage
To run the code, you will need Python installed on your machine. You will also need to install the necessary libraries, which include tensorflow, numpy, matplotlib, and os.

Once the necessary software is installed, you can run the code using a Python interpreter. The code will train and validate the model, and then use the model to make predictions on the test data.

### Contributing
Contributions are welcome. Please open an issue to discuss your ideas or submit a pull request with your changes.

### License
This project is licensed under the terms of the MIT license.
