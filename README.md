# PyDCNN


## Overview
This project implements a deep convolutional neural network (CNN) to classify handwritten digits from the MNIST dataset. The goal of this project was to design, train and evaluate a high-performance image classification model in Python while gaining hands-on experience with deep learning workflows and computer vision techniques.

![PyDCNN Architecture](https://raw.githubusercontent.com/bchafe/PyDCNN/refs/heads/main/images/architecture.png)

## Objectives
- Design and implement a deep learning model for image classification
- Incorporate convolutional layers to extract visual features
- Optimize model performance through training and evaluation
- Understand end-to-end machine learning pipelines for computer vision

## Dataset
- Dataset: [MNIST Handwritten Digits](https://en.wikipedia.org/wiki/MNIST_database)
- Classes: 10 (digits 0-9)
- Image size: 28x28 
- Training samples: 60000
- Test samples: 10000

## Tools & Technologies
- Python
- PyTorch
- NumPy
- Matplotlib

## Methodology
### 1. Data Exploration
- Visualized a subset of training images to better understand data
- Plotted the distribution of the training set to ensure uniform representation across classes
- Compared the train and test splits to verify adequate sample sizes

### 2. Model Design
- Designed CNN architecture inspired by [VGGNet](https://en.wikipedia.org/wiki/VGGNet)
- Implemented stacks of 3x3 convolutional layers to extract spatial features
- Terminated network architecture with linear layers to interpret final prediction

### 3. Model Training 
- Create training loop to classify training data and calculate cross-entropy loss
- Ran backpropagation to update weights based on loss for each epoch
- Refined hyperparameters through iterative training & evaluation

### 4. Evaluation
- Evaluated model using test dataset
- Measured performance using accuracy and loss metrics
- Analyzed prediction results to verify model effectiveness

## Results
- Achieved 99.29% accuracy on the MNIST test dataset
- Model successfully learned distinguishing features of handwritten digits
- Demonstrated strong generalization performance on unseen data

## Classification Demo
![Visualizing classification results using first 36 digits of MNIST test set](https://raw.githubusercontent.com/bchafe/PyDCNN/refs/heads/main/images/classification-demo.png)

## Limitations
- Model trained on a relatively simple dataset (MNIST)
- Performance may not directly translate to more complex real-world image data
- Limited hyperparameter tuning and architecture experimentation

## Future Improvements
- Experiment with deeper architectures and regularization techniques
- Apply data augmentation to improve robustness
- Perform automated hyperparameter tuning to maximize performance
- Test model on more complex datasets (CIFAR-10)
- Deploy model as part of a larger application

## How to Run
### Method 1: Google Colab (Recommended)
1. [Open this notebook](https://colab.research.google.com/drive/1PxygFhHZ_kf95_bHYWNGYntDR2VkCC8L?usp=sharing) in Google Colab
2. Run each code cell in order
3. If you'd prefer to evaluate the model without training it yourself, download the model [here](https://github.com/bchafe/PyDCNN/raw/refs/heads/main/PyDCNN.pkl) and follow the instructions in the notebook
### Method 2: Run the notebook locally
1. Clone this repository
2. Open a shell in the cloned directory and install dependencies:
```
python -m venv venv

source venv/bin/activate    # Mac/Linux
venv\Scripts\activate       # Windows

pip install -r requirements.txt
```
3. Open the notebook in JupyterLab or VS Code
4. Run each code cell in order
5. If you'd prefer to evaluate the model without training it yourself, simply skip the training section in the notebook and run the code block to import the model. The pre-trained model is automatically included as part of this repository.








 

