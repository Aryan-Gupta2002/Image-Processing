# 🧠 Image Denoising Techniques Comparison

This project presents a comprehensive comparison of **classical image denoising techniques**, **ensemble methods**, and **deep learning-based models**. The goal is to evaluate their performance on different types of noise using quantitative and visual analysis.

---

## 📌 Overview

Image denoising is a fundamental task in computer vision used to remove noise while preserving important details.

This project explores:

* Classical filtering techniques
* Ensemble-based denoising
* Deep learning approaches (CNN Autoencoder & ResUNet)

Evaluation is performed using:

* **PSNR (Peak Signal-to-Noise Ratio)**

---

## 🛠️ Techniques Implemented

### 🔹 Classical Filters

* Wavelet Denoising
* Total Variation (TV) Denoising
* Gaussian Filter
* Median Filter
* Bilateral Filter

### 🔹 Ensemble Method

* Combines outputs of multiple filters
* Improves robustness by averaging strengths of individual methods

### 🔹 Deep Learning Models

* **CNN Autoencoder**

  * Learns mapping from noisy → clean images
* **ResUNet**

  * U-Net architecture with residual connections
  * Preserves spatial details and improves reconstruction quality

---

## 🔊 Noise Types Used

* Gaussian Noise
* Poisson Noise
* Combined Noise (Gaussian + Poisson)

---

## 📊 Evaluation Metric

* **PSNR (Peak Signal-to-Noise Ratio)**

  * Higher PSNR indicates better image quality after denoising

---

## 🧪 Pipeline

1. Load dataset of images
2. Convert to grayscale and normalize
3. Add synthetic noise (Gaussian, Poisson, Combined)
4. Apply:

   * Classical filters
   * Ensemble method
   * Deep learning models
5. Compute PSNR scores
6. Visualize results

---

## 🧠 Model Architectures

### 🔹 CNN Autoencoder

* Encoder: Convolution + Pooling
* Decoder: Upsampling + Convolution
* Loss: Mean Absolute Error (MAE)

### 🔹 ResUNet

* Encoder-Decoder structure
* Skip connections (U-Net)
* Residual blocks for improved learning
* Custom loss based on PSNR

---

## 📈 Results Summary

| Method            | Performance                       |
| ----------------- | --------------------------------- |
| Classical Filters | Fast but limited                  |
| Ensemble Method   | Better than individual filters    |
| CNN Autoencoder   | Learns noise patterns effectively |
| ResUNet           | Best performance (highest PSNR)   |

---

## 📷 Visualization

The project includes visual comparisons of:

* Original images
* Noisy images
* Denoised outputs from each method

---

## 📂 Dataset

* Images are loaded from a specified folder
* Converted to grayscale
* Normalized to range [0, 1]

---

## 🚀 How to Run

1. Open the notebook in **Google Colab / Jupyter**
2. Mount Google Drive (if required)
3. Update dataset path:

   ```python
   input_folder = "your_dataset_path"
   ```
4. Run all cells sequentially

---

## 📦 Dependencies

* Python 3.x
* NumPy
* OpenCV
* Matplotlib
* scikit-image
* TensorFlow / Keras
* scikit-learn
* Pandas

---

## 🎯 Key Learnings

* Classical methods are simple but limited
* Ensemble methods improve stability
* Deep learning significantly outperforms traditional methods
* ResUNet provides the best balance of detail preservation and noise removal

---

## 📌 Future Improvements

* Use larger datasets
* Train deeper architectures
* Try GAN-based denoising
* Real-world noisy datasets instead of synthetic noise

---

## 👤 Author

Aryan Gupta
GitHub: https://github.com/aryan-gupta2002

---

## ⭐ If you found this useful, consider giving it a star!
