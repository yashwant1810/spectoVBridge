# SpectoV1 - Bridge Deck Condition Classification

SpectoV1 is a Convolutional Neural Network (CNN) model designed to classify bridge deck images as either 'cracked' (poor condition) or 'non-cracked' (good condition).

NOTE - RESULTS MAY VARY FOR EACH RUN AS DATASET IS SMALL. MORE DATA NEEDED FOR EXTENSIVE TRAINING

## Project Structure

- **Cell 1:** Import necessary libraries and define constants.
- **Cell 2:** Load and preprocess images, and split the data into training, validation, and test sets.
- **Cell 3:** Create an ImageDataGenerator for the test set.
- **Cell 4:** Create tf.data.Dataset objects for training and validation sets.
- **Cell 5:** Define the CNN model architecture and compile the model.
- **Cell 6:** Train the model using the training dataset and validate it.
- **Cell 7:** Plot training history for accuracy and loss.
- **Cell 8:** Evaluate the model on the test dataset.
- **Cell 9:** Import necessary libraries for inference.
- **Cell 10:** Define image paths for prediction and preprocess the images.
- **Cell 11:** Generate predictions for the sample images.
- **Cell 12:** Define a function to draw bounding boxes on images and visualize the predictions.

## Installation

To run the model, you need to have the following installed:

- Python 3.6+
- TensorFlow
- Keras
- NumPy
- Pillow
- OpenCV
- Matplotlib

You can install the required packages using pip:

```bash
pip install tensorflow keras numpy pillow opencv-python matplotlib
```
## Running the model 

- Load and Preprocess Data:

    Ensure the dataset is organized with ‘Cracked’ and ‘Non-cracked’ directories.

    Modify the cracked_dir and non_cracked_dir variables in Cell 2 to point to your dataset.
- Train the Model:
  
    Run the cells sequentially to load data, create datasets, and train the model.

- Evaluate the Model:
  
    Use Cell 8 to evaluate the model on the test dataset.
- Generate Predictions:
  
    Use Cells 10 to 12 to load sample images, generate predictions, and visualize the results.

## Model architecture 

The CNN model consists of the following layers:

- Conv2D Layer (32 filters, 3x3 kernel, ReLU activation)
- MaxPooling2D Layer (2x2 pool size)
- Conv2D Layer (64 filters, 3x3 kernel, ReLU activation)
- MaxPooling2D Layer (2x2 pool size)
- Conv2D Layer (128 filters, 3x3 kernel, ReLU activation)
- MaxPooling2D Layer (2x2 pool size)
- Flatten Layer
- Dense Layer (128 units, ReLU activation)
- Dropout Layer (0.5 rate)
- Dense Layer (1 unit, sigmoid activation)

## Results 
<img width="923" alt="Screenshot 2024-07-12 at 5 06 55 PM" src="https://github.com/user-attachments/assets/01580daf-1b90-4dab-a6f9-509c0a398657">

<img width="931" alt="Screenshot 2024-07-12 at 5 08 14 PM" src="https://github.com/user-attachments/assets/bb39ea51-b831-42ad-8305-25df3ee09894">

<img width="669" alt="Screenshot 2024-07-12 at 5 09 39 PM" src="https://github.com/user-attachments/assets/b9ebd6ed-2f89-49ab-aa4d-2aaf8328cdd6">

<img width="667" alt="Screenshot 2024-07-12 at 5 10 16 PM" src="https://github.com/user-attachments/assets/c5ba3b09-de41-43ed-aac2-3f6d73c1889a">


