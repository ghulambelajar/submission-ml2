# 🤖 Autoencoder untuk Dataset Sign Language MNIST

Proyek ini menggunakan model Autoencoder berbasis CNN (Convolutional Neural Network) untuk mempelajari representasi terkompresi (latent space) dari gambar tangan alfabet bahasa isyarat (ASL).  
Model dilatih untuk merekonstruksi kembali gambar berukuran 28x28 piksel dalam format grayscale.

---

## 📁 Dataset
- Sumber: [Sign Language MNIST – Kaggle](https://www.kaggle.com/datasets/datamunge/sign-language-mnist)
- Format: CSV, terdiri dari label dan 784 nilai piksel (28x28)

---

## 🔧 Arsitektur Model
- Encoder: 3 lapis Conv2D + ReLU + MaxPooling
- Decoder: 3 lapis ConvTranspose2D + ReLU + Sigmoid
- Dimensi latent space: 576 (hasil akhir dari encoder)

---

## 🏋️ Pelatihan
- Loss function: Mean Squared Error (MSELoss)
- Optimizer: Adam
- Jumlah epoch: 20

Model belajar mengenali pola gambar dan menghasilkan rekonstruksi yang cukup akurat.

---

## 📊 Visualisasi
- Perbandingan gambar asli vs hasil rekonstruksi
- Visualisasi latent space menggunakan t-SNE untuk melihat clustering berdasarkan label

---

## 💾 Output
- `autoencoder_signmnist.pth`: model hasil training
- Visualisasi tersedia di dalam notebook

---

## 🚀 Cara Menjalankan
Jalankan di Kaggle Notebook atau lingkungan Python lokal:

```python
!pip install torch torchvision
