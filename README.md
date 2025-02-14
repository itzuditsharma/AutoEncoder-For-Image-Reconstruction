# CNN-Based Autoencoder

This repository contains a **Convolutional Autoencoder** implemented using PyTorch. The autoencoder is trained on the MNIST dataset to learn compressed representations of handwritten digits.

## Features
- Implements a **CNN-based Autoencoder** using PyTorch.
- Trains on the **MNIST dataset** (handwritten digits).
- Uses **Convolutional layers** for encoding and decoding.
- Visualizes reconstructed images after training.

## Installation
Ensure you have Python installed, then install the required dependencies:
```bash
pip install torch torchvision matplotlib
```

## Dataset
The model is trained on the **MNIST** dataset, which is automatically downloaded via `torchvision.datasets.MNIST`.

## Model Architecture
The autoencoder consists of:
- **Encoder**: A series of convolutional layers that downsample the input.
- **Decoder**: Transposed convolutional layers to reconstruct the original image.

## Usage
Run the script to train the autoencoder:
```bash
python train.py
```

## Training Details
- **Loss Function**: Mean Squared Error (MSE)
- **Optimizer**: Adam (or SGD)
- **Batch Size**: 64
- **Epochs**: 10+ (adjustable)

## Output
After training, the model generates reconstructed images from the test set. The results can be visualized using `matplotlib`.

## Results
Example of reconstructed images after training:

### Linear AutoEncoder:
![image](https://github.com/user-attachments/assets/c4719e5c-acbb-42c4-a622-26b85807170e)

### CNN based AutoEncoder
![image](https://github.com/user-attachments/assets/0495abf0-769a-4df1-b1b6-72cbc1225449)


## License
This project is open-source under the MIT License.

