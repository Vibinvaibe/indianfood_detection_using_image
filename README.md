# indianfood_detection_using_image
# README

This repository contains a Python script that utilizes TensorFlow and Keras to train a Siamese Neural Network for image classification. The script performs the following tasks:

1. Imports necessary libraries and modules such as numpy, pandas, os, matplotlib.pyplot, tensorflow, cv2, random, and time.
2. Loads the dataset from a CSV file and image directory.
3. Preprocesses the images and divides them into training, validation, and testing sets.
4. Defines a Siamese Neural Network model using VGG19 as the base model.
5. Creates pairs of images and their corresponding labels for training, validation, and testing.
6. Computes the Euclidean distance between the feature vectors of two input images.
7. Compiles and trains the Siamese Neural Network model using the created pairs.
8. Evaluates the model's performance on the testing set and computes accuracy.
9. Provides a function to load new images and predict their labels based on the trained model.
10. Displays the predicted label for a given image.

## Prerequisites

Before running the script, make sure you have the following:

1. Python 3.x installed on your system.
2. Required Python libraries installed, including numpy, pandas, matplotlib, tensorflow, cv2, and keras.

## Dataset

The script assumes that the dataset is stored in the following locations:

1. CSV file: `E:\datasets\self_food\self_food_data.csv`
2. Image directory: `E:\datasets\image_set01\Indian Food Images\Indian Food Images`

Please adjust the paths accordingly if your dataset is located elsewhere.

## Running the Script

To run the script, perform the following steps:

1. Install the required libraries by running the command `pip install numpy pandas matplotlib tensorflow opencv-python keras`.
2. Open a Python IDE or text editor.
3. Copy and paste the provided script into a new Python file.
4. Modify the paths of the CSV file and image directory if necessary.
5. Save the file with a `.py` extension (e.g., `siamese_nn.py`).
6. Run the script, and the training process will begin.
7. After training, the model will be evaluated on the testing set, and the accuracy will be displayed.
8. To predict the label for a new image, modify the `image_path` variable with the path to the image and run the script again.

Note: The script assumes that the image to be predicted is in the same format as the images in the training set (200x200 pixels, RGB color). Make sure the input image matches this format.

## Results

Upon running the script, the training process will be displayed in the console, including the loss and accuracy for each epoch. After training, the model will be evaluated on the testing set, and the accuracy score will be shown. Finally, if provided with a new image, the script will predict the label for that image based on the trained model and display it.

Feel free to customize the script according to your specific requirements and dataset. Enjoy experimenting with the Siamese Neural Network for image classification!
