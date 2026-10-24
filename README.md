# MNIST Handwritten Digit Classifier with PyTorch

A handwritten digit classification project built with PyTorch and trained on the MNIST dataset. The model achieved **97.64% test accuracy** after 5 epochs of training.

## Overview

This project uses a fully connected neural network to recognize handwritten digits from 0 to 9. It takes a 28×28 grayscale image as input and predicts the digit represented by that image.

The project was developed in Google Colab as a practical introduction to deep learning and PyTorch.

## Technologies Used

- Python
- PyTorch
- Torchvision
- Matplotlib
- Google Colab

## Dataset

The project uses the MNIST handwritten digit dataset.

- Training images: 60,000
- Testing images: 10,000
- Image dimensions: 28 × 28 pixels
- Image type: Grayscale
- Classes: 10 digits (0–9)

## Model Architecture

The neural network consists of the following layers:

| Layer | Description |
|---|---|
| Flatten | Converts each image into 784 features |
| Linear | Maps 784 input features to 128 neurons |
| ReLU | Adds non-linearity |
| Linear | Produces 10 output scores, one for each digit |

## Training Configuration

- Loss function: CrossEntropyLoss
- Optimizer:Adam
- Learning rate: 0.001
- Epochs: 5
- Batch size: 32

## Results

| Metric | Result |
|---|---:|
| Test accuracy | 97.64% |
| Training epochs | 5 |
| Output classes | 10 |

The model was evaluated on the separate MNIST test dataset to measure its ability to classify images it did not train on.

## Project Structure

```text
mnist-digit-classifier/
├── pytorch.ipynb
├── mnist_digit_classifier.pth
├── requirements.txt
└── README.md
```

- `pytorch.ipynb` — Notebook containing the implementation and experiments.
- `mnist_digit_classifier.pth` — Saved trained model parameters.
- `requirements.txt` — Python package dependencies.
- `README.md` — Project documentation.

## How to Run

### 1. Clone the repository

```bash
git clone https://github.com/israel77798755/mnist-digit-classifier.git
cd mnist-digit-classifier
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Run the notebook

Open `pytorch.ipynb` in Jupyter Notebook or upload it to Google Colab, then execute the cells in order.

The notebook downloads the MNIST dataset when necessary, builds the neural network, trains the model, and evaluates its test accuracy.

## What I Learned

- Loading datasets with Torchvision
- Working with tensors and DataLoader
- Building neural networks using `nn.Module`
- Forward propagation and loss calculation
- Backpropagation and gradient-based optimization
- Training and evaluating a neural network
- Saving trained model parameters

## Future Improvements

- Build an interactive digit-recognition application using Gradio.
- Allow users to draw digits and receive predictions.
- Explore convolutional neural networks (CNNs).
- Deploy the model as a web application.

## Author

Israel Tsegaye Abino

Information Science Student | Aspiring AI Engineer
