# 🖼️ U‑Net for Image Denoising (CIFAR‑10 + Salt & Pepper Noise)

## 📌 Overview
I developed a **U‑Net** deep learning model to remove **Salt & Pepper** noise from the **CIFAR‑10** dataset (60,000 RGB images, 32×32 px).  
The model restores noisy images to clean, high‑quality outputs.

---

## 🛠 Steps I Took

### 1️⃣ Data Preparation  
- Loaded CIFAR‑10 dataset.  
- Added Salt & Pepper noise to create noisy inputs.  
- Split into training and testing sets.

### 2️⃣ Model Design  
- Implemented the **U‑Net** architecture from scratch.  
- Inputs: noisy images. Outputs: clean ground‑truth images.

### 3️⃣ Training  
- Optimized using **MSE** and **MAE** loss functions.  
- Trained on noisy–clean image pairs.  
- Monitored loss values to ensure convergence.

### 4️⃣ Evaluation  
- Tested on unseen noisy images.  
- Compared **Noisy → Denoised → Original** side‑by‑side.  
- Plotted training loss curve to visualize improvement.

---

## 🎯 Results
- **High visual quality** — outputs closely match original images.  
- **Low reconstruction error** — MAE and MSE confirm strong performance.  
- Clear improvement shown through comparison visuals.

---

## 📂 Repository Contents
- `data_preprocessing.py` — adding noise & splitting data  
- `unet_model.py` — U‑Net implementation  
- `train.py` — training loop & loss plotting  
- `results/` — output images & evaluation plots

---

## 📸 Sample Output
*(Noisy → Denoised → Original)*

![Sample Output](results/sample.png)

---

## 🔗 Project Info
**Repository Name:** `unet-cifar10-denoise`  
**Short Description:** U‑Net model trained on CIFAR‑10 to remove Salt & Pepper noise, achieving high‑quality image restorations. Includes code, training logs, and visual comparisons.
