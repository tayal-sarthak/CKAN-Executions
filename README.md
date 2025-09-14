Purely testing purposes using C-KAN's 
# Convolutional KANs (C-KAN)

## Introduction
This repository contains an implementation of Convolutional Kolmogorov-Arnold Networks (C-KANs), which extend the concept of Kolmogorov-Arnold Networks to convolutional layers. This approach replaces traditional linear convolutions with learnable non-linear activations for each pixel, aiming for improved parameter efficiency and expressive power compared to standard Convolutional Neural Networks (CNNs).

## Original Authors & Source
The core implementation of the Convolutional KANs in this repository is almost entirely derived from the work of Antonio Tepsich and his collaborators.

**Authors:** Alexander Bodner, Antonio Tepsich, Jack Spolski, and Santiago Pourteau.
**GitHub Repository:** [AntonioTepsich/Convolutional-KANs](https://github.com/AntonioTepsich/Convolutional-KANs)
**Academic Paper:** "Convolutional Kolmogorov-Arnold Networks" (submitted June 19, 2024)

Please refer to their original work for a comprehensive understanding of the mathematical explanations and empirical evaluations.

## Files in this Repository
*   `convolution.py`: Low-level convolutional operations for KANs.
*   `KANConv.py`: KAN-based convolutional layer implementations.
*   `KANLinear.py`: Core Kolmogorov-Arnold Network (KAN) linear layer.
*   `test.py`: Defines the `KANC_MLP` model architecture.
*   `run_model.py`: Script to train and test the `KANC_MLP` model on MNIST. (By me)

## Usage
To run the MNIST demonstration:
1.  Ensure you have PyTorch and `torchvision` installed.
2.  Execute `run_model.py` using your Python 3 interpreter:
    ```bash
    /usr/local/bin/python3 run_model.py
    ```
    (Note: The script is currently configured to use a 10% subset of MNIST training data and a smaller `grid_size` for faster demonstration.)

## License
This is distributed under the MIT License. See the `LICENSE` file for more details.