# Bridge Condition Monitoring Project

This project aims to leverage Convolutional Neural Networks (CNN) for monitoring the condition of bridges. It includes two primary models: one for classifying the condition of bridge decks as 'poor' (cracked) or 'good' (not cracked), and another for predicting the remaining life of the bridge.

## Project Structure

- **spectoV1/**: Contains the code and resources for the classification model.
- **spectoV2/**: Contains the code and resources for the regression model predicting the remaining life of the bridge.

## Overview

### 1. Classification Model (spectoV1)

The classification model is designed to analyze images of bridge decks and classify their condition into two categories: 'poor' (cracked) or 'good' (not cracked).

### 2. Regression Model (spectoV2)

The regression model predicts the remaining useful life of a bridge based on the analysis of its deck images. This model provides a numerical output indicating the predicted lifespan in years.

## Installation

To run the models, you need to have the following installed:

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

## Usage 

Clone the repo 

```bash
git clone https://github.com/yourusername/bridge-condition-monitoring.git
cd bridge-condition-monitoring
```

## Running the models 

### Classification Model 

Navigate to the spectoV1 directory and follow the instructions in the README.md file to run the classification model.

```bash
cd spectov1
```

### Regression Model 

Navigate to the spectoV2 directory and follow the instructions in the README.md file to run the regression model.

```bash
cd spectov2
```


## Future Scopes 
- Integration with IoT: Combine the CNN models with IoT sensors for real-time monitoring and predictive maintenance.
- Advanced Anomaly Detection: Implement more sophisticated algorithms for detecting subtle and complex structural issues.
- Extended Data Sources: Incorporate additional data types, such as thermal imaging and Lidar scans, for comprehensive analysis.
- Scalability: Expand the solution to monitor multiple bridges simultaneously using cloud-based services.
- Automated Reporting: Develop automated reporting tools to generate actionable insights and maintenance schedules.
