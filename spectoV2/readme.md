# SpectoV2 - Bridge Deck Life Prediction

SpectoV2 is a Convolutional Neural Network (CNN) model designed to predict the remaining useful life of bridge decks based on images.

NOTE -- PREDICTIONS MAY NOT BE ACCURATE AS MODEL HAS BEEN TRAINED ONLY ON A SMALL DATASET AS PROOF OF CONCEPT. 

## Project Structure

- **Step 1:** Import necessary libraries and define constants.
- **Step 2:** Load and preprocess images, and split the data into training and testing sets.
- **Step 3:** Define a data generator for efficient batch processing.
- **Step 4:** Define the EfficientNetB0-based regression model architecture.
- **Step 5:** Compile and train the model using the training dataset and validate it using the validation dataset.
- **Step 6:** Predict the remaining life of bridge decks for sample images.

## Installation

To run the model, you need to have the following installed:

- Python 3.6+
- TensorFlow
- Keras
- NumPy
- Pillow
- Scikit-learn

You can install the required packages using pip:

```bash
pip install tensorflow keras numpy pillow scikit-learn
```

## Running the code 
- Load and Preprocess Data:

    Ensure the dataset is organized with ‘Cracked’ and ‘Non-cracked’ directories.

    Modify the cracked_dir and non_cracked_dir variables in Cell 2 to point to your dataset.
- Train the Model:

  Run the cells sequentially to load data, create datasets, and train the model.
- Evaluate the Model:
  
  Use the validation dataset to evaluate model performance during training.
- Predict Remaining Life:
  
    Use the provided function to predict the remaining life of bridge decks for given images.

## Model architecture 

The CNN model is based on EfficientNetB0 and consists of the following layers:

- EfficientNetB0 Base Model: Pretrained on ImageNet, used for feature extraction.
- GlobalAveragePooling2D Layer: Reduces the spatial dimensions of the feature maps.
- Dense Layer (1024 units, ReLU activation)
- Dropout Layer (0.5 rate)
- Dense Layer (512 units, ReLU activation)
- Dropout Layer (0.5 rate)
- Dense Layer (1 unit, linear activation): Outputs the predicted remaining life.

## Results 

*not accurate only a proof of concept 

<img width="533" alt="Screenshot 2024-07-12 at 5 18 21 PM" src="https://github.com/user-attachments/assets/c00082b9-1102-4e75-8cba-a4effea94728">
