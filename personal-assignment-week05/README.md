# Klasifikasi Sentimen Ulasan Steam (Positif vs Negatif) dengan LSTM

Proyek ini merupakan implementasi model deep learning untuk klasifikasi teks biner, dengan tujuan membedakan ulasan pengguna terhadap gim di platform Steam ke dalam dua kategori: positif dan negatif. Model ini dibangun menggunakan arsitektur Recurrent Neural Network (RNN), khususnya Long Short-Term Memory (LSTM), dengan framework TensorFlow/Keras.

Proyek ini dibuat untuk memenuhi tugas individu mata kuliah *Machine Learning 2*, dengan penekanan pada proses eksplorasi, evaluasi, dan analisis model secara mendalam.

---

## 🔧 Fitur Utama

- **Arsitektur RNN**: Menggunakan model LSTM untuk memahami urutan kata dalam ulasan pengguna secara kontekstual.
- **Dataset Nyata**: Dataset ulasan berasal dari pengguna asli Steam, mengandung opini nyata dengan variasi gaya bahasa dan panjang teks.
- **Eksperimen Terstruktur**: Disediakan konfigurasi fleksibel agar mudah melakukan pengujian dropout, epoch, dan parameter lainnya.
- **Evaluasi Lengkap**: Disediakan metrik akurasi, loss, confusion matrix, serta visualisasi kurva learning.
- **Komentar Kritis**: Notebook disusun dengan komentar untuk menjelaskan alasan setiap langkah dalam proses.

---

## 📃 Dataset

- **Sumber**: Steam Review & Games Dataset (file `output.csv`), berisi ribuan ulasan dengan label positif dan negatif.
- **Jumlah Data**: Digunakan 500 data ulasan: 250 positif dan 250 negatif.
- **Struktur Data**:
  - `content`: Teks ulasan gim
  - `is_positive`: Label asli ("Positive" / "Negative")

Contoh:

```
"At least it's a counter strike -1/100" → Negative
"So far my playthrough has been great" → Positive
```

---

## 📁 Struktur Proyek

```
├── ml2-assignment-week05.ipynb   # Notebook utama berisi seluruh kode dan analisis
├── Laporan_Tugas.pdf              # Laporan akhir
├── README.md                     # Berkas ini
```

> Catatan: Dataset tidak disertakan dalam repositori ini dan harus diunggah secara manual ke lingkungan kerja.

---

## ⚙️ Instalasi

Untuk menjalankan proyek ini secara lokal:

1. **Persyaratan**:

   - Python >= 3.8
   - pip package manager
   - Jupyter Notebook / VSCode / Google Colab

2. **Clone repository** (jika tersedia di GitHub):

```bash
git clone https://github.com/username/ml2-assignment-week05
cd ml2-assignment-week05
```

3. **Instal dependensi**

```bash
pip install -r requirements.txt
```

---

## 📊 Hasil Evaluasi

- **Akurasi Validasi Tertinggi**: ≃85.5%
- **Model Terbaik**: LSTM(64) dengan dropout 0.5
- **Evaluasi Tambahan**: Confusion matrix, classification report, dan kurva akurasi

---

## 📚 Referensi

- TensorFlow Official Docs
- Keras API Guide
- Steam Review Dataset (diambil dari archive ZIP)

---

## 👤 Penulis

Nama: Ghulam Mushthofa
NIM: 442023611060
Kelas: Machine Learning 2

