📄 Project: U‑Net Implementation for Image Denoising
Overview
In this project, I implemented a U‑Net model to solve the problem of image denoising.

I used the CIFAR‑10 dataset, which contains 60,000 RGB images with dimensions of 32×32 pixels.

I artificially added Salt & Pepper noise to the images so that the model could learn to remove it.

What I Did
Data Preparation

Downloaded and loaded the CIFAR‑10 dataset.
Applied Salt & Pepper noise to create noisy versions of the images.
Model Design & Implementation

Coded the complete U‑Net architecture from scratch.
Set noisy images as inputs and the original clean images as outputs.
Training the Model

Trained the model using noisy–clean image pairs.
Used MAE and MSE metrics to measure and minimize reconstruction errors.
Evaluation

Ran the trained model on several test images.
Compared the noisy input, denoised output, and ground truth images side‑by‑side.
Plotted the loss curve, showing clear performance improvement over time.
Results
The model effectively removed Salt & Pepper noise.
The reconstructed images were visually very close to the originals.
Both MSE and MAE values were low, confirming strong model performance.
Extras
The full code, training process, data preprocessing steps, and visual results are included in this repository.
The image comparison approach made the model’s performance evaluation clear and interpretable.
